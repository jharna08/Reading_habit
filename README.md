## Reading Habit Analysis

## Initial Data Checks
Initial data checks were conducted to assess dataset quality, including identifying null values and duplicate records. Some columns contained missing values, and the dataset included two duplicate rows. One duplicate row was removed to maintain data accuracy.
Unique values were also reviewed across key categorical variables such as Race, Marital Status, Income, Education, and Employment to understand category distributions and ensure consistency.


## Fixing a Data Quality Issue in the Income Column
A data quality issue was identified in the Income column. The income range “1,00,000 to 1,50,000” appeared twice, but one version included an extra character ‘9’ at the beginning, making it an incorrect and separate string category.
This inconsistency was corrected using the replace() function to standardize income categories.

## Analysing Male and Female Readers
### Key Assumption: Respondents who reported reading zero books in the past 12 months were classified as non-readers. Only respondents who had read at least one book in the past year were retained in a separate dataframe for reader-focused analysis.
The gender composition among readers showed higher participation from females. Within the reader group, there were 1,329 female readers and 1,112 male readers.

### Why do females tend to read more?
Reading frequency can be influenced by factors such as employment type, retirement status, and part-time vs full-time work, which affect discretionary time available for leisure activities like reading.

The results indicate:

* The number of women employed without pay was more than double that of men.

* Among retired readers, female readers outnumbered male readers.

* In both part-time and full-time employment, female readers outnumbered male readers.

These employment patterns may be associated with greater schedule flexibility, potentially contributing to higher reading engagement.

## Analyzing readers across different races
The dataset contains seven racial categories, with White respondents representing 78.28% of the total sample. In absolute terms, White respondents also contributed the largest number of readers. However, absolute counts do not indicate higher reading tendency, as group sizes differ significantly.

To enable fair comparison, reading rates (proportion of readers within each race) were calculated. The findings show that:

* The highest reading rate was observed among Asian or Pacific Islander respondents, followed by mixed-race respondents.

* While White respondents formed the largest reader group numerically, reading participation was higher among Asian or Pacific Islander respondents.

### Why is the reading rate higher among Asian or Pacific Islander Respondents?
Education distribution appears to be a key factor. To evaluate this, education categories were grouped into a composite indicator called “college or higher”, combining:

* some college education

* college graduates

* postgraduates

This allowed consistent comparison of higher education exposure across racial groups. Asian or Pacific Islander respondents showed a notably higher representation in college-level education categories, which may explain their higher reading participation.
To validate whether education influences reading participation broadly, the relationship between higher education and reading rates was examined across all races. The results confirmed that higher education is strongly associated with higher reading participation across every racial group, not only among Asian or Pacific Islander respondents.

## Conclusion
This project explores reading habits using demographic factors like gender, race, income, education, and employment. After cleaning the dataset, readers were defined as those who read at least one book in the last 12 months. The analysis found higher female readership, the highest reading rate among Asian or Pacific Islander respondents, and a strong link between higher education and reading participation across all races.
