# Connect Amazon DynamoDB and Google Sheets using CData Connect Cloud
In this post, I demonstrate how to connect Google Sheets with an Amazon DynamoDB table using CData Connect Cloud.

## Prerequisites
To complete the walkthrough, you must have the following.

* Google account.
* CData account. If you don't have one, a free trial is available at https://cloud.cdata.com.
* AWS account with a DynamoDB table.

## Step 1: Create an Amazon DynamoDB connection
1. Sign in to your CData Connect Cloud account at https://cloud.cdata.com/.
2. On the navigation pane, choose **Connections**.
3. Choose **Add Connection**.
4. On the **Add Connection** dialog, choose **Amazon DynamoDB**.
5. (Optional) On the **Add Amazon DynamoDB Connection** page, edit the **Connection Name** of keep the default.
6. Enter the **AWS Access Key** and **AWS Secret Key** for the AWS Identity and Access Management (IAM) user. For more information, refer to [Understanding and getting your AWS credentials](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html). 
7. Enter the **User** and **Password** of the IAM user.
8. Choose **Create & Test**. If successful, CData Connect Cloud returns `Connection Saved Successfully!`. Choose **OK**.

## Step 2: Install the CData Cloud add-on for Google Sheets
1. On the CData Connect Cloud navigation pane, choose **Clients**.
2. On the **Clients** page, under **BI and Reporting Tools**, choose **Google Sheets**.
3. On the **CData Connect Cloud** page in Google Workspace Marketplace, choose **Install**.
4. Choose **Continue**.
5. Choose a Google account to connect to CData Cloud.
6. Choose **Allow**.
7. Choose **Done**.

## Step 3: Test the connection
1. In Google Sheets, choose **Extensions**, **CData Connect Cloud**, **Open**.
2. Choose **Authorize**.
3. On the **Authorize App** page, choose **Accept**. If successful, Google returns `Success!`. You can close this tab.
4. In Google Sheets, choose **Import**.
5. For **Choose a Connection**, choose the name of your Amazon DynamoDB connection.
6. For **Choose a Table**, choose a DynamoDB table.
7. Choose **Execute**.
8. For Query Output, choose **Current**. If successful, CData Connect Cloud returns `Query Succeeded!`.
