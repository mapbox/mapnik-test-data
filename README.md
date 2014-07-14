### Public data available for testing.

To use as a dependency, add the following to your `package.json`:
```
"mapnik-test-data":"http://mapbox-npm.s3.amazonaws.com/package/mapnik-test-data-1.0.1-2cdd40c2669bcb4fe9fbf05b7f8f019c1e73a624.tgz"
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
