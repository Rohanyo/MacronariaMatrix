# MacronariaMatrix v1.0.0

**Release date:** 2026-09-18

MacronariaMatrix v1.0.0 is the frozen first release of the curated cross-matrix character-concept database for the eight analysed Macronarian/titanosauriform morphological phylogenetic datasets used in this project titled: 'Decoupling the effects of Decoupling Taxon Completeness and Phylogenetic Instability in Macronarian Sauropod Morphological Datasets' as well as 'Historical inheritance and expansion of morphological character sampling in macronarian sauropod phylogenetics'

## Freeze status

- **855 active canonical character concepts**
- **2,377 biological character occurrences** across the eight analysed matrices
- **234 Wilson (2002) reference-layer occurrences**
- **87 canonical-ID redirects**
- **0 active concepts remaining under review**
- **12 concepts represented in all eight analysed matrices**

The freeze is conservative: when equivalence could not be demonstrated from the supplied project sources, concepts were retained as distinct rather than forcibly merged.

## Final residual audit

The last 45 review candidates were resolved in Phase 7. Six additional redirects were applied:

- `MC0351 -> MC0273` — anterior/cranial dorsal neural-spine orientation
- `MC0855 -> MC0111` — posterior dorsal/sacral neural-spine height relative to centrum length
- `MC0474 -> MC0366` — proximal/anteriormost caudal centrum elongation
- `MC0476 -> MC0368` — middle-caudal centrum elongation
- `MC0637 -> MC0448` — metacarpal IV–V articulation morphology
- `MC0658 -> MC0462` — posterior astragalar projection

Two M19 compound parents remain active historical concepts:
- `MC0537`, decomposed in M26 into `MC0916` and `MC0924`
- `MC0581`, decomposed in M26 into `MC0917` and `MC0937`

## Dataset counting rules

- W02/WE14: **246 biological characters**, **250 encoded columns**
- DE12: **119 biological characters**, **121 encoded columns**
- Encoding-only columns do not receive canonical biological-character IDs.

## Highest pairwise canonical overlap

- **WU09–KN10: Jaccard 0.963, 234 shared concepts**
- **WU09–W02: Jaccard 0.951, 234 shared concepts**
- **M19–M26: Jaccard 0.945, 546 shared concepts**
- **KN10–W02: Jaccard 0.918, 234 shared concepts**
- **WU09–C12: Jaccard 0.609, 215 shared concepts**

## Repository structure

- `data/` — frozen core CSV tables
- `audit/` — final residual audit and freeze manifest
- `figures/` — final persistence and overlap figures
- `documentation/` — data dictionary

Superseded canonical IDs remain permanently traceable in `data/canonical_id_redirects.csv` and the `original_canonical_character_id` column of the occurrence table.
