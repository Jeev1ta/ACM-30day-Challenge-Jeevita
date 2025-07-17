During the Day 1 tasks, I learned the fundamentals of data cleaning, including the three main approaches to handling missing values. I also explored how to detect outliers, understood their common causes, and practiced data visualization using scatter plots and box plots.

# Burnout Breakdown – Day 1 Summary
Loaded dataset and checked for missing values using .isnull().sum()
- No missing data, but used median for numeric and mode for categorical as a safe imputation strategy.

Capped extreme values:
- WorkHoursPerWeek max at 126 hrs/week
- SleepHours max at 16 hrs/day

Removed outliers using the IQR method for WorkHoursPerWeek and SleepHours

Visualized key relationships:
- Scatter Plot: SleepHours vs StressLevel colored by BurnoutLevel
- Box Plot: Age vs BurnoutLevel

Key Learnings:
- Missing data handling (median/mode)
- Outlier detection (IQR, boxplot)
- Data cleaning best practices
- EDA with scatter and box plots
