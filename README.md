# Weather Dashboard

React implementation of a weather dashboard, inspired by [Weather-Dashboard-Forecast](https://github.com/vlaine/Weather-Forecast-Dashboard) by @vlaine, after I got extremely disappointed discovering that [DarkSky API](https://darksky.net/dev) will be acquired by Apple soon and is no more accepting dev applications (can't believe the timing 🙄 ).
<br/>Using [OpenWeather API](https://home.openweathermap.org/) instead, with some tweaks, and [WeatherBit](https://www.weatherbit.io/) for the live alerts.

Live app: https://weather-forecast-dashboard.web.app/ (hosted on Firebase)

The dashboard doesn't query the APIs directly but uses a [middleware API](https://github.com/martapanc/weather-forecast-proxy-api/blob/master/app.py), which acts as a proxy between the client app and the APIs, in order to avoid overloading the latter with requests. 

---
#### Blue theme
<img src="src/assets/samples/Screenshot_1.png" width="100%" alt="Screenshot 1"/>

#### Black theme
<img src="src/assets/samples/Screenshot_2.png" width="100%" alt="Screenshot 2"/>

---

## Project setup
- Create a file `.env` in the main directory with the line 
```
REACT_APP_API_KEY=<your OpenWeather API KEY>
```
Do not forget to prepend 'REACT_API_' to any key, or the dotenv library will not be able to read it correctly.
- Edit `src/constants.js` to set the preferred configuration

The project can be run using 
```
npm run start
```
and accessed in the browser at http://localhost:3000

---
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `yarn build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
