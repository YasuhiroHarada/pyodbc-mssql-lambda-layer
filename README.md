# pyodbc-mssql-lambda-layer with glibc-gconv-extra

AWS Lambda runtimes for Python 3.12 and later are based on Amazon Linux 2023, which does not include glibc-gconv-extra, causing “Unicode conversion failed (22) (SQLGetData)” errors. This Lambda layer resolves this issue.

> [!IMPORTANT]
> Remember to set the Lambda environment variable GCONV_PATH=/opt/lib/gconv

If you only need glibc-gconv-extra lambda layer, see 
https://github.com/YasuhiroHarada/glibc-gconv-extra-lambda-layer
