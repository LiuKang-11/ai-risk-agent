# Defect Geometry Reference

## Center
- highest density in central region
- usually radially symmetric or softly clustered

## Donut
- ring-shaped concentration around center
- center remains cleaner than surrounding annulus

## Edge-Loc
- concentrated patch near perimeter
- limited arc length rather than full-ring coverage

## Edge-Ring
- continuous or broad annular band near edge
- often follows full circumference or most of it

## Loc
- compact hotspot or several localized islands
- not constrained to center or edge geometry

## Random
- low-structure, dispersed points
- weak center, edge, and linear scores

## Scratch
- elongated line or curve
- often single-direction or contact-path aligned

## Near-full
- dense coverage across most die positions
- often associated with contamination or catastrophic process excursion

## None
- sparse or background-only pattern

## Feature interpretation
- high edge density supports `Edge-Loc` or `Edge-Ring`
- high ring score supports `Donut` or `Edge-Ring`
- high scratch-line score supports `Scratch`
- high center density supports `Center`
- high randomness score with low structure supports `Random`
