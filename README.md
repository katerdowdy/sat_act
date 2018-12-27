# SAT vs. ACT: Analyzing Participation Rates, 2017-2018

## Executive Summary

> The majority of four-year colleges and universities across the U.S. require prospective students to submit scores from either the SAT or ACT as part of their application. Holding both tests to be equally challenging and rigorous, we would expect to see a fairly even proportion of students who choose to take either test for their college admissions. However, 2018 data demonstrates a 16.7% difference in average state-wide participation rates, with the SAT lagging behind the ACT.

### Problem Statement
This analysis seeks to explore what factors are behind this participation gap, and to make recommendations to the College Board on where to focus their efforts to rebuild and grow participation rates for the SAT in 2019-2010. 

### Description of Data
The final dataset used for this analysis consists of aggregate participation rates and average scores on the SAT and ACT for each state and the District of Columbia. Data came from these sources:
- [2018 ACT Data](http://www.act.org/content/dam/act/unsecured/documents/cccr2018/Average-Scores-by-State.pdf)
- [2018 SAT Data](https://reports.collegeboard.org/sat-suite-program-results/state-results) 
- [2017 ACT Data](https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows)
- [2017 SAT Data](https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/)

#### Data Dictionary 
<img src="../Project-1/Images/data_dictionary.png">

The dataframe is 51 rows x 17 columns. SAT data for both years includes a breakdown of state average scores for each section of the SAT; the ACT data only includes section averages for 2017. 

**Participation Rates**

The ACT saw a higher aggregate average participation rate than the SAT in both 2017 and 2018, although a 5% participation increase in the average SAT participation rate and 3% decrease on the ACT participation rate from 2017 saw that gap decline to 16.7% in 2018. (This data compares state averages, not the average of all U.S. students participating on either test - comparing those averages, the SAT is actually ahead of the ACT (source: https://www.washingtonpost.com/education/2018/10/23/sat-reclaims-title-most-widely-used-college-admission-test/?utm_term=.d2bd83ee7b24)).

Looking at 2017 distributions for participation rates for both tests (which didn't change much in 2018), it appears the ACT benefits from a large cluster of states administering the ACT at 90-100% participation. Conversely, a similar number of states (likely the same states with high ACT participation) had very low participation on the SAT in 2017 (0-20%), bringing down the average SAT participation rate.

<img src="../Project-1/Images/participation_2017.png">

A few changes in SAT participation that are worth noting: DC had 100% participation on the SAT in 2017 but saw a decline in 2018; Idaho converted its 95% participation on the SAT in 2017 to 100% in 2018.

Changes in ACT participation of note: 17 states had 100% participation on the ACT in 2017 and 2018. Minnesota and Colorado saw a decline in ACT participation in 2018 (down from 100% participation.) Ohio and Nebraska adopted 100% ACT testing in 2018.

**Average Test Scores**

The data shows no major changes in how well states performed on either test from year to year - states that performed well on one test in 2017 tended to also perform well on that test in 2018.  

The data also appears to show an inverse correlation between participation rates and average scores. For both the SAT and ACT, higher rates of participation on either test statewide seem to bring down the overall statewide average score on that test.

<img src="../Project-1/Images/sat_scores_part.png">
<img src="../Project-1/Images/act_scores_part.png">

**

### Conclusions
While we only have data on statewide average participation rates and scores for two years, there are some interesting relationships that could be explored further and may help explain the disparity in participation rates on the ACT and SAT.  

#### 1. Statewide adoption of college readiness assessments
It's not likely 100% participation is happening organically based purely on student choice, so we can anticipate decisions to adopt mandatory testing (for one test over another) are being made by state departments of education. 17 states selected the ACT to be their default test in 2017 and 2018; only 4 states selected the SAT for 100% testing either year. As of 2018, 21 states have adopted 100% statewide testing for one of the two tests (and another 7 are close with >95% participation on one of the two tests.) This suggests there may be an opportunity for the College Board to lobby states without 100% adoption of the ACT (yet) who may be looking to move to mandatory testing in the future.

#### 2. Historical preferences for one test over another
Looking at the states that moved toward requiring the ACT in 2018, it looks like they had a preference for  the ACT in 2017 (> 50% participation). This is also true for the one state that moved to 100% SAT participation in 2018 (Idaho). It's possible that an existing student preference for one test pushed these states to adopt the test for their mandatory state testing, although this is difficult to determine without more years' data to compare.

#### 3. Inverse relationship between participation rates and average state scores
For the SAT in 2017 and 2018, higher participation rates on the test correlated with lower state average scores. This makes sense considering what's happening when a state requires testing: students forced to take the test may be less prepared or may not take the test as seriously as the subset of students who elect to take the test (which includes picking their own date for taking the test and paying for each time they take the test.) It makes sense that students forced to take the test would bring down the overall average. 

#### 4. Preserving national rankings 
Knowing what we know about the relationship between participation rates and test scores, we can anticipate this potential impact on statewide averages may have had an impact on state decision-making on whether to roll out state-wide testing, and which test to select. Looking at how these states ranked against one another in 2017 for both the SAT and ACT, the 17 states that chose the ACT as their default test in 2017 and 2018 actually had much better scores on the SAT. In fact, these states make up the highest performers on the SAT in both 2017 and 2018. These states also scored poorly on average on the ACT (in the bottom 35 states). What we can't tell from the data we have is whether national rankings drove decision-making on participation, or if higher participation rates drove down statewide averages and national rankings. Perhaps if we were to examine the data farther back before 100% participation on either test, we would be able to analyze if rankings had an impact on decision-making.

**2018 SAT Performance, States Ranked Best (Left) to Worst (Right)**

_States in yellow had 100% ACT Participation_
<img src="../Project-1/Images/2018_sat_ranks_100_act.png">

**2018 ACT Performance, States Ranked Best (Left) to Worst (Right)**

_States in yellow had 100% ACT Participation_
<img src="../Project-1/Images/2018_act_ranks_100_act.png">

**2018 SAT Performance, States Ranked Best (Left) to Worst (Right)**

_States in orange had 100% SAT Participation_
<img src="../Project-1/Images/2018_sat_ranks_100_sat.png">

**2018 ACT Performance, States Ranked Best (Left) to Worst (Right)**

_States in orange had 100% SAT Participation_
<img src="../Project-1/Images/2018_act_ranks_100_sat.png">


### Recommendations to the College Board
The College Board should focus its efforts on trying to recruit states don't yet have 100% participation on either test to consider the SAT (especially considering the possibility of more states adopting mandatory testing.) There are XX states that already demonstrate a preference for the SAT but have not yet adopted one test for 'default' mandatory statewide testing. The College Board may also consider approaching states that score well on the ACT (and more poorly on the SAT) to adopt the SAT for their statewide tests, and can attempt to argue that these states would have a better chance of preserving their ACT rankings by adopting the SAT. 

An example of a state that fits this profile is California, which had 60% participation on the SAT in 2018 compared to 27% ACT participation. California also performs better on the ACT (ranked 16th nationwide in 2018) than the SAT (ranked 35th nationwide in 2018), so adopting the SAT as their default test shouldn't hurt their ACT ranking. Furthermore, California is on the cusp of adopting the SAT/ACT for mandatory college readiness assessments: Assembly Bill 1951 proposed replacing current mandatory 11th grade assessments with either the SAT or ACT (while the bill was vetoed in 2018, it is likely to be considered again in 2019.) California also has a large student population, so winning over CA as a 100% SAT state would be a significant boost to overal SAT participation. 

### Next steps
A deeper analysis of SAT and ACT participation trends could include more historical data (pre-dating 2017) and more granular data on each state (perhaps at the district level). State averages don't take into account the differences in population size across the states, which would be an important consideration when the College Board is assessing ROI for investing in strategies to grow participation. Participation rates may also be affected by outside factors such as cost (ex. the ACT outbidding the SAT) or the rise of more convenient digital ACT testing, which is not captured in this data.
