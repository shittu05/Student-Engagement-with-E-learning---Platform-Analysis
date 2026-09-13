# Effect of cognitive load on student learning experiences and interactions with instructional materials in an online learning platofrm

### by Muhammed Shittu

This project investigates how students' digital engagement with an online learning hub relates to their self-reported cognitive load, cognitive engagement, and perceived learner control. The learning hub included video materials, concept maps, quizzes, and a survey. The analysis focuses on whether different forms of platform interaction are associated with students' intrinsic load, extraneous load, and germane load.

There are two main sections to this project:
> In the first section, I performed exploratory data analysis and data preparation using student interaction logs and survey data from an online learning hub. I cleaned and merged data from page request events, video events, quiz attempts, and survey responses to create a student-level analytical dataset. The analysis examined how students interacted with learning resources such as videos, concept maps, and quizzes.

> In the second section, I conducted inferential analyses to examine whether different engagement profiles were associated with students' cognitive load experiences. Students were grouped using meaningful behaviour-based indicators such as video interaction, concept-map use, and quiz attempts. Kruskal-Wallis tests were used because the survey construct scores were non-normally distributed.

## Dataset

The dataset includes student-level engagement records from an online learning hub. The learning hub contained video learning materials, concept maps, quizzes, and a survey measuring students' cognitive and learning experiences.

The dataset includes the following main data sources:
> 
> - Page request event log
> - Video interaction event log
> - Quiz attempt records
> - Student survey responses
> - Cleaned student-level master dataset
  
The cleaned analytical dataset includes variables such as:
> 
> - Total page visits
> - Video events count
> - Video play count
> - Video pause count
> - Video completion count
> - Concept-map visits
> - Quiz attempts
> - Quiz retries
> - Quiz sections attempted
> - Survey completion status
> - Intrinsic load
> - Extraneous load
> - Germane load
> - Cognitive engagement
> - Perceived learner control

During the data wrangling process, the raw interaction logs were cleaned, merged, and transformed into a student-level dataset. New engagement variables and grouping profiles were created to represent different forms of student interaction with the learning hub. These included video interaction profiles, concept-map use profiles, and quiz attempt profiles.

## Research Questions

This project focused on the following research questions:
>
> - What is the impact of the amount of videos watched or interacted with on intrinsic load, extraneous load, and germane load?

> - What is the impact of concept-map use on intrinsic load, extraneous load, and germane load?

> - What is the impact of quiz attempts on intrinsic load, extraneous load, and germane load?

## Analysis Approach
>
The analysis used behaviour-based groupings derived from the platform interaction data.

### Video Interaction Analysis
>
Initial analysis group video events into groups 
> - No video interaction: 0 video events
> - Video interaction: 1 or more video events

Further analysis then grouped the students based on the level of video event activity.
> - Minimal video interaction: 1-4 video events
> - High video interaction: 5 or more video events
   

Two video analyses were conducted. The first analysis compared students with no video interaction against students with any video interaction.The second analysis removed students with no video interaction and compared minimal video interaction with high video interaction. 

### Concept-Map Use Analysis
> 
Students were grouped according to their concept-map visit counts.
> - Minimal concept-map use: 1 concept-map visit
> - High concept-map use: 2 or more concept-map visits
  
Students with no concept-map visits were removed from this analysis to focus only on students who used the concept-map resource.

### Quiz Attempt Analysis
>
Students were grouped according to quiz attempt behaviour.
> - One quiz attempt: 1 recorded quiz attempt
> - Multiple quiz attempts: 2 or more recorded quiz attempts

> Students with no quiz attempts were removed from this analysis to focus only on students who engaged with the quiz activity.

## Statistical Methods

Kruskal-Wallis tests were used to compare survey construct scores across engagement groups. This non-parametric test was selected because the survey construct scores were not normally distributed.

The main survey constructs examined were:
> - Intrinsic load
> - Extraneous load
> - Germane load

Descriptive statistics were reported as:
> - Mean
> - Standard deviation
> - Group sample size


## Summary of Findings

> The video interaction analysis showed that students with minimal video interaction did not significantly differ from students with high video interaction in intrinsic load or germane load. However, the difference for extraneous load approached significance. Students with minimal video interaction reported lower extraneous load than students with high video interaction.

> The binary video analysis showed a clearer pattern. Students with no video interaction reported significantly higher intrinsic load than students with any video interaction. The difference for extraneous load approached significance, with students who had no video interaction reporting higher extraneous load than students who interacted with videos.

> The concept-map analysis showed a statistically significant difference in intrinsic load. Students with high concept-map use reported higher intrinsic load than students with minimal concept-map use. Germane load approached significance, with high concept-map users reporting higher germane load. This suggests that students who perceived the material as more difficult may have returned to concept maps more often for support.

> The quiz attempt analysis showed no statistically significant differences between students with one quiz attempt and students with multiple quiz attempts in intrinsic load, extraneous load, or germane load.

## Key Insights for Presentation

> - Students with no video interaction reported higher intrinsic load than students who interacted with videos.
> - Extraneous load was also higher among students with no video interaction.
> - Among students who interacted with videos, minimal and high video interaction groups did not significantly differ in intrinsic or germane load.
> - Concept-map use showed an important pattern: students with repeated concept-map use reported higher intrinsic load than students who accessed concept maps only once.This may suggest that concept maps were used more frequently by students who experienced the learning material as more difficult.
> - Quiz attempt frequency did not significantly differentiate intrinsic load, extraneous load, or germane load among quiz users.
> - The findings suggest that different forms of digital engagement should not be treated as equivalent. Specific resource interactions, especially video and concept-map use, provide more meaningful insight than broad click counts alone.


## Tools Used
> - Excel
> - RStudio
> - R



Files in This Project

> - R analysis script

README project summary
