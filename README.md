### Public data available for testing.

To use as a dependency, add the following to your `package.json`:
```
"mapnik-test-data":"http://mapbox-npm.s3.amazonaws.com/package/mapnik-test-data-2.0.1-98e4e5f4d94979576d4fff22c8e447a3a5048302.tgz"
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
