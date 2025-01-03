# Static website hosted on AWS S3
## Steps to Follow:
### Step 1: Set Up an S3 Bucket
1.  Log in to your AWS Management Console.<br>
2.  In the search bar, type S3 and select the S3 service.<br>
3.  Click the Create bucket button to begin the setup.<br>

![alter text](images/1.png)

    bucket Creation Completed Successfully:
4.  Provide a unique name for your bucket (e.g.,aws-mystatic-website-s3) and select a preferred region.<br>

![alter text](images/2.png)

5.  Disable the "Block all public access" option to make the website accessible publicly.<br>
6.  Acknowledge the warning by selecting the checkbox, then click "Create bucket" to finalize the process.<br>

![alter text](images/3.png)

### Step 2: Upload Your Website Files
1.  Open the newly created S3 bucket.<br>
2.  Navigate to the Objects tab and click on Upload.<br>
3.  Select all the website files you want to host (e.g., index.html,etc.).<br>
4.  Click Upload to add the files to your S3 bucket.<br>

![alter text](images/4.png)
Objects uploaded to the bucket.

### Step 3: Enable Static Website Hosting
1.  Navigate to the "Properties" tab of your S3 bucket.<br>
![alter text](images/5.png)


2.  Scroll down to the "Static website hosting" section and click "Edit."<br>
![alter text](images/6.png)

3.  Select the "Enable" option to activate static website hosting.<br>
4.  Enter the name of your index document (e.g., index.html), and optionally, provide an error document (e.g., error.html).<br>
![alter text](images/7.png)

5.  Click "Save changes" to apply the settings.<br>

### Step 4: Customize Public Access Settings
1.  In the "Edit Block public access (bucket settings)" screen, you will see four options:
![alter text](images/8.png)

2.  Choose the settings based on your requirements.<br>
3.  If you want to allow public access, uncheck the options as per your needs.<br>
4.  If you want to enforce strict blocking, ensure all options are checked or click the top-level "Block all public access" checkbox.<br>
![alter text](images/9.png)

5.  After selecting the desired settings, click the "Save changes" button at the bottom.<br>
6.  A confirmation dialog will appear, warning you that modifying these settings might make some objects public or private.<br>
7.  Enter "confirm" in the text field provided.<br>
8.  Click the "Confirm" button to apply your changes.
![alter text](images/10.png)

### Step 5: Enable Object Ownership
1.  In the bucket settings, click on Edit Object Ownership.<br>
2.  Select the option ACLs Enabled.<br>
3.  Click on the I acknowledge that ACLs will be restored (checkbox).
![alter text](images/11.png)

![alter text](images/12.png)


### Step 6: Make Objects Public
1.  Select the Objects tab.<br>
2.  Click on the Actions dropdown menu.<br>
3.  Select Make public.<br>
4.  Select the objects aws.jpg and index.html.<br>
5.  Click Make public.
![alter text](images/13.png)

## Result:

![alter text](images/14.png)


