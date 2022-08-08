Simple Nodejs implementation of Auth using AWS Cognito - 
================================================================

Referenced from -  https://onexlab-io.medium.com/aws-cognito-node-js-cc05760b61c3

Steps : 

1. Follow the above ref link to create a user pool and grab the values required in the *.env.example* file
2. Create the .env file as per *.env.example* file
3. `npm i`
4. Use the Signup(), Verify() and Login() function in *index.js* to signup a hardcoded email id as in index.js
5. `node index.js`
6. On successful signin response should be like - 

```
{
  statusCode: 200,
  response: {
    token: {
      accessToken: 'xxxxx-token-xxxxxx',
      idToken: 'xxxxx-token-xxxxxx',
      refreshToken: 'xxxxx-token-xxxxxx'
    },
    email: 'user@example.com',
    exp: 1659998003,
    uid: 'xxx-xxxx-xxxxx-xxxx',
    auth_time: 1659994403,
    token_use: 'id'
  }
}
```