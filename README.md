# npmdoc-react-native-code-push

#### api documentation for  [react-native-code-push (v2.0.2-beta)](https://microsoft.github.io/code-push)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-native-code-push.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-native-code-push) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-native-code-push.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-native-code-push)

#### React Native plugin for the CodePush service

[![NPM](https://nodei.co/npm/react-native-code-push.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-native-code-push)

- [https://npmdoc.github.io/node-npmdoc-react-native-code-push/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-native-code-push/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-native-code-push/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-native-code-push/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-native-code-push/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-native-code-push/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "react-native-code-push",
    "version": "2.0.2-beta",
    "description": "React Native plugin for the CodePush service",
    "main": "CodePush.js",
    "typings": "typings/react-native-code-push.d.ts",
    "homepage": "https://microsoft.github.io/code-push",
    "keywords": [
        "react-native",
        "code",
        "push"
    ],
    "author": "Microsoft Corporation",
    "license": "MIT",
    "repository": {
        "type": "git",
        "url": "https://github.com/Microsoft/react-native-code-push"
    },
    "dependencies": {
        "code-push": "1.8.0-beta",
        "glob": "^5.0.15",
        "inquirer": "1.1.2",
        "plist": "1.2.0",
        "xcode": "0.9.2"
    },
    "devDependencies": {
        "archiver": "latest",
        "body-parser": "latest",
        "code-push-plugin-testing-framework": "file:./code-push-plugin-testing-framework",
        "del": "latest",
        "express": "latest",
        "gulp-insert": "latest",
        "gulp-tslint": "latest",
        "gulp-typescript": "2.12.2",
        "mkdirp": "latest",
        "q": "^1.4.1",
        "run-sequence": "latest",
        "tslint": "^4.3.1",
        "typescript": "^2.1.5"
    },
    "rnpm": {
        "android": {
            "packageInstance": "new CodePush(${androidDeploymentKey}, getApplicationContext(), BuildConfig.DEBUG)"
        },
        "ios": {
            "sharedLibraries": [
                "libz"
            ]
        },
        "params": [
            {
                "type": "input",
                "name": "androidDeploymentKey",
                "message": "What is your CodePush deployment key for Android (hit <ENTER> to ignore)"
            }
        ],
        "commands": {
            "postlink": "node node_modules/react-native-code-push/scripts/postlink/run"
        }
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
