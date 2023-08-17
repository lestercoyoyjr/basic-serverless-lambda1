Basic Serverless Lambda using the Serverless Framework & GitHub Actions

IMPORTANT NOTE:

When using '$ serverless create --template aws-nodejs' don't forget to:

1. Make sure node is updated.
2. Access as root and go to the folder of the project.
3. run '$ npm i -g serverless'.
4. run '$ serverless create --template aws-nodejs'.
5. The most important, make sure that if you created your project using Github desktop, the ```.gitignore``` file is not added, cause it has to be created by serverless framework.

This is the template for github actions:
https://github.com/serverless/github-action

Probably, you will have an error like this one

```
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for ...
```

So, follow this guide in order to access with token instead of password

https://collabnix.com/how-to-fix-support-for-password-authentication-was-removed-error-in-github/

IMPORTANT:
In 2023, add S3fullAccess permission too, not just mentioned on video.