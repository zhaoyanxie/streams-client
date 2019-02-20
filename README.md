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
