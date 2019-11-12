# S3 Multipart Upload

## Moving Data into S3
* 3 options to uploading data
    * Console (not-recommended for large files)
    * CLI
    * SDKs
* ### Transfer Acceleration
    * Instead of uploading directly to an S3, the service uploadsa it to a CloudFront edge location and THEN an S3 bucket using AWS Network

## Mass Data Importing
* ### Snowball
    * __Petabyte__
    * Tamper-proof data transport
    * It's essentially a big suitcase
    * *Note: That this is a decent option for database migrations, because this is delivered with a DML-tool*
* ### Snowmobile
    * __Exabyte__
    * A truck that arrives with an armed escort