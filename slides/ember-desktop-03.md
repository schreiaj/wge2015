# Do it in Ember
```
ember install ember-cli-node-webkit
```
* Installs the NPM package
* Adds the blueprint files
* Installs the `nw` NPM package locally

## Don't forget to config
1. Update `package.json` to include an entry for "main" that will be a path to the HTML file.
2. modify `ENV.locationType` to hash because there's no webserver
