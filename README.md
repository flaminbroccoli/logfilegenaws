# LogFileGenAWS


This a fork of the original [LogFileGenerator repo](https://github.com/0x1DOCD00D/CS441_Fall2022/tree/main/LogFileGenerator) project and provides a REST
 with functionality added to store the resultant logs to AWS S3.


## Summary of changes
1. logback_test.xml: Added -mm to filePatter nto generate logs by the minute
2. application.conf: Added info to store S3 bucket name and region. Credentials
will be taken from local machine.
3. GenerateLogData.scala: Built a Transfer manager and uploaded the files upon
completion of generation.
