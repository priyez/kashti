# kashti

Brigade v1 pipelines can be difficult to inspect from the command line alone. Kashti provides a web dashboard for viewing pipeline builds and examining the projects, scripts, and jobs behind them.

> **Status:** Brigade v1 reached end-of-life on June 1, 2022. This project is based on the archived Brigade v1 dashboard and is no longer maintained for new Brigade deployments.

## Features

- Visualize Brigade pipeline builds in a web dashboard.
- Browse Brigade projects.
- Inspect the scripts used by projects.
- Examine jobs associated with pipeline builds.

## Installation

Kashti is a TypeScript application. Install its dependencies and build the frontend with npm:

```sh
npm ci
npm run build
```

For local development, use the project's development server:

```sh
npm start
```

Kashti requires a Brigade v1 environment for its dashboard data. See the project documentation and deployment configuration for details about connecting it to Brigade.

## Usage

Start Kashti on a local development host and port:

```sh
npm start -- --host 0.0.0.0 --port 4200
```

Open `http://localhost:4200/` in a browser, then use the dashboard to view Brigade projects, pipeline builds, scripts, and jobs.

## License

Kashti is licensed under the Apache License 2.0. This project is based on [brigadecore/kashti](https://github.com/brigadecore/kashti), which is also licensed under Apache-2.0. See [LICENSE](LICENSE) for the full license text.
