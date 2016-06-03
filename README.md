# Promise Zone Explorer

### In honor of the [National Day of Civic Hacking 2016](https://www.codeforamerica.org/events/national-day-2016), we aim to provide tools to help decisionmakers better understand, visualize, and prioritize the challenges faced by the most disadvantaged neighborhoods in Sacramento.

### Getting Started

The development environment for this repo is using Node 6.2.0 and npm 3.8.9.

If node and npm are not installed on your system, it is recommended to install [nvm](https://github.com/creationix/nvm) to switch between versions.

After cloning the repo to your system, run `npm install` to install dependencies, then run `npm start serve` to start the Webpack Dev Server with a bundle that features live incremental builds. Navigate to [http://localhost:8080](http://localhost:8080) to see the web app in development.

Note: The included npm scripts will work on OS X/Linux environments, but include certain file system commands that will likely fail in Windows dev environments.

### Development & Scripts

Edit files in `./app/` folder, this is the entry point for the Webpack bundle. When running the production server, Webpack will build a bundle in a `./dist` folder that is not checked into the repo.

If any changes need to be made to the main html wrapper at `./index.html`, they will be copied to the `./dist` folder on build.

Start development server with live Webpack incremental builds:
```
npm run serve
```

Start production server and build Webpack bundle, simulates deployed state:
```
npm run serve:dist
```

Start production server only if dist bundle is already built:
```
npm start
```

Run ESLint on all JS files in `./app/`:
```
npm test
```
