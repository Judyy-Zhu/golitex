# Concept Inventory

| Concept | Litex form | Role |
| --- | --- | --- |
| squared distance | `definitions::distance_sq` | avoids square roots while expressing equidistance |
| perpendicular dot product | `definitions::perpendicular_dot` | gives a direct coordinate test for `PO ⟂ AB` |
| midpoint | `predicates::is_midpoint` | records the two coordinate midpoint equations |
| perpendicularity | `predicates::is_perpendicular` | packages the zero-dot-product condition |
| perpendicular bisector theorem | `theorems::perpendicular_bisector_equidistant` | proves equal squared distances from midpoint and perpendicularity |

The proof expands both predicates, rewrites each coordinate using the midpoint
equations, applies the difference-of-squares identity, and converts the sum of
the two coordinate differences to twice the perpendicular dot product.

The scope is deliberately analytic and two-dimensional. It does not import the
synthetic Tarski development in Showcase 14, define square roots, or claim a
full Euclidean geometry library.
