# school_district_analysis_UT_data

## Project Overview
The school board has notified Maria and her supervisor that the [students complete (csv)](resources/students_complete.csv) file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to us for help. We are to replace the math and reading scores for Thomas High School with 'NaNs' while keeping the rest of the data intact. Once we’ve replaced the math and reading scores, we will repeat the school district analysis, and write up a report to describe how these changes affected the overall analysis, if at all.

## Resources
- Data Source: [students complete (csv)](resources/students_complete.csv)
- Software:
   - Python 3.7.6
   - Jupyter Notebook 6.3.0

## Results
#### How is the district summary affected?
   - After the removal of the data points in question, the district summary changed very minorly, with the passing rates of math scores and the overall passing rates each falling by 1/10th of a point. This is no believed to be a statistically significant change.
   - [District Summary (png)](analysis/district_summary.png)
#### How is the school summary affected?
   - [School Summary (png)](analysis/school_summary.png)
   - After the removal of the data points in question, there are significant changes to Thomas High School's average scores and passing rates. Note the above photo compared to the below "corrupted" data results of Thomas High School.
#### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
   - [Corrupted Thomas Summary (png)](analysis/thomas_corrupted_data_summary.png)
   - After the removal of the data points in question, Thomas High School was placed into the top five performing schools within the district.
#### How does replacing the ninth-grade scores affect the following:
   - Math and reading scores by grade
      - After the removal of the data points in question, the only change was that of the lack of data now present for Thomas High School ninth graders, no other changes were detected.
   - Scores by school spending
      - [Spending Summary (png)](analysis/score_spending_results.png)
      - After the removal of the data points in question, in respect to the affect of spending per student on passing score rates, no change was detected.
   - Scores by school size
      - [Score Summary (png)](analysis/score_size_results.png)
      - After the removal of the data points in question, in respect to the affect of school size on passing score rates, no change was detected.
   - Scores by school type
      - [Type Summary (png)](analysis/score_type_results.png)
      - After the removal of the data points in question, in respect to the affect of school type on passing score rates, no change was detected.

## Summary
The only significant change after removing the suspected foul data points were results directly with Thomas High School (listed below), no change was noticed on a district level due to these changes.
   - Average math passing rate for Thomas High School rose from 66.91% to 93.19%
   - Average reading passing rate for Thomas High School rose from 69.66% to 97.02%
   - Average overall passing rate for Thomas High School rose from 65.08% to 90.63%
   - Thomas High School moved up to one of the highest performing schools in the district (by these two passing metrics).
   
   