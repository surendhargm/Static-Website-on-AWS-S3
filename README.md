# Static website hosted on AWS S3
## Steps to Follow:
### Step 1: Set Up an S3 Bucket
a.Log in to your AWS Management Console.<br>
b.In the search bar, type S3 and select the S3 service.<br>
c.Click the Create bucket button to begin the setup.<br>

![alter text](images/1.png)

bucket Creation Completed Successfully:<br>
d.Provide a unique name for your bucket (e.g.,aws-mystatic-website-s3) and select a preferred region.<br>

![alter text](images/2.png)

e.Disable the "Block all public access" option to make the website accessible publicly.<br>
f.Acknowledge the warning by selecting the checkbox, then click "Create bucket" to finalize the process.<br>

![alter text](images/3.png)

### Step 2: Upload Your Website Files
a.Open the newly created S3 bucket.<br>
b.Navigate to the Objects tab and click on Upload.<br>
c.Select all the website files you want to host (e.g., index.html,etc.).<br>
d.Click Upload to add the files to your S3 bucket.<br>

![alter text](images/4.png)
Objects uploaded to the bucket.

### Step 3: Enable Static Website Hosting
a.Navigate to the "Properties" tab of your S3 bucket.<br>
![alter text](images/5.png)


b.Scroll down to the "Static website hosting" section and click "Edit."<br>
![alter text](images/6.png)

c.Select the "Enable" option to activate static website hosting.<br>
d.Enter the name of your index document (e.g., index.html), and optionally, provide an error document (e.g., error.html).<br>
![alter text](images/7.png)

e.Click "Save changes" to apply the settings.<br>

### Step 4: Customize Public Access Settings
a.In the "Edit Block public access (bucket settings)" screen, you will see four options:
![alter text](images/8.png)

b.Choose the settings based on your requirements.<br>
c.If you want to allow public access, uncheck the options as per your needs.<br>
d.If you want to enforce strict blocking, ensure all options are checked or click the top-level "Block all public access" checkbox.<br>
![alter text](images/9.png)

e.After selecting the desired settings, click the "Save changes" button at the bottom.<br>
f.A confirmation dialog will appear, warning you that modifying these settings might make some objects public or private.<br>
g.Enter "confirm" in the text field provided.<br>
h.Click the "Confirm" button to apply your changes.
![alter text](images/10.png)

### Step 5: Enable Object Ownership
a.In the bucket settings, click on Edit Object Ownership.<br>
b.Select the option ACLs Enabled.<br>
c.Click on the I acknowledge that ACLs will be restored (checkbox).
![alter text](images/11.png)

![alter text](images/12.png)


### Step 6: Make Objects Public
a.Select the Objects tab.<br>
b.Click on the Actions dropdown menu.<br>
c.Select Make public.<br>
d.Select the objects aws.jpg and index.html.<br>
e.Click Make public.
![alter text](images/13.png)

## Result:

![alter text](images/14.png)
