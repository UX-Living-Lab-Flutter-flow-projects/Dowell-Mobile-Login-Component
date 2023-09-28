# Official Dowell-Mobile-Login-Component Documentation
         flutterflow component of login


## Understanding how Login Component works
We value our devs , so to save their time, we developed Login component in flutterflow, which means we can use it every 
FF project, without creating api calls, and updating AppState each time.


```mermaid
graph TD;
    FlutterFlow --> Team Code;
    Team Code --> Login Component;
     Login Component--> Project x;
     Login Component-->  Project y;
    C-->D;
```

### App State
As mentioned earlier, The Login Component stores user information in you project's appstate, so developer dont have to call login api's
and update the app state.

Please note that in Appstate you can see two new variables ,1 response, 2 sessionId

response (Json) after login user's information will be stored in this variable. you can access userinfo, portfolio info, org info, selected workspaces and its id.
sessionId (String) after login user's session id will be stored in this variable. you can use this for handeling user logs.

### Accessing Basic User information through Json Path
First select the response variable to access the data and then select json path as value, then you can give a specific
json path to retrieve your needed value. 

| Value | Json Path |
| --- | --- |
| ` user name ` | $.userinfo.username |
| `first name` | $.userinfo.first_name |
| `email` | $.userinfo.email |
| `profile image` | $.userinfo.profileImage |
| `phone` | $.userinfo.phone |



