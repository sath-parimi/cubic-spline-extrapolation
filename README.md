# Cons of Cubic Spline Extrapolation
This project investigates the mathematical limitations of cubic spline extrapolation, focusing on the behavior of natural and quadratic boundary conditions. Using synthetic data and visualizations in Python, we analyze why these interpolation techniques often fail when extended outside the observed data range, particularly when x-values are large or unevenly spaced.

## Summary
- Goal: Visualize and assess how natural cubic and quadratic splines extrapolate outside known data ranges
- Data:
  - Scenario 1: `x² + N(0.5, 1)` — stochastic samples from a quadratic function
  - Scenario 2: `3x³ − 2x² + x` — randomized cubic polynomial with Gaussian noise
- Comparison: Natural cubic vs. quadratic spline extrapolation on both datasets
- Method: Constructed interpolants using `CubicSpline` and `interp1d` from SciPy, visualized their behavior beyond data boundaries

## Tools & Packages
- Python (Jupyter / Colab)
- `numpy`
- `matplotlib`
- `scipy.interpolate`

## Project Structure
- `cubic_spline_extrapolation_report.ipynb`: Main notebook with code, plots, and commentary
- `cubic_spline_extrapolation_report.html`: Static HTML export of the notebook (best for sharing)
- `figure-1.png` to `figure-4.png`: Key plots comparing extrapolation behavior
- `README.md`: This project overview

## Results
- Natural cubic splines extrapolated smoothly but tended to diverge quickly due to their higher-order continuity and boundary assumptions
- Quadratic splines offered more stable, local extrapolation but at the cost of overall smoothness
- Visualizations highlight differences in extrapolation direction and stability depending on the underlying function and noise

## How to Run
To reproduce this project locally:
1. Clone this repository or download the ZIP
2. Open `cubic_spline_extrapolation_report.ipynb` in Jupyter or Google Colab
3. Ensure all figure files (`figure-1.png` to `figure-4.png`) are in the same directory
4. Run all cells to view code, outputs, and conclusions

## View Project Deliverables
- [Full analysis report (HTML)](https://sath-parimi.github.io/cubic-spline-extrapolation/cubic_spline_extrapolation_report.html): Python notebook showing all code, spline constructions, extrapolation comparisons, and visualizations

## Authors
This project was completed collaboratively by UC Santa Barbara Students:
- Lin Fang  
- Sathvika Parimi  
- Katya Rodova  
- Aishvari Trivedi  
- Helen Zeng

## Notes
This repository is shared by Sathvika Parimi as part of a public academic portfolio. All content, including code, figures, and write-up, reflects joint work and shared contributions by the entire project team.
