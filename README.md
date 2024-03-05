# Keyboard-Focus-Typing
A web to  improve typing speed through focus the word.

# Static Website Deployment on AWS S3

Deploymenteploy a static website on Amazon S3 with a custom error page.

## Steps:

1. **Create S3 Bucket:**
   - Create a new bucket in the AWS S3 console.

2. **Upload Files:**
   - Upload HTML, CSS, JS files, including `error.html`.

3. **Configure Hosting:**
   - Enable static website hosting in bucket properties.
   - Set index document (e.g., index.html) and error document (e.g., error.html).

4. **Set Public Access:**
   - Configure bucket policy for public read access.

    - Go to the "Permissions" tab.
    - Click on "Bucket Policy."
    - Add a policy allowing public read access. Replace "your-bucket-name" with your bucket name.
  
  ```json
{
    "Version": "2012-10-17",
    "Id": "Policy1705994504443",
    "Statement": [
        {
            "Sid": "Stmt1705994503332",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::devops-training-yatharth/*"
        }
    ]
}
```
  

5. **Access Website:**
   - Find the endpoint URL under static website hosting.


Now, static website is live on AWS S3. Replace "your-bucket-name" with your actual bucket name.

## Author
- [Visit My Portfolio](https://yatharthchauhan.me)

- [LinkedIn: Yatharth Chauhan](https://www.linkedin.com/in/yatharth-chauhan-729674202/)

- [GitHub: Yatharth Chauhan](https://github.com/YatharthChauhan2362)

