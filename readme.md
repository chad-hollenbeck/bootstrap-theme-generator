# Bootstrap Theme Generator

Bootstrap v5.3

## How To Use

1. Download Node & NPM (LTS)
1. Modify `src/theme.scss` with desired additions and overrides. To revert to default bootstrap settings, replace the content of theme.scss with _default.scss. 
1. Generate the theme.css file by executing `npm run build`
1. Copy the theme.css files out of the `dist` folder and into your project. 
1. Add a `src` link in HTML header for the new theme file. Remove any references to the default bootstrap css
1. Add a `script` tag  for the matching version of the bootstrap.js file used to generate the theme. You can find this from the CDN or a local download of the Bootstrap css/js suite. 


## Upgrading
To support an older/newer version of bootstrap:

1. Modify the bootstrap version in package.json
1. Install the new packages with `npm i` or `yarn i`
1. Locate the `_variables.scss` file from the package files
1. Replace all relevant variable names in _theme.scss. Keep in mind variable names may change between bootstrap versions.
1. Follow the steps under How To Use to generate the new theme file. 


