Setup Auth0 dashboard:
===
1-) Create a client in dashboard. Select “Native” as type.

2-) Enable Google login for the client.

3-) In Allowed Callback URLs section of the client enter:
    
    file://\*


Testing the sample app in sample-app directory with Xcode:
===
0-) Go to sample-app directory. All commands below assume you are working in this directory.

1-) Copy `sample-auth0-credentials.js` file as `auth0-credentials.js` in the same directory. You must set your Auth0 `ClientId` and `Domain` in this sample so that it works. For that, just open the `auth0-credentials.js` file and replace the `{CLIENT_ID}` and `{DOMAIN}` fields with your account information.

2-) Install packages from command line

    >> cd ios
    >> pod install
    >> cd..
    >> npm install

3-) Open LockReact.xcworkspace in ios directory with Xcode and run.

If you get “Ignoring return value of function declared with warn_unused_result attribute” error message in RCTWebSocket project, click on Build Settings for RCTWebSocket and in “Custom Compiler Flags” setting remove -Werror -Wall options in “Other Warning Flags” section by pressing -

