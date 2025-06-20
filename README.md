# Walkability in Corpus Christi

This project uses Bayesian causal inference to analyze the relationship between population density, job density, and road network density on walkability in Corpus Christi, TX. The analysis is based on publicly available data from the EPA’s National Walkability Index and uses Directed Acyclic Graphs (DAGs) and counterfactual simulations to explore causal effects.

## 📄 Project Summary

- **Data Source**: Smart Location Database (SLD) from [data.gov](https://catalog.data.gov/dataset/walkability-index1)
- **Modeling Framework**: Bayesian regression using `rethinking` and `dagitty` packages in R
- **Key Insight**: Road density is the most influential predictor of walkability, followed by job and population density.

## 📁 Repository Contents

- `FinalProject.Rmd`: R Markdown source code for the analysis
- `FinalProject.pdf`: Rendered PDF report

## 🔧 Dependencies

This project uses R and the following packages:
- `rethinking`
- `dagitty`
- `tidyverse`

Install via:

```R
install.packages("dagitty")
remotes::install_github("rmcelreath/rethinking")
```

## 📈 Highlights

- Constructed and tested a DAG to model causal relationships
- Used `quap()` and `ulam()` for parameter estimation
- Compared quadratic approximation and HMC
- Generated counterfactual plots to visualize causal effects

## 📜 License

This project is licensed under the MIT License.
