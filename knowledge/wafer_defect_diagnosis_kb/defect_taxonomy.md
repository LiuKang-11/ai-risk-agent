# Defect Taxonomy

## Supported classes
- `Center`: defect concentration in the wafer center region
- `Donut`: annular ring around center with cleaner center and outer edge
- `Edge-Loc`: localized defect cluster near one edge sector
- `Edge-Ring`: continuous or near-continuous ring near wafer perimeter
- `Loc`: one or more compact local hotspots away from a simple ring
- `Random`: spatially dispersed defects without strong geometry
- `Scratch`: linear or curving streak consistent with contact damage
- `Near-full`: defects cover most of the wafer surface
- `None`: no meaningful defect pattern detected

## Classification rules
- prefer the simplest class that explains the dominant geometry
- if two classes are both strong, return dominant class plus mixed-pattern note
- use `None` only when signal is absent, negligible, or clearly non-defect noise

## Dominance heuristic
- dominant area coverage
- spatial concentration
- repeatability across wafers
- agreement between model output and extracted features
