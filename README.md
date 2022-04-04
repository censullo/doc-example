# Connect Amazon DynamoDB and Google Sheets using CData Connect Cloud
In this post, I demonstrate how to connect Google Sheets with an Amazon DynamoDB table using CData Connect Cloud.

## Prerequisites
To complete the walkthrough, you must have the following.

. Google account.
. CData account. If you don't have one, a free trial is available at https://cloud.cdata.com.
. AWS account with a DynamoDB table.

## Step 1: Create an Amazon DynamoDB connection
* Sign in to your CData Connect Cloud account at https://cloud.cdata.com/.
* On the navigation pane, choose **Connections**.
* Choose **Add Connection**.
* On the **Add Connection** dialog, choose **Amazon DynamoDB**.
* (Optional) On the **Add Amazon DynamoDB Connection** page, edit the **Connection Name** of keep the default.
* Enter the **AWS Access Key** and **AWS Secret Key** for the AWS Identity and Access Management (IAM) user. For more information, refer to https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html[Understanding and getting your AWS credentials]. 
* Enter the **User** and **Password** of the IAM user.
* Choose **Create & Test**. If successful, CData Connect Cloud returns `Connection Saved Successfully!`. Choose **OK**.

## Step 2: Install the CData Cloud add-on for Google Sheets
* On the CData Connect Cloud navigation pane, choose **Clients**.
* On the **Clients** page, under **BI and Reporting Tools**, choose **Google Sheets**.
* On the **CData Connect Cloud** page in Google Workspace Marketplace, choose **Install**.
* Choose **Continue**.
* Choose a Google account to connect to CData Cloud.
* Choose **Allow**.
* Choose **Done**.

## Step 3: Test the connection
* In Google Sheets, choose **Extensions**, **CData Connect Cloud**, **Open**.
* Choose **Authorize**.
* On the **Authorize App** page, choose **Accept**. If successful, Google returns `Success!`. You can close this tab.
* In Google Sheets, choose **Import**.
* For **Choose a Connection**, choose the name of your Amazon DynamoDB connection.
* For **Choose a Table**, choose a DynamoDB table.
* Choose **Execute**.
* For Query Output, choose **Current**. If successful, CData Connect Cloud returns `Query Succeeded!`.
