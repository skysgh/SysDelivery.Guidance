# New SELF Repository Migration Implementation Plan

## Purpose

This plan describes how to construct the proposed `TARGET` repository structure without losing source material, silently collapsing SELF concepts, or making the current repository unrecoverable. Migration is copy-first. No source item is moved or deleted until the target has been reviewed, verified, committed, pushed, and explicitly accepted.

## Current planning baseline

- Source folders represented in `target-index.md`: 483
- Source files considered: 2,021
- Unmapped source files: 0
- Existing numbered SELF entries recorded: 525
- Existing SELF identifiers occurring more than once: 88
- Mixed source folders requiring controlled file-level splits: 79
- Source folders containing low-confidence placements: 51
- Individual low-confidence file placements: 215
- Longest proposed folder path after adopting local folder numbers: 120 characters
- Physical folder names use local two-digit components; the complete SELF identifier is composed from the path.

These figures must be recalculated immediately before implementation in case the source repository changes.

## Safety principles

1. Copy first; never reorganise by moving the only existing copy.
2. Do not delete source folders during migration.
3. Record the source path, target path, size, extension, and SHA-256 hash for every file.
4. Preserve every existing SELF concept through an explicit coverage disposition.
5. Stop on an unplanned collision, unreadable file, missing source, hash mismatch, or path of 220 characters or longer.
6. Do not infer that similarly named files are duplicates; compare content hashes and, where necessary, document content.
7. Keep ambiguous items in a visible review queue rather than forcing a convenient classification.
8. Commit the migration in reviewable stages rather than as one opaque change.

## Phase 0 Repository freeze and baseline

### Actions

1. Confirm the authoritative source root and Git branch.
2. Record `git status`, current commit, configured remotes, and upstream branch.
3. Confirm whether the existing `TARGET` directory contains only planning artefacts.
4. Generate a fresh source inventory excluding `.git` and generated migration reports.
5. Record SHA-256 hashes for all source files.
6. Record empty directories separately because Git does not preserve them without placeholder files.

### Outputs

- `migration/source-inventory.csv`
- `migration/source-hashes.csv`
- `migration/source-empty-folders.csv`
- `migration/git-baseline.md`

### Gate 0

Proceed only when the inventory count agrees with the live source and the repository state is understood. Uncommitted user changes must not be overwritten or absorbed accidentally.

## Phase 1 Approve the New SELF taxonomy

### Actions

1. Review the proposed variable-depth destination tree in `target-index.md`.
2. Review all 525 extracted existing SELF entries.
3. Resolve the 88 duplicated existing identifiers.
4. Give every existing SELF entry one disposition:
   - preserved;
   - split into explicit concepts;
   - merged with traceability;
   - replaced;
   - intentionally retired;
   - unresolved.
5. Expand areas where current material or delivery risk shows that important work remains hidden.
6. Confirm local folder numbering and reserved numeric gaps.

### Outputs

- `migration/self-coverage.csv`
- Updated `target-index.md`
- `migration/taxonomy-decisions.md`

### Gate 1

No copying begins while an existing SELF concept lacks a disposition. Unresolved concepts remain visible and block final migration approval, although they may be copied into a review area during a controlled trial.

## Phase 2 Approve the file-level landing manifest

### Actions

1. Regenerate `index-shown.md` from the approved New SELF taxonomy.
2. Assign every source file exactly one proposed authoritative target path.
3. Review all mixed source folders marked `SPLIT`.
4. Review every low-confidence file placement using content, not merely its filename.
5. Identify exact duplicates by SHA-256 hash.
6. Identify variant documents that require a human choice rather than automatic deduplication.
7. Apply the naming rules:
   - local two-digit document order;
   - optional controlled state metadata;
   - no inherited SELF prefix in document filenames;
   - no ordering or state prefixes on media;
   - concise non-repeating names.
8. Check case-insensitive target collisions because Windows treats names case-insensitively.
9. Calculate the complete absolute path for every target file and shorten proposed names where required.

### Outputs

- `migration/file-map.csv`
- `migration/collision-report.csv`
- `migration/duplicate-content-report.csv`
- `migration/variant-review.md`
- Updated `index-shown.md`

### Gate 2

Required results:

- every source file occurs exactly once in the manifest;
- zero unexplained target collisions;
- zero paths of 220 characters or longer;
- no document folder exceeds the two-digit local-order capacity;
- every shortened name remains traceable to its source path;
- all forced placements have been accepted or remain explicitly quarantined.

## Phase 3 Build the empty target structure

### Actions

1. Create the approved folder tree beneath `TARGET`.
2. Use local folder components such as `[60]\[40]\[40]`.
3. Generate a machine-readable path-to-canonical-ID register.
4. Create `_media` only where media will actually be copied.
5. Do not create speculative empty branches merely for symmetry.

### Outputs

- `TARGET/INDEX.md`
- `TARGET/_self-paths.csv`
- Empty approved destination tree

### Gate 3

Compare the generated structure with `target-index.md`. Confirm that each physical path composes to the expected canonical SELF identifier.

