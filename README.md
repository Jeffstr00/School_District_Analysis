# PyCitySchools with Pandas

## School District Analysis Overview

We were initially tasked with assisting Maria, a school district's chief data scientist, with analyzing data on the district's funding and standardized test scores so that future decisions could be made.  To do so, we were provided with a file containing name and ID number, gender, grade number, school, and both math and reading standardized test scores for the almost 40,000 students in the district.  Analyzing this data and showing how different schools perform, and how this performance may be tied to funding, would allow the school board to make informed and hopefully good decisions going forward.  Such decisions could include how to allocate funding, whether or not certain schools need special attention, if any successful schools should be used as examples, etc.

However, it later became apparent that some of the data used in the analysis seems to have been fraudulant.  It seems as if both math and reading grades for Thomas High School 9th graders had been altered.  It is currently unknown exactly what had been changed, so we don't have new, correct data that we can simply enter in and run again.  As a result, since we couldn't submit analysis based on fraudulant data (imagine if we pointed to Thomas High 9th grade as the shining beacon that every other school in the district should emulate!), the best course of action was to simply remove the scores from the data so that it wouldn't be affected by possible fraud.  The students were still kept in the analysis for purposes of looking at funding, but their potentially fraudulent scores wouldn't impact the overall analysis.

(Note: images of the updated data with Thomas High School 9th grade scores removed are displayed first with the original data being shown second for comparison.)

## Results

* ### District Summary
![District Summary New](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_211.png)
![District Summary Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_212.png)

The overall effect on the district summary was miniscule.  That makes sense, as only 461 datapoints were removed from a population of almost 40,000, so even extreme cheating would struggle to really move the needle much versus the other 99% of unchanged data.  In fact, unformatted data had to be shown in order to notice a difference (otherwise, results were the same to second decimal point).  However, slight decreases in both math and reading scores could be observed when you look close enough, which does make sense if the removed scores were unnaturally high due to fraud.

* ### School Summary
![School Summary New](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_221.png)
![School Summary Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_222.png)

For school summary, data only changed for Thomas High School students, so obviously other schools weren't affected.  However, Thomas High School predictably had their numbers suffer once the fraudulent data was removed (though not by tremendous amounts).  Math passing percentage fell from 93.27 to 93.19 and reading went from 97.31 to 97.02, for an overall drop of 90.95 to 90.63.

* ### Performance vs. Other Schools
![School Performance New](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_231.png)
![School Performance Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_232.png)

While Thomas High School's numbers took a hit after their fraudulent scores were removed, it didn't result in a huge difference when compared to other schools.  In fact, they are the #2 school either with or without the changes.  However, they definitely lost some position in the race.  While their original 90.95 passing percent was a relatively safe 0.35 points ahead of Griffin and only 0.38 away from the overall lead, their #2 spot after the change isn't as secure.  With the updated data, they are now 0.7 points away from first place, and are only 0.03 points away from falling into third.

* ### Scores by Grade
![Grade Scores Math New](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_241math.png)
![Grade Scores Math Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_242math.png)

Since the only data that changed was from 9th grade students at Thomas High School, grades 10-12 were not affected.  However, 9th grade saw its second highest math scoring school removed, relatively improving the performances of the other schools as a result.

![Grade Scores Reading Now](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_241reading.png)
![Grade Scores Reading Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_242reading.png)

While Thomas High School's reading scores weren't as relatively impressive as their math scores, they still scored in the upper third of 9th grade schools.  As a result, again, removing their scores from the data would make the other schools look better in comparison.

* ### Scores by School Spending
![School Spending New](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_251.png)
![School Spending Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_252.png)

With a $638 per student budget, Thomas High School's changes would only be reflected in the $630-644 bracket.  However, the changes were so slight that they cannot even be noticed to the second decimal place.  However, by looking at raw numbers, it can be seen that performance slightly drops across the board for schools in this range.

* ### Scores by School Size
![School Size New](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_261.png)
![School Size Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_261.png)

With 1,635 students, Thomas High School's numbers being changed would only impact medium-sized schools with 1000-2000 students.  While the changes aren't even noticeable in the displayed charts, numbers did slightly change.  With the scores removed, math passing percentage fell from 93.60 to 93.58 and reading went from 96.79 to 96.73, with a corresponding dip in overall passing percentage of 90.62 down to 90.56.

* ### Scores by School Type
![School Type New](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_271.png)
![School Type Old](https://github.com/Jeffstr00/School_District_Analysis/blob/main/Resources/schools_271.png)

## Summary Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
