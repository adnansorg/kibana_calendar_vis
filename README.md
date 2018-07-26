# kibana_calendar_vis

A calendar heatmap visualization in Kibana Visualize app

![Demo](demo.gif)

## Installation

Copy installation file's url as same version of your kibana from [the repository releases](https://github.com/aaronoah/kibana_calendar_vis/releases).

And
```bash
$ cd path/to/your/kibana
$ bin/kibana-plugin install <installation file's url>
```

### Compatibility

The minimum supported version of Kibana is version 6.4.0.

## Development

Be sure to clone `kibana_calendar_vis` under a folder `kibana_extra` that is in parallel to `kibana` in order to properly link scripts and tests.

See the [kibana contributing guide](https://github.com/elastic/kibana/blob/master/CONTRIBUTING.md) for instructions setting up your development environment. Once you have completed that, use the following yarn scripts.

  - `yarn kbn bootstrap`

    Install dependencies and crosslink Kibana and all projects/plugins.

    > ***IMPORTANT:*** Use this script instead of `yarn` to install dependencies when switching branches, and re-run it whenever your dependencies change.

  - `yarn start`

    Start kibana and have it include this plugin. You can pass any arguments that you would normally send to `bin/kibana`

      ```
      yarn start --elasticsearch.url http://localhost:9220
      ```

  - `yarn build`

    Build a distributable archive of your plugin.

  - `yarn test`

    Run all tests.

    - `yarn test:browser`

      Run the browser tests in a real web browser.

    - `yarn test:jest`

      Run jest tests in command line.

    - `yarn test:functionalTests`

      Run functional tests in command line and a real browser.

For more information about any of these commands run `yarn ${task} --help`. For a full list of tasks checkout the `package.json` file, or run `yarn run`.
