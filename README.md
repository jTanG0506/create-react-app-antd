# 🐜 create-react-app template with Ant Design

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app) and comes with [Ant Design's](https://github.com/ant-design/ant-design) UI Library.

## ✨ Features

- 🌈 Easy to override Ant Design's default styles.
- 🛡 Includes TypeScript support for predictable static types.
- ⚙️ Automatic rebuild and restart when changes are made to Ant Design overrides.
- 💼 Uses `craco-antd` to remove unused CSS, resulting in a smaller bundle size.

## 🎨 Changing Ant Design's styles

The default Ant Design theme can be modified using the Less file at `./src/styles/antOverrides.less`. You can change this file path in the `craco.config.js` file. An example `antOverrides.less` file is shown below.

```less
@import '~antd/dist/antd.less';

@primary-color: #1890ff;               // Primary color for all components
@link-color: #1890ff;                  // Link color
@success-color: #52c41a;               // Success state color
@warning-color: #faad14;               // Warning state color
@error-color: #f5222d;                 // Error state color
@font-size-base: 14px;                 // Main text font size
@text-color: rgba(0, 0, 0, 0.65);      // Main text color
```

The full list of Less variables can be found [here](https://github.com/ant-design/ant-design/blob/master/components/style/themes/default.less).

#### 🌚 Dark Theme
To use the dark theme, change `@import '~antd/dist/antd.less';` to `@import "~antd/dist/antd.dark.less";`.

## 🛠 Available Scripts

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
