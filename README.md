# 02-aerostructural-analysis-of-rocket-fin

# Aerostructural Assessment of a Rocket Fin

**Independent Engineering Research | August 2026**

An analytical investigation of whether static aerodynamic loading governs rocket fin thickness, combining classical aerodynamic theory, experimental data comparison, structural mechanics, and parametric sensitivity studies.

## Key Findings

* **Compared four aerodynamic models** against 25 published experimental measurements of the Army Navy Basic Finner across Mach 1.0 to 4.5.
* **Quantified model error:** the Ackeret modified model had an RMSE equal to 50.7% of the mean experimental coefficient; the finite strip refinement reduced this to 47.2%.
* **Investigated the source of prediction error:** finite span corrections alone did not resolve the discrepancy. Body fin shock and expansion wave interference was identified as a physically plausible explanation for further investigation.
* **Assessed structural loading:** at the selected representative Max Q condition, the calculated fin root bending stress was 2.63 MPa for the baseline 6061 T6 aluminum fin.
* **Explored thickness sensitivity:** even at half the baseline trailing edge thickness, the calculated yield factor of safety remained above 25 under the study's static loading assumptions.

## Engineering Approach

1. **Reference geometry:** Reconstructed the dimensioned Army Navy Basic Finner configuration in FreeCAD using published reference data.
2. **Aerodynamic modeling:** Applied Barrowman theory as a baseline, introduced an Ackeret supersonic correction, and investigated finite strip and fin tip Mach cone effects.
3. **Experimental comparison:** Compared predictions against 25 published aeroballistic range measurements and evaluated mean error, mean absolute error, root mean square error, and coefficient of determination.
4. **Structural assessment:** Applied the estimated aerodynamic load to a tapered wedge cantilever model and calculated bending stress, tip deflection, and yield margin.
5. **Sensitivity studies:** Examined changes in Mach number, fin thickness, material properties, and predicted structural response.

## Main Conclusion

The analysis indicates that static aerodynamic bending is unlikely to govern the baseline fin thickness under the modeled conditions. The isolated fin aerodynamic models also show substantial discrepancies against the experimental data. The results point toward body fin aerodynamic interference as a plausible missing mechanism and establish a direction for further model development.

## Limitations and Next Steps

The aerodynamic model does not resolve the full three dimensional flowfield, including coupled body fin shock interactions. The structural model is quasi static and does not establish flutter limits, dynamic response, root stress concentrations, or experimental structural validation. Future work could incorporate published body fin interference methods or CFD, then refine the structural assessment using dynamic and test based evidence.

The local buckling estimate also requires review before its reported safety factor is treated as a reliable design margin.

## Tools and Methods

* FreeCAD for reference geometry
* Excel for analytical calculations and sensitivity studies
* Classical aerodynamic theory and beam mechanics
* Statistical comparison against published experimental measurements

## Report

See the full technical report in this repository for assumptions, derivations, comparison tables, sensitivity studies, figures, references, and limitations.
