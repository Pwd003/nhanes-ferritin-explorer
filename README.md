# Ferritin Explorer | NHANES Research Models

Version 1.2.0 — research reproducibility demonstration (NHANES P03AA).

This browser-based, self-contained tool reproduces four frozen logistic equations for concurrent serum ferritin ≤30 ng/mL in nonpregnant women aged 20–44 years with haemoglobin ≥12 g/dL. Development: NHANES 2017–March 2020 (n=1,275; 385 cases); temporal validation: August 2021–August 2023 (n=825; 212 cases).

Open `index.html` in a browser or serve it with GitHub Pages. The calculator runs entirely in the browser without collecting or transmitting inputs. Do not enter identifiable or real patient data. This is not a clinical diagnostic, testing or treatment tool.

## Equations and missing inputs

The common hypothetical profile requires age, Hb, MCV, RDW and confirmation of eligibility. BMI and race/ethnicity may be omitted. A1 and HB_BASE require both BMI and race/ethnicity; NO_RACE requires BMI; CBC_ONLY requires neither. No default reference-category substitution or imputation is performed. Each equation uses its own frozen development-period coefficients. All model performance comparisons use the same complete-case temporal validation sample.

## Files

- `index.html`: standalone HTML, CSS, JS, frozen model and decision curve data.
- `frozen_coefficients.csv`: exact archived coefficient precision for the four calculator equations.
- `Synthetic_test_vectors.csv`: fictional profiles and reference predictions.
- `Browser_tests_v1.1.0.csv`: local browser regression checks for this presentation version.
- Remaining CSVs: aggregate validation and sensitivity results only. No participant-level NHANES records.

## Version history

1.2.0: public-facing name and page metadata revised. No changes to equations, JavaScript or embedded evidence. The v1.1.0 browser test record is retained as historical evidence.

1.1.0: presentation-only update; clearer research-use notice, collapsed evidence sections and local-processing policy. Model coefficients, original JS calculation logic and embedded DCA data unchanged.

## Citation and release

The accompanying manuscript is in preparation. Cite the specific release/commit and its version-specific archival DOI once available. Authorship and software license are to be confirmed by the study team before formal release.
