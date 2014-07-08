### Public data available for testing.

To use as a dependency, add the following to your `package.json`:
```
"mapnik-test-data":"http://mapbox-npm.s3.amazonaws.com/package/mapnik-test-data-0.0.1-e0ce09b79f92b1ae96fa2062199966510a0b3461.tgz"
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
