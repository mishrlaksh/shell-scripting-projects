# AWS S3 Event Triggering




**NOTE**: REPLACE YOUR AWS ACCOUNT ID IN THE LAMBDA FUNCTION CODE. & INSTALL jq. BEFORE EXECUTING PROJECT

AWS S3 Event triggering is a very popular project used by top companies in the Industry.

Here are some examples of top companies that use S3 event triggering:

**Netflix**: Netflix use S3 event triggering to automatically process video files uploaded to Amazon S3, enabling seamless content ingestion and processing.

**Airbnb**: This lodging and homestays aggregator use S3 event triggering to automatically process and analyze data stored in Amazon S3, such as guest reviews and booking information.

**Expedia**: They use S3 event triggering to automatically process and analyze data stored in Amazon S3, such as travel bookings, user profiles, and pricing information, to power their personalized travel recommendations and search features.

---

## Install and Configure AWS CLI

1. **Install the AWS CLI** – After installation, configure the CLI by logging into your AWS account.
   - Go to **Security Credentials** in your AWS account and create an **AWS Access Key ID** and **AWS Secret Access Key**.
   - Run the following command to configure the AWS CLI:

     ```bash
     aws configure
     ```

   - Enter the **AWS Key ID**, **AWS Secret Key**, your **default region**, and your **output format** when prompted.

## Project Execution

### Step 1: Clone the GitHub Repository

Clone the repository named `shell scripting projects` from the GitHub namespace provided in the video description. This repository contains the shell script and Lambda function code required for the project.

### Step 2: Update the Shell Script

- **Modify the Email Address** – Open the script and replace the placeholder email address with your own.
- **Parameterize the Script (Optional)** – If desired, parameterize the shell script by passing command-line arguments for additional flexibility.

### Step 3: Execute the Shell Script

Run the shell script using the following command:

```bash
./<script_name>.sh
```

This script will create the following resources in your AWS account:

- **S3 Bucket** – Used to store files uploaded for processing.
- **Lambda Function** – Triggered automatically when a file is uploaded to the S3 bucket.
- **SNS Topic** – Used to send email notifications upon file upload.
- **IAM Role** – Assigned to the Lambda function, granting it necessary permissions to access the S3 bucket and invoke the SNS topic.

### Step 4: Confirm Email Subscription

After running the script, you’ll receive an email to confirm the subscription to the SNS topic. Confirm the subscription to start receiving notifications when files are uploaded to the S3 bucket.

### Step 5: Upload a File to the S3 Bucket

Upload a file to the S3 bucket created by the script. This action will trigger the Lambda function.

### Step 6: Receive Email Notification

You should receive an email notification confirming the file upload to the S3 bucket, indicating successful configuration of the automation workflow.

---


![Screenshot 2023-04-14 at 7 06 46 PM](https://user-images.githubusercontent.com/43399466/232058778-a7299e9b-9892-471c-a05d-14d773b5b333.png)
