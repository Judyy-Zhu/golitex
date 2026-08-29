# Showcase 15: Euclidean Geometry

This showcase packages the original split Euclidean-geometry knowledge base
with Problem 639, the perpendicular-bisector example.

## Structure

- `KB/definitions.lit` — the complete definitions module (77 lines)
- `KB/predicates.lit` — the complete predicates module (196 lines)
- `KB/theorems.lit` — the complete theorems/axioms module (1917 lines)
- `problem_639/main.lit` — the original Problem 639 statement and proof

The three files under `KB/` are copied unchanged from the source `Litex/KB`
directory. `problem_639` imports this local `KB`, so the showcase does not
depend on files outside its own directory.

## Run

From the repository root:

```bash
target/release/litex -compact -runner -r showcases/math_concepts_in_litex/15-Euclidean-Geometry/problem_639
```

The current KB contains declared axioms, including the predicate-form
perpendicular-bisector theorem used by Problem 639. Therefore this showcase is
run with normal dependency loading rather than presented as a fully strict,
axiom-free proof library.
