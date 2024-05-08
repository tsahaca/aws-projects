# Alert Notifications for Long Running EMR Jobs

Many Organizations run big data ETL Jobs using open source tool Apache Spark in Amazon EMR. 
To monitor the job progress, it is essential to get alert notifications if the job is running longer than expected, failed due to some error condition. 

# Solution Overview

Out of the box EMR does not generate any such alert notifications. In this blog post we will show you how to create such alert notifications using event driven architecture. We will use the following AWS Services 
1. EventBridge
2. Stepfunction
3. Lambda 
4. SNS
