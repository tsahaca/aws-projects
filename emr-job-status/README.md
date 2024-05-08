# Alert Notifications for Long Running EMR Jobs

Many Organizations run big data ETL Jobs using open source tool Apache Spark in Amazon EMR. 
ETL Jobs may run from few minutes to few hours, so it is very important to know the status of the job and get alert notifications if the job is running longer than expected or failed due to some error condition. 

# Solution Overview

Out of the box EMR does not generate any such alert notifications. In this blog post we will show you how to create such alert notifications using event driven architecture. We will use the following AWS Services 
1. EventBridge
2. Stepfunction
3. Lambda 
4. SNS

![Architecture Diagram](images/emr-job-status.png)