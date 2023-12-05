### A-B_test_analysis
During testing, a new payment mechanism for services on the website was proposed to the target group, while the control group retained the basic mechanism. It is necessary to analyze the results of the experiment and draw a conclusion on whether to launch the new payment mechanism for all users.

- groups.csv: a file containing information about user affiliation to the control or experimental group (A – control, B – target group).
- groups_add.csv: an additional file with users that was sent to you 2 days after the data transfer.
- active_studs.csv: a file with information about users who accessed the platform on the days of the experiment.
- checks.csv: a file with information about user payments on the days of the experiment.


1) Define the metrics to be used for analysis, 
2) Statistically test differences between groups A/B, 
3) Make a decision on whether to launch the new mechanism, 
4) Optimize the query for automating the processing of the groups_add.csv file to calculate metrics
5) Integrate SQL request inside python query for calculation of ARPU,ARPAU, CR


### Results:
- The change in Conversion Rate (CR) is random and not statistically significant.
- The change in Average Revenue Per User (ARPU) is random and not statistically significant.
- The change in Average Revenue Per Paying User (ARPPU) is not random – there are statistically significant differences in Group B, with the test group showing a higher ARPPU.

When looking at the data for active users, the test group with the new mechanism did not show statistically significant differences in CR and ARPU. However, the average revenue per paying user was higher in Group B. Since we were creating a payment mechanism, the experiment can be considered successful.

Implementing a similar experiment across the entire platform will not lead to statistically significant results in conversion, average revenue per user, but it will increase the average revenue per paying user.
