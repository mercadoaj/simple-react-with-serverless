


# This is a simple react page that calls from a springboot serverless service.

serverless service: https://github.com/mercadoaj/springboot-serverless-with-mysql.

# To set-up this page, you need to the the following:

In the package.json, change the proxy parameter:

```
{
  "name": "frontend",
  "version": "0.1.0",
  "proxy": "https://tfk4h1ivz7.execute-api.ap-southeast-1.amazonaws.com/dev/person",
  "private": true,
  "dependencies": {
```
In addition, edit the `fetch()` calls too the correct path.

use this endpoint for reference:
  ![ScreenShot](/docs/endpoints.PNG)

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!