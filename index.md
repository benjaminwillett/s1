## Welcome to my AWS S1 Pages

Learn How To Host Images Amazon S3
Step 1: Create an AWS Account
Head on over to https://aws.amazon.com and setup a new account. You should only need a credit card and a phone so that Amazon can call to verify you are real.
 
Step 2: Create an S3 Bucket
Once your account is setup and verified, we need to create a bucket. A bucket is similar to a folder on your computer and the only limitation of a bucket is that you must have a unique name across all of aws. Typically we suggest your business name – media. (ie: mybusinessname-media).
1. Once logged in and verified in AWS, click the Services dropdown in the top left and Select Amazon S3 
2. Click Create Bucket, enter the name, and select Region: US Standard
 
Step 3: Upload your files into the bucket
Once created, click on the bucket name in the list on the left and then click Upload on the next screen
 
Step 4: Make the Bucket Public So we Can grab the images
After you upload all files, the last step is to make the bucket public so we can get the images from it.
Click to the right of the bucket name and not on the text to get the properties tab to the right.
Click permissions and Add Bucket Policy and copy and paste the following in making SURE you change the highlighted word “bucket” below to match the bucket name you created in step 2.
{ “Version“:“2008-10-17”, “Statement“:[{ “Sid“:“AllowPublicRead”, “Effect“:“Allow”, “Principal“: { “AWS“: “*” }, “Action“:[“s3:GetObject”], “Resource“:[“arn:aws:s3:::bucket/*” ] } ] }
 
5. Find the URLs for your files by clicking on the bucket name, then selecting a single file and showing the properties.
If you did everything right, clicking that link should show you the image in your browser.
 
Now you can send us an example URL of one file and we’ll be able to get your files over the internet with out the need for a disk and so you can share in the future.
If you need to add new ones you can repeat step 3 over and over again.

1.Create AWS Account
2.Create S3 Bucket
3.Upload files to the S3 Bucket
4.Make bucket accessible to the world
5.Found how to get the URL for the image.


### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/benjaminwillett/s1/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
