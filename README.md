# Cons of Cubic Spline Extrapolation
This project investigates the mathematical limitations of cubic spline extrapolation, focusing on the behavior of natural and quadratic boundary conditions. Using synthetic data and visualizations in Python, we analyze why these interpolation techniques often fail when extended outside the observed data range, particularly when x-values are large or unevenly spaced.

## Summary
- Topic: Extrapolation limitations of cubic splines due to boundary conditions
- Methods: Implemented natural cubic and quadratic spline interpolation on synthetic data
- Data: Noisy samples from x² + N(0.5, 1) and 3x³ − 2x² + x
- Key Findings: Both spline types behave well within data bounds but diverge significantly when extrapolated. Natural splines flatten at boundaries due to second-derivative constraints; quadratic splines lack the flexibility to match curvature outside range.

## Tools & Packages
- Python (Colab / Jupyter)
- `numpy`
- `matplotlib`
- `scipy.interpolate`

## Project Structure
- `spline_extrapolation.ipynb`: Main notebook with code, analysis, and figures
- `spline_extrapolation.html`: Exported report (hosted on GitHub Pages)
- `figure-1.png` through `figure-4.png`: All figures used in the notebook and report
- `README.md`: Project overview and background

## View Project Deliverables
- [Full analysis report (HTML)](https://sath-parimi.github.io/cubic-spline-extrapolation/spline_extrapolation.html): Python notebook showing all code, spline constructions, extrapolation comparisons, and visualizations

## Collaborators
This project was completed collaboratively by UC Santa Barbara Students:
- Lin Fang  
- Sathvika Parimi  
- Katya Rodova  
- Aishvari Trivedi  
- Helen Zeng

## Notes
This repository is shared by Sathvika Parimi as part of a public academic portfolio. All content, including code, figures, and write-up, reflects joint work and shared contributions by the entire project team.
