### Public data available for testing.

To use as a dependency, add the following to your `package.json`:
```
"mapnik-test-data":"https://mapbox-npm.s3.amazonaws.com/package/mapnik-test-data-2.0.5-c84800ed20a6a9bc2143dd11b1b2a3190b9ae698.tgz"
```

Then use in your js file like so:
```
//require
var pathToData = path.dirname(require.resolve('mapnik-test-data'));

//and use
fs.readFile(pathToData + '/data/geotiff/sample.tif', function (err, data) {
  if (err) throw err;
  console.log(data);
});

```
