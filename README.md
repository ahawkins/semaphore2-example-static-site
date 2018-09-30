# Semaphore Static Site Example

This repo demonstrates a [hugo][] static site to AWS. The example
configures AWS access, installs Hugo, builds the site, and syncs files
to the relevant S3 bucket.

Here's how to setup it up:

1. Fill in your AWS credentials in `secret.yml`. Create the secret
   with: `sem create -f secret.yml`
2. Create and configure an [S3 website bucket][aws].
3. Configure the `BUCKET_NAME` and `AWS_DEFAULT_REGION` in
   `.semaphore/semaphore.yml`
4. Commit and push.
5. Done!

This example is not Hugo specific. The same concept applies to any
static generator or single page application build tools.

[hugo]: https://gohugo.io
[aws]: https://docs.aws.amazon.com/AmazonS3/latest/dev/HowDoIWebsiteConfiguration.html
