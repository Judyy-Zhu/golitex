# Showcase 15: Euclidean Geometry

This showcase packages the original split Euclidean-geometry knowledge base
with Problem 639, the perpendicular-bisector example.

## Structure

- `KB/definitions.lit` — primitive sets and helper functions such as vectors, dot products, squared distance, lines, and circles
- `KB/predicates.lit` — composite geometric predicates such as midpoint, perpendicularity, parallelism, and triangle relations
- `KB/theorems.lit` — the theorems and declared axioms used by the knowledge base
- `problem_639/main.lit` — the original Problem 639 statement and proof

The knowledge base is kept as three separate Litex modules. In particular,
`is_midpoint` and the other composite geometric relations belong to
`predicates.lit`; `definitions.lit` intentionally contains only the primitive
sets and helper functions. `problem_639` imports this local `KB`, so the
showcase does not depend on files outside its own directory.

## Run

From the repository root:

```bash
target/release/litex -compact -runner -r showcases/math_concepts_in_litex/15-Euclidean-Geometry/problem_639
```

The current KB contains declared axioms, including the predicate-form
perpendicular-bisector theorem used by Problem 639. Therefore this showcase is
run with normal dependency loading rather than presented as a fully strict,
axiom-free proof library.
