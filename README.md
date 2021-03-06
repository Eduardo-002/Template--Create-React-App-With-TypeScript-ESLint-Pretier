This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Setup Create-React-App with TypeScript,ESLint and Prettier

[reference link](https://medium.com/@brygrill/create-react-app-with-typescript-eslint-prettier-and-github-actions-f3ce6a571c97)<br />
npx create-react-app my-app --template typescript<br />
yarn add -D @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-airbnb-typescript eslint-plugin-jest<br />
yarn add -D @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-airbnb-typescript@6.3.2 eslint-plugin-jest eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react-hooks eslint-plugin-react prettier eslint-config-prettier eslint-plugin-prettier<br />
yarn add -D prettier eslint-config-prettier eslint-plugin-prettier<br />
-> copy config from .eslintrc.js<br />
-> add to package.json the next "scripts": {<br />
  "format": "prettier --write src/**/*.ts{,x}",<br />
  "lint": "tsc --noEmit && eslint src/**/*.ts{,x}"<br />
}<br />
// use "yarn run format" to use prettier and "yarn run lint" to run eslint<br />
// p.s. if you use the reference link don't forget to add in .eslintrc.js the rule ("@typescript-eslint/camelcase": "off")<br />

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
