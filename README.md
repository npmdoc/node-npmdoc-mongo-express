# api documentation for  [mongo-express (v0.39.1)](https://github.com/mongo-express/mongo-express#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mongo-express.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mongo-express) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mongo-express.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mongo-express)
#### Web-based admin interface for MongoDB

[![NPM](https://nodei.co/npm/mongo-express.png?downloads=true)](https://www.npmjs.com/package/mongo-express)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mongo-express/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mongo-express_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mongo-express/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mongo-express/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mongo-express/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "https://github.com/mongo-express"
    },
    "bin": {
        "mongo-express": "./app.js"
    },
    "bugs": {
        "url": "https://github.com/mongo-express/mongo-express/issues"
    },
    "dependencies": {
        "async": "2.0.1",
        "basic-auth-connect": "^1.0.0",
        "body-parser": "1.15.2",
        "busboy": "^0.2.13",
        "cli-color": "^1.1.0",
        "commander": "^2.9.0",
        "cookie-parser": "1.4.3",
        "cross-env": "^3.2.4",
        "csurf": "1.9.0",
        "errorhandler": "1.4.3",
        "express": "4.14.0",
        "express-session": "1.14.1",
        "flat": "^2.0.1",
        "gridfs-stream": "^1.1.1",
        "json2csv": "^3.7.1",
        "lodash": "~4.17.4",
        "method-override": "2.3.6",
        "mongodb": "2.2.24",
        "morgan": "1.7.0",
        "serve-favicon": "2.3.0",
        "swig-templates": "2.0.2",
        "update-notifier": "1.0.2"
    },
    "description": "Web-based admin interface for MongoDB",
    "devDependencies": {
        "assets-webpack-plugin": "^3.5.1",
        "babel-core": "^6.23.1",
        "babel-loader": "^6.3.2",
        "babel-preset-es2015": "^6.22.0",
        "bootstrap": "^3.3.7",
        "chai": "3.5.0",
        "clean-webpack-plugin": "^0.1.15",
        "codemirror": "^5.23.0",
        "concurrently": "^3.3.0",
        "copy-webpack-plugin": "^4.0.1",
        "eslint": "~3.9.1",
        "eslint-config-airbnb-base": "^8.0.0",
        "eslint-plugin-import": "^1.16.0",
        "eslint-plugin-lodash": "^2.3.5",
        "jquery": "^3.1.1",
        "mocha": "3.0.2",
        "nodemon": "^1.11.0",
        "pre-commit": "1.1.3",
        "renderjson": "^1.2.3",
        "supertest": "^3.0.0",
        "webpack": "^2.2.1"
    },
    "directories": {},
    "dist": {
        "shasum": "2362cda67eb7ff36c1567b81aaf1750df32e6a5c",
        "tarball": "https://registry.npmjs.org/mongo-express/-/mongo-express-0.39.1.tgz"
    },
    "engines": {
        "node": ">=4.0.0",
        "npm": ">=3.0.0"
    },
    "gitHead": "5790acfa5f4a49535dc577981c70e2efdd01f752",
    "homepage": "https://github.com/mongo-express/mongo-express#readme",
    "keywords": [
        "admin",
        "administration",
        "collection",
        "database",
        "GUI",
        "interface",
        "manage",
        "manage-mongo",
        "mongo",
        "mongodb",
        "phpmyadmin",
        "UI",
        "web-based"
    ],
    "license": "MIT",
    "main": "./middleware",
    "maintainers": [
        {
            "name": "andz",
            "email": "zegg90@gmail.com"
        },
        {
            "name": "dozoisch",
            "email": "hugo@dozoisch.com"
        },
        {
            "name": "wulfsolter",
            "email": "wulf@wulf.co.nz"
        }
    ],
    "name": "mongo-express",
    "optionalDependencies": {},
    "pre-commit": [
        "test"
    ],
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/mongo-express/mongo-express.git"
    },
    "scripts": {
        "build": "cross-env NODE_ENV=production webpack",
        "build-dev": "webpack --watch",
        "lint": "eslint .",
        "mocha": "cross-env NODE_ENV=test mocha",
        "prepublish": "npm run build",
        "start": "cross-env NODE_ENV=production node app",
        "start-dev": "concurrently --kill-others \"nodemon app\" \"npm run build-dev\"",
        "test": "npm run mocha && npm run lint",
        "test-watch": "cross-env NODE_ENV=test mocha --watch --reporter spec"
    },
    "version": "0.39.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mongo-express](#apidoc.module.mongo-express)
