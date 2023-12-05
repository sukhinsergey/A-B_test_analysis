# A-B_test_analysis
During testing, a new payment mechanism for services on the website was proposed to the target group, while the control group retained the basic mechanism. It is necessary to analyze the results of the experiment and draw a conclusion on whether to launch the new payment mechanism for all users.

roups.csv: a file containing information about user affiliation to the control or experimental group (A – control, B – target group).
groups_add.csv: an additional file with users that was sent to you 2 days after the data transfer.
active_studs.csv: a file with information about users who accessed the platform on the days of the experiment.
checks.csv: a file with information about user payments on the days of the experiment.


1) Define the metrics to be used for analysis, 
2) Statistically test differences between groups A/B, 
3) Make a decision on whether to launch the new mechanism, 
4) Optimize the query for automating the processing of the groups_add.csv file to calculate metrics
5) Integrate SQL request inside python query for calculation of ARPU,ARPAU, CR