## Phase 4 Trial migration

### Actions

1. Select representative material from:
   - a coherent one-destination folder;
   - a mixed folder requiring a split;
   - a deep Delivery branch;
   - a document with associated editable diagrams and rendered images;
   - an overlength source name requiring shortening;
   - a duplicate-content case;
   - a low-confidence placement.
2. Copy the sample into `TARGET`; do not move it.
3. Apply proposed names and `_media` placement.
4. Verify copied-file hashes against source hashes.
5. Open representative documents and diagrams to confirm they remain usable.
6. Review usability in Windows Explorer and Git.

### Outputs

- `migration/trial-report.md`
- `migration/trial-hash-verification.csv`

### Gate 4

The user reviews the trial tree. Any structural or naming problem changes the plan and regenerates the manifests before bulk copying.

## Phase 5 Full copy migration

### Actions

1. Copy files strictly from the approved file map.
2. Never overwrite an existing target path silently.
3. On collision, stop that item and record it; do not invent a new name during execution.
4. Preserve timestamps where practical, but use hashes—not timestamps—as the integrity authority.
5. Record every attempted copy and outcome.
6. Leave source files untouched.

### Outputs

- Populated `TARGET`
- `migration/copy-log.csv`
- `migration/copy-errors.csv`

### Gate 5

Required results:

- successful target file count equals approved manifest count;
- every target hash matches its intended source hash;
- zero unexplained extra target files;
- zero missing sources;
- zero silent overwrites.

## Phase 6 Structural and content validation

### Actions

1. Re-enumerate `TARGET` independently of the copy log.
2. Compare the independent inventory with the approved manifest.
3. Recalculate SHA-256 hashes.
4. Verify path lengths and case-insensitive uniqueness.
5. Check that document order values are unique within each folder.
6. Check that media names do not carry obsolete ordering or state prefixes.
7. Check links and references where they can be detected automatically.
8. Open a risk-based sample of DOCX, PDF, spreadsheet, Draw.io and image files.
9. Confirm that review and quarantine items remain visible.

### Outputs

- `migration/target-inventory.csv`
- `migration/target-hashes.csv`
- `migration/verification-report.md`
- `migration/link-review.csv`

### Gate 6

Migration passes only when every manifest item is accounted for and hash verification succeeds. Conceptual review findings may remain, but they must be listed rather than hidden.

## Phase 7 Git staging and safe remote backup

### Actions

1. Create a dedicated migration branch from the verified baseline.
2. Confirm `.gitignore` treatment for temporary, backup and generated verification files.
3. Stage the planning artefacts first and review the diff.
4. Commit the approved New SELF taxonomy and migration manifests.
5. Commit the generated target structure and copied content in logical groups.
6. Inspect `git status`, staged changes, rename detection, file counts, and repository size.
7. Push the migration branch to the configured GitHub remote.
8. Confirm the remote branch and commit IDs independently.

### Suggested commit sequence

1. `Document New SELF taxonomy and migration mapping`
2. `Create New SELF target structure`
3. `Copy management strategy investment and discovery material`
4. `Copy procurement and design material`
5. `Copy detailed delivery material`
6. `Copy transition operations and closure material`
7. `Add migration verification reports`

### Gate 7

Do not merge to the primary branch until the pushed branch is visible remotely and the local-to-remote commit relationship has been verified.

## Phase 8 Human acceptance

### Actions

1. Review the target tree on the work device where the documents can be opened.
2. Resolve variant documents and low-confidence placements.
3. Confirm that the detailed Delivery structure exposes the work SELF is intended to protect.
4. Confirm that browsing, searching and reading order are practical.
5. Update mappings and repeat verification for any accepted changes.

### Gate 8

The user explicitly accepts the target as the definitive candidate repository.

## Phase 9 Merge and later retirement of the old layout

### Actions

1. Merge the reviewed migration branch using a method that preserves an auditable history.
2. Pull or clone the merged repository into a separate clean location and verify it.
3. Retain the original source layout until the clean clone passes file-count and hash checks.
4. Archive or delete old folders only under a separate explicit instruction.

### Gate 9

Old source material is eligible for retirement only when:

- the definitive branch is on GitHub;
- a clean clone reproduces it;
- migration verification passes;
- unresolved variants have been retained visibly;
- the user explicitly authorises removal.

## Stop conditions

Implementation stops immediately if any of the following occurs:

- a source file disappears after baseline inventory;
- a target collision was not approved in the manifest;
- a copied hash differs from its source;
- a proposed path reaches 220 characters;
- a required SELF concept has no recorded disposition;
- the target contains an unexplained extra file;
- Git reports unexpected unrelated modifications;
- the remote branch cannot be verified;
- a command would require deleting or overwriting the only known copy.

## Implementation authority

Approval of this plan authorises creation and copy operations inside `TARGET` only after the corresponding gates pass. It does not authorise deletion of the existing repository layout, automatic selection between substantive document variants, merging to the primary branch, or removal of backup folders without an additional explicit decision.
