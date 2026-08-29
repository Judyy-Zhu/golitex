# Concept Inventory

| Concept | Litex form | Location |
| --- | --- | --- |
| squared distance | `KB::definitions::distance_sq` | `KB/definitions.lit` |
| midpoint | `KB::predicates::is_midpoint` | `KB/predicates.lit` |
| perpendicularity | `KB::predicates::is_perpendicular` | `KB/predicates.lit` |
| perpendicular-bisector equidistance | `KB::theorems::perpendicular_bisector_equidistant_sq` | `KB/theorems.lit` |
| Problem 639 proof | `perpendicular_bisector_problem_639` | `problem_639/main.lit` |

Problem 639 assumes that `O` is the midpoint of `AB` and that `PO` is
perpendicular to `AB`, then applies the KB theorem to conclude
`distance_sq(P, A) = distance_sq(P, B)`.
