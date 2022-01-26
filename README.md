# School District Analysis

## School District Analysis Overview:

We have been provided data in regards to recent school and student performance on math and reading.  The School District has asked Maria and myself to analyze the data for the following detail:

- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school, presented in a table format
- Tables presenting each of the following metrics:

    - Top 5 and bottom 5 performing schools, based on the overall passing rate
    - The average math score received by students in each grade level at each school
    - The average reading score received by students in each grade level at each school
    - School performance based on the budget per student
    - School performance based on the school size 
    - School performance based on the type of school

Before presenting the data, we were asked to rerun reports removing the 9th Grade data of Thomas High School as academic dishonesty was under investigation.  The below results show the data analysis before and after the removal of that data and its impacts.

## Resources

- Data Sources: [schools_complete.csv](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/schools_complete.csv) & [students_complete.csv](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/students_complete.csv)
- Software: 
    - Python 3.7.11
        - Dependencies: Pandas 1.3.5 & Numpy 1.20.3  
    - Anaconda Command line Client 1.9.0
    - Conda 4.11.0
    - Jupyter Notebook 6.4.6

## Results: 


-   ### **District Summary**

    Removing the 9th Grade Thomas High School scores made minor impact to the overall district summary.  Percent Passing Math dropped by 0.2%, Reading dropped by 0.3% and Overall dropped by 0.1%.  However, all of those are decreases nonetheless indicating the Thomas High School 9th grade scores may have had a positive or skewed impact to the overalls.

     *before*
     
     ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/district_mod.PNG)
     
     *after*
     
     ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/district_chal.PNG)

-   ### **School Summary**
    
    The only impact to the High Performers DataFrame is with Thomas High School, but not enough to bump it from its second place spot.  Average Math scores decreased by .06 and Average Reading increased by .05.  However all of the Percent Passing's decreased within tenths of percentages as they did in the District report: Math dropped by 0.1%, Reading dropped by 0.3% and Overall dropped by 0.3%   Since the only performance changes made were to Thomas High School; Low Performing schools remain unchanged.
    
    **High performers**
    
     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/highperform_mod.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/highperform_chal.PNG)
    
    **Low performers**

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/lowperform_mod.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/lowperform_chal.PNG)

-   ### **Thomas High School performance changes**

    As seen below, in an expanded list of all schools, the only changes were reflected on Thomas High School's stats.  Both reports do show the total number of students as 1635, however the calculations on the grade averages and percentages were made using just the 10th, 11th, and 12th grade for a total of 1174 students.

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/schoolsummary_mod.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/schoolsummary_chal.PNG)
    
-   ### **Math and reading scores by grade**
    
    Below are the average scores by grade of each school; showing the NaN replacement for *only* Thomas High School 9th grade.
    
    **Math Scores by grade**
    
     *before* ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/mathbygrade_mod.PNG) *after* ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/mathbygrade_chal.PNG)

    **Reading Scores by grade**
    
     *before* ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/readingbygrade_mod.PNG) *after* ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/readingbygrade_chal.PNG)

-   ### **Scores by school spending**

    Upon initial look, the Thomas High School changes appear to have not changed the averages within spending ranges of schools.

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbyspend_mod1.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbyspend_chal1.PNG)
    
    HOWEVER, if you expand the percentages, we again see the neglible decimal adjustments in the $630-$644 range where Thomas High School falls under.  Average Math scores decreased by .01 and Average Reading increased by .01.  However all of the Percent Passing's decreased within hundreths of percentages: Math dropped by 0.02%, Reading dropped by 0.08% and Overall dropped by 0.07%
    
     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbyspend_mod2.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbyspend_chal2.PNG)
    
-   ### **Scores by school size**

    Just as the school spending dataframes, it first appears that there was no change to the school size scores.

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbysize_mod1.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbysize_chal1.PNG)
    
    HOWEVER, again the expanded formatting shows the minor adjustments to the Medium size schools that Thomas High is apart of.  Average Math scores decreased by .01 and Average Reading increased by .01.  However all of the Percent Passing's decreased within hundreths of percentages: Math dropped by 0.01%, Reading dropped by 0.06% and Overall dropped by 0.07%
    
     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbysize_mod2.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbysize_chal2.PNG)

-   ### **Scores by school type**

    And last, just as size and spending, changes appear not to make an impact to summaries by school type - Charter vs. District.

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbytype_mod1.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbytype_chal1.PNG)
    
    HOWEVER, Thomas High School is a Charter School, therefore when we expand the formatting we see the minor change impacts.  Average Math scores decreased by .01 and Average Reading increased by .01.  However all of the Percent Passing's decreased within hundreths of percentages: Math dropped by 0.01%, Reading dropped by 0.03% and Overall dropped by 0.04%
    
     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbytype_mod2.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbytype_chal2.PNG)

## Summary: 

In Summary, removing the 9th grade Thomas High School grades made very minor changes, within tenths and hundredths; however it is a consistent decrease in those numbers.  Changes to the District Summary, School Spending, School Size, and School Type all reflect the neglible changes we see to Thomas High School directly.  Average reading scores showed a slight improvement, but overall percentages decreased.  If the there was indeed dishonesty in the 9th grade scores, the impact wasn't big enough to skew for any major changes.

![changes](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/changes.PNG)

Code  from this analysis can be accessed [HERE](https://github.com/catsdata/School_District_Analysis/blob/main/PyCitySchools.ipynb) for the original, and [HERE](https://github.com/catsdata/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb) for the adjustment for Thomas High School.
