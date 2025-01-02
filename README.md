# Fuzzy Project Success

This repository contains the Julia code that supports the paper **"A Fuzzy Approach to Project Success: Measuring What Matters"**, submitted to the **2025 IEEE International Conference on Fuzzy Systems**. The code demonstrates a fuzzy logic-based framework for evaluating project success, utilizing a hierarchical Type-1 Mamdani fuzzy inference system.

## Overview

The methodology implemented here addresses the inherent complexities and uncertainties in evaluating project success by leveraging the power of fuzzy logic. The system evaluates three core dimensions of project success:

1. **Project Management Success (PMS):** Assesses dimensions such as time, budget, team satisfaction, and startup problems.
2. **Project Impact Success (PIS):** Focuses on outcomes like user adoption, sustainability, and positive impact for end users.
3. **Stakeholder Satisfaction (SS):** Evaluates satisfaction levels of key stakeholders, including beneficiaries and donors.

These dimensions are aggregated at the final level to compute a comprehensive **Project Success (PS)** score.

## Features

- **Hierarchical Mamdani Fuzzy Inference System:** Modular structure for evaluating success at multiple levels.
- **Fuzzification and Defuzzification:** Converts input variables into fuzzy sets and produces interpretable, crisp success scores.
- **Flexible Membership Functions:** Incorporates linear and triangular membership functions to represent key project attributes.
- **Visualization:** Provides plots to visualize the fuzzy outputs for each dimension and the final project success score.

## Code Structure

The repository includes the following sections:

1. **Project Management Success:** Code and explanation for defining and evaluating the PMS dimension.
2. **Project Impact Success:** Code and explanation for evaluating the PIS dimension.
3. **Stakeholder Satisfaction:** Code and explanation for assessing SS.
4. **Final Aggregation (Project Success):** Combines the three dimensions into a single Project Success score.
5. **Graphs and Visualization:** Plots the fuzzy logic outputs for each dimension and the overall score.

## Requirements

To run this code, you need to have Julia installed along with the following packages:

- [Plots.jl](https://github.com/JuliaPlots/Plots.jl) for visualizations.
- [FuzzyLogic.jl](https://github.com/azcunaga/FuzzyLogic.jl) for fuzzy logic implementation.

You can install these packages by running:
```julia
using Pkg
Pkg.add("Plots")
Pkg.add("FuzzyLogic")
```

## Usage

Clone this repository:
```bash
git clone https://github.com/joaojcorreia/FuzzyLogic_ProjectSuccess.git
cd FuzzyLogic_ProjectSuccess
```

Open the `fuzzy_project.jl` file in Julia.

Run the file to see:

- Definitions of fuzzy sets and rules.
- Aggregated fuzzy outputs for each project success dimension.
- Visualization of results for PMS, PIS, SS, and overall PS.

Modify inputs or rules as needed to adapt the model to your specific project evaluation requirements.

## Plots

The code includes visualization for:

- Project Management Success
- Project Impact Success
- Stakeholder Satisfaction
- Overall Project Success

These plots help interpret the fuzzy outputs and provide insights into how various dimensions contribute to the final project success score.

## Citation

If you use this code, please cite the accompanying paper:

Granja-Correia, J., Hernández-Linares, R., Ferranti, L., & Rego, A. "A Fuzzy Approach to Project Success: Measuring What Matters," Proceedings of the 2025 IEEE International Conference on Fuzzy Systems, DOI to be updated upon publication.

## License

This repository is licensed under the MIT License. See the LICENSE file for details.
