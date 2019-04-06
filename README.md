# account-kit-tester
A simple client for testing account kit workflows. Only SMS flow is supported as of yet.

- Run the `index.html` file from a web server.
- Input you app ID and redirect url and press login (make sure the redirect url matches the route from which `index.html` is served, and is registered in account kit for your app.
- Press login. After completing the SMS sign in, you will be redirected to the redirect url which will hopefully again load the `index.html` file, where you will now see an authorization code.
- Enter your account kit client secret and press get access token. If successful, an access token will now be visible which can be used to access the Graph Api.
