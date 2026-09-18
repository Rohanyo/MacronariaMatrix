# MacronariaMatrix v1.0.0 — data dictionary

## Core tables

### `data/character_concepts.csv`
One row per active canonical character concept. Canonical IDs are frozen for v1.0.0.
Occurrence counts and matrix-presence fields are recalculated after all redirects.

### `data/character_occurrences.csv`
One row per character occurrence in an analysed matrix or the Wilson (2002) reference layer.
`canonical_character_id` gives the frozen v1.0.0 ID.
`original_canonical_character_id` preserves the pre-redirect assignment.

### `data/character_relationships.csv`
Explicit historical, split, merged, modified, and related-character relationships.
The final residual audit adds relationship rows for the last six redirects.

### `data/canonical_id_redirects.csv`
Permanent redirect ledger. Superseded IDs must not be reused for new concepts.

### `data/matrix_character_summary.csv`
Biological character counts, encoded-column counts, and unique canonical concepts for each analysed matrix.

### `data/matrix_character_overlap.csv`
Pairwise shared concepts, unions, Jaccard similarity, and directional containment.

### `data/concept_persistence_summary.csv`
Distribution of canonical concepts by the number of analysed matrices in which they occur.

### `data/universal_concepts.csv`
Canonical concepts represented in all eight analysed matrices.

### `data/encoding_only_columns.csv`
Analytical encoding columns that are not independent biological character concepts.

## Audit tables

### `audit/final_residual_audit.csv`
Final decisions for the last 45 concepts that remained under review after Phase 6.

### `audit/freeze_manifest.csv`
Release-level counts and freeze metadata.
