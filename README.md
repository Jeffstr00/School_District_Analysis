# PyCitySchools with Pandas

## School District Analysis Overview

We were initially tasked with assisting Maria, a school district's chief data scientist, with analyzing data on the district's funding and standardized test scores so that future decisions could be made.  To do so, we were provided with a file containing name and ID number, gender, grade number, school, and both math and reading standardized test scores for the almost 40,000 students in the district.  Analyzing this data and showing how different schools perform, and how this performance may be tied to funding, would allow the school board to make informed and hopefully good decisions going forward.  Such decisions could include how to allocate funding, whether or not certain schools need special attention, if any successful schools should be used as examples, etc.

However, it later became apparent that some of the data used in the analysis seems to have been fraudulant.  It seems as if both math and reading grades for Thomas High School 9th graders had been altered.  It is currently unknown exactly what had been changed, so we don't have new, correct data that we can simply enter in and run again.  As a result, since we couldn't submit analysis based on fraudulant data (imagine if we pointed to Thomas High 9th grade as the shining beacon that every other school in the district should emulate!), the best course of action was to simply remove the scores from the data so that it wouldn't be affected by possible fraud.  The students were still kept in the analysis for purposes of looking at funding, but their potentially fraudulent scores wouldn't impact the overall analysis.

## Results

![District Summary New](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_211.png)
![District Summary Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_212.png)
* How is the district summary affected?
* 461

* How is the school summary affected?

* How does replacing the ninth grader's math and reading scores affect Thomas High School's performance relative to the other schools?

* How does replacing the ninth-grade scores affect the following: math and reading scores by grade.

* ^^ scores by school spending

* ^^ scores by school size

* ^^ scores by school type

## Summary Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
