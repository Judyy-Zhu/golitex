# Coordinate Geometry Case Study

This showcase demonstrates formal verification of coordinate geometry problems using Litex.

## Structure

- **geo/**: Shared geometric definitions (flatten module)
- **problem_XXX/**: Individual verified problems (7 total)

Each problem is a standalone module that imports the geo library.

## Verification

From the repository root, verify any problem using:

```bash
# Verify a single problem
golitex verify showcases/math_concepts_in_litex/15_coordinate_geometry_case_study/problem_639

# Verify all problems
golitex verify showcases/math_concepts_in_litex/15_coordinate_geometry_case_study/problem_207
golitex verify showcases/math_concepts_in_litex/15_coordinate_geometry_case_study/problem_210
golitex verify showcases/math_concepts_in_litex/15_coordinate_geometry_case_study/problem_212
golitex verify showcases/math_concepts_in_litex/15_coordinate_geometry_case_study/problem_214
golitex verify showcases/math_concepts_in_litex/15_coordinate_geometry_case_study/problem_217
golitex verify showcases/math_concepts_in_litex/15_coordinate_geometry_case_study/problem_297
golitex verify showcases/math_concepts_in_litex/15_coordinate_geometry_case_study/problem_639
```

Note: problem_217 requires ~104s due to proof complexity.

## Problems Included

1. **problem_639**: Perpendicular bisector property (0.35s)
2. **problem_210**: Coordinate geometry proof (27.6s)
3. **problem_212**: Quadrilateral problem (6.7s)
4. **problem_214**: Angle congruence (29.9s)
5. **problem_217**: Extension and perpendicularity (101.2s)
6. **problem_297**: Geometric proof (69.6s)
7. **problem_207**: Square and angle bisector (63.6s)

**Total verification time**: ~299 seconds

## Important Notes

- For problems with `translation.lit`, export order matters: translation must come before solution
- The showcase root is a plain directory (no litex.config) to allow independent module verification
- All problems verified successfully as of 2026-09-03
