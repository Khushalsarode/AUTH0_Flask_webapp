# Auth0 Python Web App Sample
This sample demonstrates how to add authentication to a Python web app using Auth0.

# Running the App
Before Running application or clonning of code please ensure to do following:
- To run the sample, make sure you have `python3` and `pip` installed.
- create an folder in your system and open cmd in the folder path
- If you have virtualenv already skip this step otherwise install it use 'pip install virtualenv' & check using 'virtualenv -version'
- Make an envirnment using 'python -m venv <nameforyourenv>
- To activate env : '<nameforyourenv>\Scripts\activate' or '<nameforyourenv>\Scripts\activat.bat' can be used either way
- Clone the repository into the folder
- Run: 'pip install -r requirements.txt'
- create an `.env` and populate it with the client ID, domain, secret, callback URL and audience for your
Auth0 app.

- .env file
  `
     AUTH0_CLIENT_ID=
     AUTH0_CLIENT_SECRET=
     AUTH0_DOMAIN=
     APP_SECRET_KEY=
you will get all above three value in application setting page of auth0 when logined and created application
For App_SECRET_KEY use 'openssl rand hex 32' and paste it here run command using shell
`
- After this add the following url as suggested:
- replace localhost by <local_DNS_IP> i.e 127.0.0.1 
Register `http://localhost:3000/callback` as `Allowed Callback URLs` and `http://localhost:3000`
as `Allowed Logout URLs` in your client settings.

- Run `pip install -r requirements.txt` to install the dependencies and run `python server.py`.
- The app will be served at [http://localhost:3000/](http://localhost:3000/).

## What is Auth0?
Auth0 helps you to:
* Add authentication with [multiple authentication sources](https://auth0.com/docs/identityproviders),
either social like **Google, Facebook, Microsoft Account, LinkedIn, GitHub, Twitter, Box, Salesforce, among others**,or
enterprise identity systems like **Windows Azure AD, Google Apps, Active Directory, ADFS or any SAML Identity Provider**.
* Add authentication through more traditional **[username/password databases](https://docs.auth0.com/mysql-connection-tutorial)**.
* Add support for **[linking different user accounts](https://auth0.com/docs/link-accounts)** with the same user.
* Support for generating signed [JSON Web Tokens](https://auth0.com/docs/jwt) to call your APIs and
**flow the user identity** securely.
* Analytics of how, when and where users are logging in.
* Pull data from other sources and add it to the user profile, through [JavaScript rules](https://auth0.com/docs/rules).

## Create a free account in Auth0

1. Go to [Auth0](https://auth0.com) and click Sign Up.
2. Use Google, GitHub or Microsoft Account to login.

## Author

[Auth0](https://auth0.com)

## License

This project is licensed under the MIT license. See the [LICENSE](../LICENSE) file for more info.