1.  object <span class="apidocSignatureSpan">mongo-express.</span>bson
1.  object <span class="apidocSignatureSpan">mongo-express.</span>filters
1.  object <span class="apidocSignatureSpan">mongo-express.</span>json
1.  object <span class="apidocSignatureSpan">mongo-express.</span>utils

#### [module mongo-express.bson](#apidoc.module.mongo-express.bson)
1.  [function <span class="apidocSignatureSpan">mongo-express.bson.</span>getSandbox ()](#apidoc.element.mongo-express.bson.getSandbox)
1.  [function <span class="apidocSignatureSpan">mongo-express.bson.</span>hexToObjectId (string)](#apidoc.element.mongo-express.bson.hexToObjectId)
1.  [function <span class="apidocSignatureSpan">mongo-express.bson.</span>toBSON (string)](#apidoc.element.mongo-express.bson.toBSON)
1.  [function <span class="apidocSignatureSpan">mongo-express.bson.</span>toJsonString (doc)](#apidoc.element.mongo-express.bson.toJsonString)
1.  [function <span class="apidocSignatureSpan">mongo-express.bson.</span>toObjectId (string)](#apidoc.element.mongo-express.bson.toObjectId)
1.  [function <span class="apidocSignatureSpan">mongo-express.bson.</span>toSafeBSON (string)](#apidoc.element.mongo-express.bson.toSafeBSON)
1.  [function <span class="apidocSignatureSpan">mongo-express.bson.</span>toString (doc)](#apidoc.element.mongo-express.bson.toString)

#### [module mongo-express.filters](#apidoc.module.mongo-express.filters)
1.  [function <span class="apidocSignatureSpan">mongo-express.filters.</span>convertBytes (input)](#apidoc.element.mongo-express.filters.convertBytes)
1.  [function <span class="apidocSignatureSpan">mongo-express.filters.</span>is_embeddedDocumentNotation (input)](#apidoc.element.mongo-express.filters.is_embeddedDocumentNotation)
1.  [function <span class="apidocSignatureSpan">mongo-express.filters.</span>json (input)](#apidoc.element.mongo-express.filters.json)
1.  [function <span class="apidocSignatureSpan">mongo-express.filters.</span>stringDocIDs (input)](#apidoc.element.mongo-express.filters.stringDocIDs)
1.  [function <span class="apidocSignatureSpan">mongo-express.filters.</span>to_display (input)](#apidoc.element.mongo-express.filters.to_display)
1.  [function <span class="apidocSignatureSpan">mongo-express.filters.</span>to_string (input)](#apidoc.element.mongo-express.filters.to_string)

#### [module mongo-express.json](#apidoc.module.mongo-express.json)
1.  [function <span class="apidocSignatureSpan">mongo-express.json.</span>stringify (value, replacer, space)](#apidoc.element.mongo-express.json.stringify)

#### [module mongo-express.utils](#apidoc.module.mongo-express.utils)
1.  [function <span class="apidocSignatureSpan">mongo-express.utils.</span>buildCollectionURL (base, dbName, collectionName)](#apidoc.element.mongo-express.utils.buildCollectionURL)
1.  [function <span class="apidocSignatureSpan">mongo-express.utils.</span>bytesToSize (bytes)](#apidoc.element.mongo-express.utils.bytesToSize)
1.  [function <span class="apidocSignatureSpan">mongo-express.utils.</span>colsToGrid (cols)](#apidoc.element.mongo-express.utils.colsToGrid)
1.  [function <span class="apidocSignatureSpan">mongo-express.utils.</span>deepmerge (target, src)](#apidoc.element.mongo-express.utils.deepmerge)
1.  [function <span class="apidocSignatureSpan">mongo-express.utils.</span>roughSizeOfObject (object)](#apidoc.element.mongo-express.utils.roughSizeOfObject)



# <a name="apidoc.module.mongo-express"></a>[module mongo-express](#apidoc.module.mongo-express)



# <a name="apidoc.module.mongo-express.bson"></a>[module mongo-express.bson](#apidoc.module.mongo-express.bson)

#### <a name="apidoc.element.mongo-express.bson.getSandbox"></a>[function <span class="apidocSignatureSpan">mongo-express.bson.</span>getSandbox ()](#apidoc.element.mongo-express.bson.getSandbox)
- description and source-code
```javascript
getSandbox = function () {
  return {
    Long: mongodb.Long,
    NumberLong: mongodb.Long,
    Double: mongodb.Double,
    NumberDouble: mongodb.Double,
    ObjectId: mongodb.ObjectID,
    ObjectID: mongodb.ObjectID,
    Timestamp: Timestamp,
    DBRef: DBRef,
    Dbref: DBRef,
    Binary: mongodb.Binary,
    BinData: mongodb.Binary,
    Code: mongodb.Code,
    Symbol: mongodb.Symbol,
    MinKey: mongodb.MinKey,
    MaxKey: mongodb.MaxKey,
    ISODate: Date,
    Date: Date,
    Buffer: Buffer,
  };
}
```
- example usage
```shell
...
};
};

//JSON.parse doesn't support BSON data types
//Document is evaluated in a vm in order to support BSON data types
//Sandbox contains BSON data type functions from node-mongodb-native
exports.toBSON = function (string) {
var sandbox = exports.getSandbox();

string = string.replace(/ISODate\(/g, 'new ISODate(');
string = string.replace(/Binary\(("[^"]+"),/g, 'Binary(new Buffer($1, "base64"),');

vm.runInNewContext('doc = eval((' + string + '));', sandbox);

return sandbox.doc;
...
```

#### <a name="apidoc.element.mongo-express.bson.hexToObjectId"></a>[function <span class="apidocSignatureSpan">mongo-express.bson.</span>hexToObjectId (string)](#apidoc.element.mongo-express.bson.hexToObjectId)
- description and source-code
```javascript
hexToObjectId = function (string) {
  if (!/^[0-9a-f]{24}$/.test(string)) {
    return false;
  }
  var sandbox = exports.getSandbox();
  return sandbox.ObjectID(string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.bson.toBSON"></a>[function <span class="apidocSignatureSpan">mongo-express.bson.</span>toBSON (string)](#apidoc.element.mongo-express.bson.toBSON)
- description and source-code
```javascript
toBSON = function (string) {
  var sandbox = exports.getSandbox();

  string = string.replace(/ISODate\(/g, 'new ISODate(');
  string = string.replace(/Binary\(("[^"]+"),/g, 'Binary(new Buffer($1, "base64"),');

  vm.runInNewContext('doc = eval((' + string + '));', sandbox);

  return sandbox.doc;
}
```
- example usage
```shell
...
};

// This function as the name suggests attempts to parse
// the free form string in to BSON, since the possibilities of failure
// are higher, this function uses a try..catch
exports.toSafeBSON = function (string) {
  try {
    var bsonObject = exports.toBSON(string);
    return bsonObject;
  } catch (err) {
    return null;
  }
};

// Converts string to ObjectID.
...
```

#### <a name="apidoc.element.mongo-express.bson.toJsonString"></a>[function <span class="apidocSignatureSpan">mongo-express.bson.</span>toJsonString (doc)](#apidoc.element.mongo-express.bson.toJsonString)
- description and source-code
```javascript
toJsonString = function (doc) {
  let sJson = json.stringify(doc, null);
  sJson = sJson.replace(/ObjectID\(([^)]+)\)/g, '{ "$oid": $1 }');
  sJson = sJson.replace(/DBRef\(([^)]+)\)/g, '{ "$ref": $1 }');
  sJson = sJson.replace(/ISODate\(([^)]+)\)/g, '$1');
  return sJson;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.bson.toObjectId"></a>[function <span class="apidocSignatureSpan">mongo-express.bson.</span>toObjectId (string)](#apidoc.element.mongo-express.bson.toObjectId)
- description and source-code
```javascript
toObjectId = function (string) {
  var sandbox = exports.getSandbox();

  // Validation
  if (
    !string ||                                            // No input at all
    string === '' ||                                      // empty string
    string.toUpperCase().indexOf('OBJECTID(') === -1 ||   // missing the opening 'ObjectID('
    string.indexOf(')') === -1                            // missing the closing '('
  ) {
    return false;
  }

  // Strip quotes
  string = string.replace('"', '').replace('"', '');

  // Convert ObjectId("526ddf5a9f610ffd26000001") to 526ddf5a9f610ffd26000001
  string = string.replace(/ObjectID\(/i, '').replace(')', '');

  // Make sure it's a 24-character string to prevent errors.
  if (string.length === 24) {
    return sandbox.ObjectID(string);
  } else {
    return false;
  }
}
```
- example usage
```shell
...

var DBRef = function (namespace, oid, db) {
  //Allow empty/undefined db value
  if (db === undefined || db === null) {
    db = '';
  }

  var objectId = exports.toObjectId(oid);
  if (objectId === false) {
    objectId = mongodb.ObjectId(oid);
  }
  return mongodb.DBRef(namespace, objectId, db);
};

var Timestamp = function (high, low) {
...
```

#### <a name="apidoc.element.mongo-express.bson.toSafeBSON"></a>[function <span class="apidocSignatureSpan">mongo-express.bson.</span>toSafeBSON (string)](#apidoc.element.mongo-express.bson.toSafeBSON)
- description and source-code
```javascript
toSafeBSON = function (string) {
  try {
    var bsonObject = exports.toBSON(string);
    return bsonObject;
  } catch (err) {
    return null;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.bson.toString"></a>[function <span class="apidocSignatureSpan">mongo-express.bson.</span>toString (doc)](#apidoc.element.mongo-express.bson.toString)
- description and source-code
```javascript
toString = function (doc) {
  //Use custom json stringify function from json.js
  return json.stringify(doc, null, '    ');
}
```
- example usage
```shell
...
exports.json = function (input) {
return JSON.stringify(input, null, '    ');
};

exports.convertBytes = function (input) {
input = parseInt(input, 10);
if (input < 1024) {
  return input.toString() + ' Bytes';
} else if (input < 1024 * 1024) {
  //Convert to KB and keep 2 decimal values
  input = Math.round((input / 1024) * 100) / 100;
  return input.toString() + ' KB';
} else if (input < 1024 * 1024 * 1024) {
  input = Math.round((input / (1024 * 1024)) * 100) / 100;
  return input.toString() + ' MB';
...
```



# <a name="apidoc.module.mongo-express.filters"></a>[module mongo-express.filters](#apidoc.module.mongo-express.filters)

#### <a name="apidoc.element.mongo-express.filters.convertBytes"></a>[function <span class="apidocSignatureSpan">mongo-express.filters.</span>convertBytes (input)](#apidoc.element.mongo-express.filters.convertBytes)
- description and source-code
```javascript
convertBytes = function (input) {
  input = parseInt(input, 10);
  if (input < 1024) {
    return input.toString() + ' Bytes';
  } else if (input < 1024 * 1024) {
    //Convert to KB and keep 2 decimal values
    input = Math.round((input / 1024) * 100) / 100;
    return input.toString() + ' KB';
  } else if (input < 1024 * 1024 * 1024) {
    input = Math.round((input / (1024 * 1024)) * 100) / 100;
    return input.toString() + ' MB';
  } else if (input < 1024 * 1024 * 1024 * 1024) {
    input = Math.round((input / (1024 * 1024 * 1024)) * 100) / 100;
    return input.toString() + ' GB';
  } else if (input < 1024 * 1024 * 1024 * 1024 * 1024) {
    input = Math.round((input / (1024 * 1024 * 1024 * 1024)) * 100) / 100;
    return input.toString() + ' TB';
  } else {
    return input.toString() + ' Bytes';
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.filters.is_embeddedDocumentNotation"></a>[function <span class="apidocSignatureSpan">mongo-express.filters.</span>is_embeddedDocumentNotation (input)](#apidoc.element.mongo-express.filters.is_embeddedDocumentNotation)
- description and source-code
```javascript
is_embeddedDocumentNotation = function (input) {
  return /^(?:[a-zA-Z0-9_]+\.)+[a-zA-Z0-9_]+/.test(input);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.filters.json"></a>[function <span class="apidocSignatureSpan">mongo-express.filters.</span>json (input)](#apidoc.element.mongo-express.filters.json)
- description and source-code
```javascript
json = function (input) {
  return JSON.stringify(input, null, '    ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.filters.stringDocIDs"></a>[function <span class="apidocSignatureSpan">mongo-express.filters.</span>stringDocIDs (input)](#apidoc.element.mongo-express.filters.stringDocIDs)
- description and source-code
```javascript
stringDocIDs = function (input) {

  // Turns {_bsontype: ' ObjectID', id:12345... } into a plain string
  if (input && typeof input === 'object' && input._bsontype === 'ObjectID') {
    return input.toString();
  }

  return input;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.filters.to_display"></a>[function <span class="apidocSignatureSpan">mongo-express.filters.</span>to_display (input)](#apidoc.element.mongo-express.filters.to_display)
- description and source-code
```javascript
to_display = function (input) {

  var entifyGTLTAmp = function (text) {
    // Turn < ? > into HTML entities, so data doesn't get interpreted by the browser
    return text.replace(/&/g, '&amp;')
      .replace(/</g, '&lt;')
      .replace(/>/g, '&gt;')
      .replace(/"/g, '&quot;')
      .replace(/'/g, '&apos;');
  };

  var retHTML = '';

  // Get nulls out of the way
  if (input === null || input === undefined) {
    return '';
  }

  // Large property
  if (
    typeof input === 'object' &&
    input.display &&
    input.display === '*** LARGE PROPERTY ***' &&
    input.preview &&
    input.roughSz &&
    input.humanSz &&
    input.attribu &&
    input.maxSize &&
    input._id
  ) {
    retHTML += '<div class="tooDamnBig" doc_id="' + encodeURIComponent(JSON.stringify(input._id)) + '" ' +
      'doc_prop="' + input.attribu + '" title="Max prop size: ' + input.maxSize + '">';
    retHTML += input.display + '<br>~' + input.humanSz;
    retHTML += '<br>Preview:' + input.preview;
    retHTML += '<br>Click to fetch this property';
    retHTML += '</div>';
    return retHTML;
  }

  // Large row
  if (
    typeof input === 'object' &&
    input.display &&
    input.display === '*** LARGE ROW ***' &&
    input.preview &&
    input.roughSz &&
    input.humanSz &&
    input.attribu &&
    input.maxSize &&
    input._id
  ) {
    retHTML += '<div class="tooDamnBig" doc_id="' + encodeURIComponent(JSON.stringify(input._id)) + '" ' +
      'doc_prop="' + input.attribu + '" title="Max row size: ' + input.maxSize + '">';
    retHTML += input.display + '<br>' + input.attribu + ': ~' + input.humanSz;
    retHTML += '<br>Preview:' + input.preview;
    retHTML += '<br>Click to fetch this property';
    retHTML += '</div>';
    return retHTML;
  }

  // Images inline
  if (
    typeof input === 'string' &&
    (
      input.substr(0, 22) === 'data:image/png;base64,' ||
      input.substr(0, 22) === 'data:image/gif;base64,' ||
      input.substr(0, 22) === 'data:image/jpg;base64,' ||
      input.substr(0, 23) === 'data:image/jpeg;base64,'
    )
  )  {
    return '<img src="' + input + '" style="max-height:100%; max-width:100%; "/>';
  }

  // Audio inline
  if (
    typeof input === 'string' &&
    (
      input.substr(0, 22) === 'data:audio/ogg;base64,' ||
      input.substr(0, 22) === 'data:audio/mp3;base64,'
    )
  )  {
    return '<audio controls style="width:45px;" src="' + input + '">Your browser does not support the audio element.</audio>';
  }

  // Video inline
  if (
    typeof input === 'string' &&
    (
      input.substr(0, 23) === 'data:video/webm;base64,' ||
      input.substr(0, 22) === 'data:video/mp4;base64,'  ||
      input.substr(0, 22) === 'data:video/ogv;base64,'
    )
  )  {
    return '<video controls><source type="' + input.substring(input.indexOf(':') + 1, input.indexOf(';')) + '" src="' + input + '"/>' +
      'Your browser does not support the video element.</video>';
  }

  if (typeof input === 'object' && input.toString().substr(0, 15) === '[object Object]') {
    return '<pre>' + JSON.stringify(input, null, 2) + '</pre>';
  }

  // Concatenate long strings
  if (typeof input === 'string' && input.length > 50) {
    return entifyGTLTAmp(input.substr(0, 49) + '…');
  }

  // Return basic .toString() since we've tried all other cases
  return entifyGTLTAmp(input.toString());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.filters.to_string"></a>[function <span class="apidocSignatureSpan">mongo-express.filters.</span>to_string (input)](#apidoc.element.mongo-express.filters.to_string)
- description and source-code
```javascript
to_string = function (input) {
  return (input !== null && input !== undefined) ? input.toString() : '';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongo-express.json"></a>[module mongo-express.json](#apidoc.module.mongo-express.json)

#### <a name="apidoc.element.mongo-express.json.stringify"></a>[function <span class="apidocSignatureSpan">mongo-express.json.</span>stringify (value, replacer, space)](#apidoc.element.mongo-express.json.stringify)
- description and source-code
```javascript
stringify = function (value, replacer, space) {

  // The stringify method takes a value and an optional replacer, and an optional
  // space parameter, and returns a JSON text. The replacer can be a function
  // that can replace values, or an array of strings that will select the keys.
  // A default replacer method can be provided. Use of the space parameter can
  // produce text that is more easily readable.

  var i;
  gap = '';
  indent = '';

  // If the space parameter is a number, make an indent string containing that
  // many spaces.

  if (typeof space === 'number') {
    for (i = 0; i < space; i += 1) {
      indent += ' ';
    }

  // If the space parameter is a string, it will be used as the indent string.

  } else if (typeof space === 'string') {
    indent = space;
  }

  // If there is a replacer, it must be a function or an array.
  // Otherwise, throw an error.

  rep = replacer;
  if (replacer && typeof replacer !== 'function' &&
          (typeof replacer !== 'object' ||
          typeof replacer.length !== 'number')) {
    throw new Error('JSON.stringify');
  }

  // Make a fake root object containing our value under the key of ''.
  // Return the result of stringifying the value.

  return str('', { '': value });
}
```
- example usage
```shell
...
    console.log();
    console.error(clc.red('Address ' + addressString + ' already in use! You need to pick a different host and/or port.'));
    console.log('Maybe mongo-express is already running?');
  }

  console.log();
  console.log('If you are still having trouble, try Googling for the key parts of the following error object before posting an issue
');
  console.log(JSON.stringify(e));
  return process.exit(1);
});
...
```



# <a name="apidoc.module.mongo-express.utils"></a>[module mongo-express.utils](#apidoc.module.mongo-express.utils)

#### <a name="apidoc.element.mongo-express.utils.buildCollectionURL"></a>[function <span class="apidocSignatureSpan">mongo-express.utils.</span>buildCollectionURL (base, dbName, collectionName)](#apidoc.element.mongo-express.utils.buildCollectionURL)
- description and source-code
```javascript
buildCollectionURL = function (base, dbName, collectionName) {
  return base + 'db/' + dbName + '/' + encodeURIComponent(collectionName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.utils.bytesToSize"></a>[function <span class="apidocSignatureSpan">mongo-express.utils.</span>bytesToSize (bytes)](#apidoc.element.mongo-express.utils.bytesToSize)
- description and source-code
```javascript
function bytesToSize(bytes) {
  if (bytes === 0) return '0 Byte';
  var k = 1000;
  var sizes = ['Bytes', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB'];
  var i = Math.floor(Math.log(bytes) / Math.log(k));
  return (bytes / Math.pow(k, i)).toPrecision(3) + ' ' + sizes[i];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongo-express.utils.colsToGrid"></a>[function <span class="apidocSignatureSpan">mongo-express.utils.</span>colsToGrid (cols)](#apidoc.element.mongo-express.utils.colsToGrid)
- description and source-code
```javascript
colsToGrid = function (cols) {
  // Generate list of GridFS buckets
  // takes databases, filters by having suffix of '.files' and also a corresponding '.chunks' in the DB list, then returns just
the prefix name.

  // cols comes in an object of all databases and all their collections
  // return an object of all databases and all potential GridFS x.files & x.chunks

  var rets = _.clone(cols);

  _.each(rets, (val, key) => {
    rets[key] = _.map(
      _.filter(rets[key], col =>
        col.toString().substr(-6) === '.files' && _.intersection(rets[key], [col.toString().slice(0, -6) + '.chunks'])
      ),
      col => col.toString().slice(0, -6)
    ).sort();
  });

  return rets;
}
```
- example usage
```shell
...
  };

  // View helper, sets local variables used in templates
  appRouter.all('*', function (req, res, next) {
res.locals.baseHref       = buildBaseHref(req.originalUrl, req.url);
res.locals.databases      = mongo.databases;
res.locals.collections    = mongo.collections;
res.locals.gridFSBuckets  = utils.colsToGrid(mongo.collections);

// Flash messages
if (req.session.success) {
  res.locals.messageSuccess = req.session.success;
  delete req.session.success;
}
...
```

#### <a name="apidoc.element.mongo-express.utils.deepmerge"></a>[function <span class="apidocSignatureSpan">mongo-express.utils.</span>deepmerge (target, src)](#apidoc.element.mongo-express.utils.deepmerge)
- description and source-code
```javascript
deepmerge = function (target, src) {
  var array = Array.isArray(src);
  var dst = array ? [] : {};

  if (array) {
    target = target || [];
    dst = dst.concat(target);
    src.forEach(function (e, i) {
      if (typeof dst[i] === 'undefined') {
        dst[i] = e;
      } else if (typeof e === 'object') {
        dst[i] = exports.deepmerge(target[i], e);
      } else {
        if (target.indexOf(e) === -1) {
          dst.push(e);
        }
      }
    });
  } else {
    if (target && typeof target === 'object') {
      Object.keys(target).forEach(function (key) {
        dst[key] = target[key];
      });
    }

    Object.keys(src).forEach(function (key) {
      if (typeof src[key] !== 'object' || !src[key]) {
        dst[key] = src[key];
      } else {
        if (!target[key]) {
          dst[key] = src[key];
        } else {
          dst[key] = exports.deepmerge(target[key], src[key]);
        }
      }
    });
  }

  return dst;
}
```
- example usage
```shell
...
let sslOptions;

// Notify of any updates
notifier.notify();

try {
// eslint-disable-next-line import/no-unresolved
config = utils.deepmerge(require('./config.default'), require('./config'));
} catch (e) {
if (e.code === 'MODULE_NOT_FOUND') {
  console.log('No custom config.js found, loading config.default.js');
} else {
  console.error(clc.red('Unable to load config.js!'));
  console.error(clc.red('Error is:'));
  console.log(clc.red(e));
...
```

#### <a name="apidoc.element.mongo-express.utils.roughSizeOfObject"></a>[function <span class="apidocSignatureSpan">mongo-express.utils.</span>roughSizeOfObject (object)](#apidoc.element.mongo-express.utils.roughSizeOfObject)
- description and source-code
```javascript
roughSizeOfObject = function (object) {

  var objectList = [];
  var recurse = function (value) {
    var bytes = 0;

    if (typeof value === 'boolean') {
      bytes = 4;
    } else if (typeof value === 'string') {
      bytes = value.length * 2;
    } else if (typeof value === 'number') {
      bytes = 8;
    } else if (typeof value === 'object' && objectList.indexOf(value) === -1) {
      objectList[objectList.length] = value;

      for (var i in value) {
        bytes += 8; // an assumed existence overhead
        bytes += recurse(value[i]);
      }
    }

    return bytes;
  };

  return recurse(object);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
