# Official Dowell-Mobile-Login-Component Documentation
         flutterflow component of login


# Understanding AppState

The Login Component stores user information in you project's appstate, so developer dont have to call login api's
and update the app state.

Please note that in Appstate you can see two new variables ,1 response, 2 sessionId

response (Json) after login user's information will be stored in this variable. you can access userinfo, portfolio info, org info, selected workspaces and its id.
sessionId (String) after login user's session id will be stored in this variable. you can use this for handeling user logs.

# Accessing User info through Json Path

| Value | Json Path |
| --- | --- |
| ` user name ` | $.userinfo.username |
| `first name` | $.userinfo.first_name |
| `email` | $.userinfo.email |
| `profile image` | $.userinfo.profileImage |
| `phone` | $.userinfo.phone |



