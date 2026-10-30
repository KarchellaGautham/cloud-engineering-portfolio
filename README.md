# Cloud Engineering Portfolio

My personal portfolio website showcasing my skills, learning journey, and projects in Cloud Computing and DevOps.

## Live Website

[View My Portfolio](https://d2k2wmhtz9z5bn.cloudfront.net)

## Technologies Used

- HTML
- CSS
- JavaScript
- Amazon S3
- Amazon CloudFront
- CloudFront Origin Access Control (OAC)
- HTTPS

## Architecture

The portfolio is hosted using Amazon S3 and delivered through Amazon CloudFront.

**Request flow:**

Visitor → CloudFront (HTTPS) → Origin Access Control (OAC) → Private S3 Bucket → `index.html`

## AWS Implementation

1. Created an Amazon S3 general-purpose bucket.
2. Uploaded the portfolio as `index.html`.
3. Kept S3 Block Public Access enabled.
4. Created a CloudFront distribution.
5. Configured Origin Access Control to allow CloudFront to access the private S3 bucket.
6. Configured the default root object as `index.html`.
7. Enabled HTTP-to-HTTPS redirection.
8. Verified that the portfolio was accessible through the CloudFront distribution URL.

## Security

- S3 bucket is not publicly accessible.
- CloudFront accesses the S3 origin using OAC.
- Website visitors access the portfolio through HTTPS.

## Future Improvements

- Add a custom domain.
- Automate deployment using GitHub Actions.
- Add cloud engineering projects.
- Expand the portfolio with serverless AWS applications.

## Author

Aspiring Cloud Engineer | B.Tech Computer Science Student

[GitHub](https://github.com/KarchellaGautham) · [LinkedIn](https://www.linkedin.com/in/gautham-karchella)
