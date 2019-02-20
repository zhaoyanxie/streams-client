# React-Router-Dom

## BrowserRouter

- A react component
- Listens to changes in the "history" object, which keeps track of the address bar in the browser
- Communicates the address to the route components
- Route components with path that matches the address will be displayed

## Bad Navigation

1. Adding an `<a/>` tag to the application with `href="/page2"`and click it
2. Browser makes a request to /page2
3. Development server responds with index.html file
4. Browser receives index.html file, dumps the old HTML file it was showing (including all React/Redux state data!). i.e. all API requests have to be re-fetched.
5. index.html lists out JS files in script tags, browser downloads and executes these scripts
6. App starts up

# Handling Authentication with React

| Email/Password Authentication                                                       | OAuth Authentication                                                                                             |
| ----------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| We store a record in a database with the user's email and password.                 | User authenticates with outside service provider (Google, Facebook, LinkedIn)                                    |
| When the user logins in, the email/pw entered is compared against the db's version. | User authorises the app to access their information.                                                             |
| A user is logged in if email/pw are correct.                                        | Outside provider tells us about the user.                                                                        |
|                                                                                     | We are trusting the outside provider to correctly handle identification of a user.                               |
|                                                                                     | OAuth can be used for user identification in the app and allowing the app to make actions on behalf of the user. |
