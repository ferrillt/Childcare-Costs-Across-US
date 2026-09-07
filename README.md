# Childcare Costs Across the United States
![Childcare affordability dashboard](images/childcare_affordability_dashboard.png)

## Project Overview

Childcare is a significant household expense that can affect
family finances, employment decisions, and workforce participation.
This project uses the National Database of Childcare Prices to examine
how weekly childcare prices vary across states, regions, age groups,
and care settings in the United States.

The analysis translates a large public dataset into visual comparisons
intended for policymakers, workforce planners, organizational leaders,
parents, and other audiences interested in childcare affordability.

## Questions Examined

This project examines the following questions:

- How do childcare prices vary across U.S. states and regions?
- How do center-based and family childcare prices compare?
- Which age group has the highest childcare prices?
- Which states appear at the upper and lower ends of the price range?
- What do these differences suggest about childcare affordability?

## Dataset

The project uses the National Database of Childcare Prices published
by the U.S. Department of Labor Women's Bureau.

The dataset contains county-level childcare price estimates and
related demographic and economic variables. Childcare prices are
provided by care setting and children's age group.

Key fields used in this analysis include:

- `State_Abbreviation`
- `MCInfant`
- `MCToddler`
- `MCPreschool`
- `MFCCInfant`
- `MFCCToddler`
- `MFCCPreschool`

`MC` represents center-based childcare, while `MFCC` represents
family childcare or home-based care. The price variables represent
weekly childcare prices.

[View the National Database of Childcare Prices](https://www.dol.gov/agencies/wb/topics/featured-childcare)

## Analysis Process

The analysis was completed in Python using a Jupyter Notebook. The
process included:

1. Loading and reviewing the childcare dataset.
2. Examining missing values.
3. Comparing mean and median weekly prices.
4. Comparing center-based care with family childcare.
5. Calculating average prices by state and age group.
6. Identifying higher-cost states.
7. Assigning states to geographic regions.
8. Comparing regional childcare-price patterns.
9. Creating charts for a dashboard, presentation, and infographic.

## Principal Findings

The analysis produced several notable findings:

- Childcare prices vary considerably across states and regions.
- Center-based care is generally more expensive than family childcare.
- Center-based care averaged approximately $133 per week, compared
  with approximately $108 per week for family childcare in the
  analyzed observations.
- Infant care was consistently the most expensive age category.
- Infant care was approximately 15% more expensive than the combined
  average for toddler and preschool care.
- Massachusetts appeared at the higher end of the family childcare
  price comparison, while Mississippi appeared at the lower end.
- Family childcare prices were highest in the Northeast and lowest
  in the South in the regional comparison.

These findings demonstrate that childcare affordability depends on
where a family lives, the age of the child, and the type of care used.

## Technologies

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- Seaborn
- Microsoft PowerPoint

## Repository Contents

| Folder | Contents |
|---|---|
| `analysis` | Jupyter Notebook containing the Python analysis |
| `data` | Compressed National Database of Childcare Prices dataset |
| `presentations` | Dashboard and narrative presentation files |
| `reports` | Complete written analysis in PDF format |

## Project Materials

- [View the Jupyter Notebook](analysis/Childcare_Analysis_JupyterNotebookCode.ipynb)
- [View the written analysis](reports/Childcare_Costs_Across_US_analysis.pdf)
- [View the narrative presentation](presentations/Childcare_Costs_Economic_Strain.pptx)
- [View the dashboard presentation](presentations/Dashboard_Childcare_Affordability.pptx)

## Running the Analysis

### Requirements

Install Python 3 and the required packages:

    pip install pandas numpy matplotlib seaborn jupyter

Clone the repository:

    git clone https://github.com/ferrillt/Childcare-Costs-Across-US.git

Move into the repository:

    cd Childcare-Costs-Across-US

Start Jupyter Notebook:

    jupyter notebook

Open:

    analysis/Childcare_Analysis_JupyterNotebookCode.ipynb

Run the notebook cells in order.

## Assumptions and Limitations

- Missing childcare-price values were excluded from applicable
  calculations.
- State averages were calculated from the observations available in
  the dataset.
- The analysis does not adjust childcare prices for regional
  cost-of-living differences or inflation.
- The analysis combines observations from multiple study years.
  Consequently, the results should not be interpreted as current
  childcare prices for a particular year.
- State-level comparisons may not represent prices in individual
  cities or communities.
- Childcare prices alone do not provide a complete measure of
  affordability.
- Provider availability, childcare quality, public assistance,
  household income, and the number of children in a household were
  not incorporated into the comparisons.
- The results identify price differences but do not establish why
  those differences exist.

## Ethical Considerations

The dataset is publicly available and does not contain personal
information about individual families. The project avoids attributing
causes to observed price differences when those causes cannot be
established from the data. Findings are presented as descriptive
comparisons rather than guarantees about what an individual family
will pay.

## Potential Enhancements

Future work could:

- Examine price changes over time instead of combining study years.
- Adjust prices for inflation and regional cost of living.
- Compare childcare prices with household income.
- Incorporate provider availability and childcare-assistance programs.
- Develop an interactive web-based dashboard.
- Examine county-level differences within individual states.

## Author

Teresa Ferrill
