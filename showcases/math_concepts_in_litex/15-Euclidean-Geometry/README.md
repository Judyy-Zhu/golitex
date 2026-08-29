# Euclidian Geometry System

This standalone analytic-geometry showcase proves the perpendicular bisector
theorem over Cartesian points in `R²`:

> If `O` is the midpoint of `AB` and `PO` is perpendicular to `AB`, then `P`
> is equidistant from `A` and `B`.

The Litex source remains split into the requested layers:

- `definitions.lit` defines squared distance and the perpendicular dot product;
- `predicates.lit` defines midpoint and perpendicularity predicates;
- `theorems.lit` proves the general equidistance theorem from those predicates;
- `main.lit` checks the concrete configuration
  `A = (0,0)`, `B = (4,0)`, `O = (2,0)`, `P = (2,3)` and obtains squared
  distances `13` on both sides.

Run it from the repository root:

```bash
target/release/litex -compact -runner -r showcases/math_concepts_in_litex/15-Euclidean-Geometry
```

The project has no external KB import. The theorem is proved directly by
explicit coordinate algebra.
