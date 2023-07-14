# Amazon S3 File Upload

This script allows you to upload a file to an Amazon S3 bucket using the Boto3 library. You need to provide your AWS access key, secret key, the local file path, the target bucket name, and the desired file name on S3.

## Prerequisites

Before running this script, ensure that you have the following:

- Python 3.x installed on your system
- The Boto3 library installed. You can install it using the following command:
  ```
  pip install boto3
  ```

## Usage

1. Open the script and update the following variables with your own values:
   - `ACCESS_KEY`: Your AWS access key
   - `SECRET_KEY`: Your AWS secret key
   - `LOCAL_FILE`: The path to the file on your local machine that you want to upload
   - `BUCKET_NAME`: The name of the S3 bucket you want to upload the file to
   - `S3_FILE_NAME`: The desired file name for the file on S3
2. Save the script after making the necessary changes.
3. Run the script using a Python environment.
4. The script will establish a connection to the specified S3 bucket using the provided credentials.
5. The file specified by `LOCAL_FILE` will be uploaded to the S3 bucket with the name specified by `S3_FILE_NAME`.
6. If the upload is successful, the script will print "Upload Successful".
7. If there is an error, such as a file not found or missing credentials, an appropriate error message will be displayed.

## Note

- Make sure you have proper AWS credentials with the necessary permissions to upload files to the specified S3 bucket.
- Ensure that the local file path is correct and the file exists.
- The script uses the `boto3.client()` method to create an S3 client object and the `s3.upload_file()` method to upload the file.
- The script handles potential errors, such as a file not found or missing credentials, and provides informative error messages.

## License

This script is licensed under the [MIT License](LICENSE).