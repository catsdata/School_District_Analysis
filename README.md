# School District Analysis

## Overview:

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

## Results: 


-   ### **District Summary**

    Removal of Thomas High School 9th Grade scores made minor impact to the overall district summary; Dropping %Passing Math by 0.2%, Reading by 0.3% and Overall by 0.1%.

     *before*
     
     ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/district_mod.PNG)
     
     *after*
     
     ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/district_chal.PNG)

-   ### **School Summary**
    
    The only impact to the High Performers DataFrame is with Thomas High School, but not enough to bump it from its second place spot.  Again, impact was only within tenths or hundredths of percentages.  Since the only changes made were to Thomas High School; Low Performing schools remain unchanged.
    
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

    As seen below, in an expanded list of all schools, the only changes were reflected on Thomas High School's percentages.

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/schoolsummary_mod.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/schoolsummary_chal.PNG)
    
-   ### **Math and reading scores by grade**
    
    Below are the average scores by grade of each school; showing the NaN replacement for Thomas High School 9th grade.
    
    **Math Scores by grade**
    
     *before* ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/mathbygrade_mod.PNG) *after* ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/mathbygrade_chal.PNG)

    **Reading Scores by grade**
    
     *before* ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/readingbygrade_mod.PNG) *after* ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/readingbygrade_chal.PNG)

-   ### **Scores by school spending**

    The Thomas High School changes appear to have not changed the averages within spending ranges of schools.

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbyspend_mod1.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbyspend_chal1.PNG)
    
    However, if you expand the percentages, we again see the neglible tenths and hundredths decimal adjustments in the $630-$644 range where Thomas High School fits under.  
    
     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbyspend_mod2.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbyspend_chal2.PNG)
    
-   ### **Scores by school size**

    Same situation as the spending dataframes, it appears there was no change.

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbysize_mod1.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbysize_chal1.PNG)
    
    But the expanded formatting again shows the minor adjustments to the Medium size schools that Thomas High is apart of.
    
     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbysize_mod2.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbysize_chal2.PNG)

-   ### **Scores by school type**

    And last, changes appear not to make an impact to summaries by school type - Charter vs. District.

     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbytype_mod1.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbytype_chal1.PNG)
    
    Thomas High School is a Charter School, therefore when we expand the formatting we see the minor change impacts.
    
     *before*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbytype_mod2.PNG)
    
     *after*
     
    ![This is an image](https://github.com/catsdata/School_District_Analysis/blob/main/Resources/scoresbytype_chal2.PNG)

## Summary: 

In Summary, removing the 9th grade Thomas High School grades made insignificant changes and we can assume that the grades were not fraudulent.  Changes to the District Summary, School Spending, School Size, and School Type all reflect the neglible changes we see to Thomas High School directly.  It is my recommendation that the original reports, including the 9th grade Thomas High School data, are used for reporting detail to the school board.

Code can be accessed [HERE](https://github.com/catsdata/School_District_Analysis/blob/main/PyCitySchools.ipynb) for the original, and [HERE](https://github.com/catsdata/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb) for the adjustment for Thomas High School.
