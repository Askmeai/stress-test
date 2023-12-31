# stress-test
A collection of stress tests of Askme AI

ASKMEAI STRESS TEST RESULTS

1. Test Date and Time:
   - Date: 27 SEPT 2023 09:00 UTC - 02 OCT 2023 09:00 UTC
   - Time: Total 96 Hours (Non-Stop)

2. Tested Model:
   - Model Name: ASKMEAI 
   - Model Version: 1.3993

3. Test Parameters:
Priority "Accessing the queried projects, collecting data, analyzing data naming, establishing relationships, and generating a meaningful score."
    - Parameter 1: Processor
    - Parameter 2: RAM - Memory Usage
    - Parameter 3: Power Outage  
    - Parameter 4: Attack
   
4. Results:
238 projects were queried. 
The longest process took 2 minutes and 2 seconds, while the shortest took 48 seconds. 
Long-duration transactions occurred in cases where project links were not properly provided.
Out of the 238 project queries, 
18 resulted in errors, 
1 of them is done-done(Double verified, error)
The remaining 219 were completed successfully, and points were generated. 
As shown in the following section, 16 out of the 18 incorrect queries were not project names or links.
   - Metric 1: Sufficient. It peaked at 100% usage once throughout the entire test.
   - Metric 2: Sufficient . There were no memory usage problems throughout the test.
   - Metric 3: The power outage could not be tested, but the server was restarted during the query. The query process was lost and a new query was required.
   - Metric 4: There are no results.

You can access information and results of all questioned projects from this link.
https://github.com/Askmeai/stress-test/blob/main/RequestResult.htm


All error conclusions share a common issue: incorrect entry of project names and links by the end user. Measures will be taken to address this in the new version.Click to view errors
https://github.com/Askmeai/stress-test/blob/main/Errorscreen.png



Metric 1

CPU Test Results (96 Hours)

https://github.com/Askmeai/stress-test/blob/main/Error.png
Test Details:
- Test Method: 
User access and queries
Prime95 not applied

Observations:
- The CPU was tested continuously for 96 hours without any failures.
- CPU usage reached 100% twice during the test, indicating its ability to handle heavy workloads.
- The CPU remained stable and did not experience overheating issues.
-It was discovered that a query was causing the high CPU usage. This query was made for the same project twice in a row, and they were found to have been launched within the same time frame. When two different users initiated a query for the same project simultaneously, it resulted in the absence of results.

Recommendations:
- Based on the test results, the CPU has demonstrated reliability and the ability to handle intensive workloads.
- Continue monitoring system performance regularly to ensure long-term stability.
-This situation, along with related log records, has been examined, and this issue will be completely resolved in version 1.4. If the same project that AskMeAI is querying is queried again, it will hold one of these queries and display the result of the first user's query to both users.


Metric 2:

RAM Test Results (96 Hours)

The 70 percent level was steadfastly maintained throughout the entire test.
https://github.com/Askmeai/stress-test/blob/main/MemoryUsage.png

Observations:
- The RAM was tested continuously for 96 hours without any failures.
- All memory addresses were successfully read and written multiple times without errors.
- The RAM appears to be stable and reliable under prolonged usage.

Recommendations:
- Based on the test results, the RAM is in good working condition and no immediate issues were detected.
- Continue monitoring system performance regularly to catch any potential future RAM issues.


5. Comments and Evaluation:
    - Interpretation of Results: Although it was made publicly available for the first time and many project queries were made, it worked very well and produced thousands of useful log records for us.
For example, during his research with the Linkedin presence, we clearly saw a problem he was experiencing and were able to intervene immediately.
By examining these valuable logs and access records, we will be able to prepare the V1.4 model very well.
It did not embarrass us, so the people who made inquiries witnessed how reliably the project works. They learned risk scores.

    - Model Performance: 96%

6. Recommendations and Improvements:

    - Improvement Suggestions: Some adjustments and renovations are needed. These arise especially due to the difficulties of interworking many models. It doesn't work only text-based. Askmeai uses the text mining model, not text-based querying. LAMDA for text model processing Beautiful Soup and Scrapy for Web Scraping and Data Extraction. Data Storage, Sharing Filemaker Data Indexing Solr and has a specific class developed using YOLO. For these reasons, sections prepared in both PHP and Python are called separately.

    - Key Points to Consider:
Thanks to the log records obtained, it will be possible to clearly identify the time periods during which delays occurred. Discussing new models to enable the program to work modularly may also be considered.

    ASKMEAI
    - Contact Information: admin@askmeaiproject.com
