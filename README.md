# Artifact Package of "IoT Bugs and Development Challenges" Paper (ICSE 2021)

Paper pre-print: http://ece.ubc.ca/~amesbah/resources/papers/iot-icse21.pdf 

This repository includes all the collected and analyzed data for this study.


## Subject Repositories
In the **IoT-repositories directory**, all the data related to the subject IoT projects and the selection process details can be found.

### Selection Process Details (P1, P2, P3)
As the papers notes, IoT repositories are filtered in different phases to get the final set of subject repositories. **phase1, phase2, and phase3 directories** contain the resulting repositories in each phase. In these directories, IoT repositories are classified based on the topic they are obtained from.  For instance, **P2_iotdevice** means the second filtering phase of the repositories that are obtained from the *iot-device* topic in Github. Similarly, this structure is available for all phases (P1, P2, P3) and all the subject topics mentioned in the paper (IoT, Internet-of-Things, IoT-application, IoT-platform, IoT-device).

### Final Selected Repositories
In the root of the IoT-repositories directory, a CSV file **final_subject_repositories.csv** can be found that contains the details of the final selected repositories in tabular format. 

## Bug Categories
In the **bug-categorization** directory, there are two main files.
 - **5565-collected_bugs.json** is a JSON file that contains all the collected bug reports from the subject repositories. This file includes the URL, title, body, and date of each bug report. This collection can be used as a pool of representative bug reports as all the bug instances are valid flagged GitHub issues and are collected from representative IoT repositories.
 - **323-analyzed_bugs.json** is a JSON file that contains a subset of all collected bug reports which are analyzed and categorized. In this file, in addition to the URL and identifiers of each bug report, the details of our categorization process are also available. In our Root Cause Analysis process (RCA) using the Five-whys technique, we kept track of “what bugs are the consequences of a given bug”. After extracting the bug categories by open coding, we replaced bugs with their category. This data is available in this file with the format [ bugCat1/bugCat2/bugCat3/… ] for each bug report which shows a causation relationship from left to right. The most important root cause of the bug (named with the convention in the paper) and the location of the most relevant fault leading to the bug are also recorded.

## User Studies
For keeping the qualitative data brief, we used their associated tags to present them. To find the meaning of each tag we refer you to the Tag Guide files described below: 
### Tag Guide Files
There are two files in the root directory that are intended to connect the tags with their name in the paper.
- TagGuide_BugCategories.pdf: Contains the tags of each node in the taxonomy
- tagGuide_challenges.pdf: This contains the tags of each developer challenge in the paper.
## Interviews
In the **interviews directory**, there are two files:
- Interview_Questions.pdf: This PDF file contains the questions asked in the interviews.
- Interview_coding.csv: This CSV file includes the bug categories and developer challenges that each interviewee mentioned in the interviews. Each row contains the associated tags for each distinct meaningful unit of information that the interviewee discussed. The interviewee IDs are the same as the table 1 in the paper.

## Survey
In the **survey directory**, there are two files:
- survey.pdf: This is a PDF version of the online survey distributed to IoT developers.
- Survey_Valid_responses.csv : This CSV file includes all the raw collected data from the survey. The incomplete and invalid responses have been removed.

**Note**: All the publicly available data from participants are anonymous.

## Authors
Amir Makhshari: [Linkedin](https://www.linkedin.com/in/amirosein/), [Twitter](https://twitter.com/makhshari)

[Ali Mesbah](http://ece.ubc.ca/~amesbah/): [Linkedin](https://www.linkedin.com/in/ali-mesbah-4646102/), [Twitter](https://twitter.com/amesbah)


IoT Research at [Salt Lab](http://salt.ece.ubc.ca/)


