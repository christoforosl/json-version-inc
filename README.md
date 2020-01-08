# json-version-inc
> Increments a version field property in a json file and rewrites the original file

## Why ?
> I needed a way to increment the versions for android and ios react-native expo builds in order to be able to use CI and fastlane to submit builds to Play Store and App Store.

## Install
```
$ npm install -g json-version-inc
```

## Usage
```
json-version-inc -j [JSON_FILE_PATH] -p [VERSION_PROPERTY_PATH] -t [TYPE: MAJOR | MINOR | PATCH] -o [xml|json|text]
```

## Example
```
json-version-inc -j ./app.json -p expo.ios.buildNumber -t PATCH -o xml
> to produce xml output like this: <newVersion>1.0.7</newVersion>

json-version-inc -j ./app.json -p expo.ios.buildNumber -t PATCH -o json
> to produce json output like this: {"newVersion":"1.0.8"}

```

## License

MIT
