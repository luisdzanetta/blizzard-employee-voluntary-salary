# Blizzard Employee Voluntary Salary Analysis

## Business Question

In 2020, Blizzard Entertainment employees circulated an anonymous salary spreadsheet amid growing concerns about compensation equity. This analysis asks: **are salary premiums and raise percentages distributed consistently across performance levels and seniority tiers — or do the patterns suggest structural inequity that could drive talent retention risk?**

Understanding compensation equity matters in game studios because cross-functional team stability over multi-year development cycles has a measurable impact on product quality and shipping cadence. Disproportionate raises for specific functions, independent of performance, may indicate market-pressure-driven compensation rather than merit-based structures.

## Installation Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/luisdzanetta/blizzard-employee-voluntary-salary.git
   cd blizzard-employee-voluntary-salary
   ```

2. **Install required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Data Source

Self-reported salary data collected via anonymous employee survey in 2020.  
Dataset: [Kaggle — Blizzard Employee Voluntary Salary Info](https://www.kaggle.com/datasets/mexwell/blizzard-employee-voluntary-salary-info)

**Key caveat:** Participation was voluntary and anonymous, which introduces selection bias — respondents may skew toward employees with stronger opinions about compensation. All conclusions should be interpreted in light of this limitation.

## Project Structure

```plaintext
.
├── data/                                   # Raw dataset
├── README.md                               # Project documentation
├── exploratory-data-analysis.ipynb         # Main analysis notebook
├── exploratory-data-analysis.py            # Script version
├── requirements.txt                        # Dependencies
└── LICENSE
```

## Key Findings

**Salary premiums are consistent across seniority levels, but not equally distributed across functions.**  
Software Engineers at all levels (entry through principal) report salaries above the external market range by 20–43%, with the largest premium at the principal level lower bound (+43%). However, this premium is concentrated in engineering roles — non-engineering functions show a wide salary spread with a median 45% below the SE median.

**Raise percentages are significantly higher for Software Engineers (Mann-Whitney U test, p < 0.05).**  
The difference in raise percentages between SE and non-SE employees is statistically significant, suggesting that raises are being used as a market-correction mechanism for engineering talent specifically, independent of performance rating distribution — which is similar across both groups.

**Performance rating does not predict salary level within the SE population.**  
Senior engineers rated "Developing" report salaries comparable to peers rated "High" or "Top," which may reflect pay-band rigidity or seniority-based progression rather than performance-driven compensation.

## Limitations

**Sample bias:** The dataset represents only employees who chose to participate in the anonymous survey. Employees with outlier salaries (very high or very low) may be overrepresented.

**External market data:** The salary benchmarks used for comparison are sourced from a single reference (2023 data applied to 2020 salaries), which introduces measurement uncertainty. Comparisons should be treated as directional, not precise.

**Observational data:** All findings are correlational. Causal claims about Blizzard's compensation strategy cannot be made from self-reported cross-sectional data.

## References

1. [Wikipedia — Blizzard Entertainment](https://en.wikipedia.org/wiki/Blizzard_Entertainment)
2. [Time, 2020 — Blizzard Wage Disparities](https://time.com/5875371/blizzard-wage-disaparities/)
3. [Bloomberg, 2020](https://www.bloomberg.com/news/articles/2020-08-03/blizzard-workers-share-salaries-in-revolt-over-wage-disparities)
4. [OpenIntro Dataset](https://www.openintro.org/data/index.php?data=blizzard_salary)
5. [Kaggle Dataset](https://www.kaggle.com/datasets/mexwell/blizzard-employee-voluntary-salary-info)
6. [Ellow — Contract vs Full-Time](https://ellow.io/contract-work-vs-full-time-employment/)
7. [IT Career Finder — Software Engineer Salaries](https://www.itcareerfinder.com/brain-food/it-salaries/computer-software-engineer-salary-range.html)

## Contact

**Luís D'Avoglio Zanetta**  
luis.dzanetta@gmail.com | [GitHub](https://github.com/luisdzanetta)
