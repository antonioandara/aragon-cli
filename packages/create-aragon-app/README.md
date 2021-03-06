# Create Aragon App

Will set up an Aragon app project so you can start building your app from a functional boilerplate.

## Command

```sh
create-aragon-app <app-name> [boilerplate]
```

- `app-name`: The name or ENS domain name for your app in an aragonPM Registry (e.g. `myapp` or `myapp.aragonpm.eth`). If only the name is provided it will create your app on the default `aragonpm.eth` registry.

- `boilerplate`: the Github repo name or alias for a boilerplate to set up your app. It default to `react`. The currently available boilerplates are:
  - `react`: this boilerplate contains a very basic Counter app and a webapp for interacting with it. It showcases the end-to-end interaction using the [buidler](https://buidler.dev/) task runner with a custom plugin for developing Aragon apps from the contracts to the webapp.
  - `reactWithCli`: (deprecated) this is similar to the `react` boilerplate but use aragonCLI as development tool.

## Example

```sh
npx create-aragon-app myapp
cd myapp
npm start
```

Once finished, this will open [http://localhost:3000/](http://localhost:3000/) in your default browser.

_Note: [npx](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b) comes with npm 5.2+ and higher. If you use npm 5.1 or earlier, you can't use `npx`. Instead, install `create-aragon-app` globally._

_Note: We also support [yarn](https://yarnpkg.com/getting-started/install) as a package manager during installation and will use it by default if you have it available in your PATH._

# Tests

In the root of the repository, run:

```sh
npm test
```
