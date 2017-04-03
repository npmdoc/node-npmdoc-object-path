# api documentation for  [object-path (v0.11.4)](https://github.com/mariocasciaro/object-path)  [![npm package](https://img.shields.io/npm/v/npmdoc-object-path.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-object-path) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-object-path.svg)](https://travis-ci.org/npmdoc/node-npmdoc-object-path)
#### Access deep object properties using a path

[![NPM](https://nodei.co/npm/object-path.png?downloads=true)](https://www.npmjs.com/package/object-path)

[![apidoc](https://npmdoc.github.io/node-npmdoc-object-path/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-object-path_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-object-path/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-object-path/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-object-path/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mario Casciaro"
    },
    "bugs": {
        "url": "https://github.com/mariocasciaro/object-path/issues"
    },
    "dependencies": {},
    "description": "Access deep object properties using a path",
    "devDependencies": {
        "@mariocasciaro/benchpress": "^0.1.3",
        "chai": "^3.5.0",
        "coveralls": "^2.11.2",
        "istanbul": "^0.4.4",
        "mocha": "^2.2.4",
        "mocha-lcov-reporter": "^1.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "370ae752fbf37de3ea70a861c23bba8915691949",
        "tarball": "https://registry.npmjs.org/object-path/-/object-path-0.11.4.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "99d9d30087493f6def258ddfb45d34029f5ce4eb",
    "homepage": "https://github.com/mariocasciaro/object-path",
    "keywords": [
        "deep",
        "path",
        "access",
        "bean",
        "get",
        "property",
        "dot",
        "prop",
        "object",
        "obj",
        "notation",
        "segment",
        "value",
        "nested",
        "key"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "mariocasciaro",
            "email": "mariocasciaro@gmail.com"
        }
    ],
    "name": "object-path",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/mariocasciaro/object-path.git"
    },
    "scripts": {
        "test": "istanbul cover ./node_modules/mocha/bin/_mocha test.js --report html -- -R spec"
    },
    "version": "0.11.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module object-path](#apidoc.module.object-path)
1.  [function <span class="apidocSignatureSpan">object-path.</span>coalesce (obj, paths, defaultValue)](#apidoc.element.object-path.coalesce)
1.  [function <span class="apidocSignatureSpan">object-path.</span>create (options)](#apidoc.element.object-path.create)
1.  [function <span class="apidocSignatureSpan">object-path.</span>del (obj, path)](#apidoc.element.object-path.del)
1.  [function <span class="apidocSignatureSpan">object-path.</span>empty (obj, path)](#apidoc.element.object-path.empty)
1.  [function <span class="apidocSignatureSpan">object-path.</span>ensureExists (obj, path, value)](#apidoc.element.object-path.ensureExists)
1.  [function <span class="apidocSignatureSpan">object-path.</span>get (obj, path, defaultValue)](#apidoc.element.object-path.get)
1.  [function <span class="apidocSignatureSpan">object-path.</span>has (obj, path)](#apidoc.element.object-path.has)
1.  [function <span class="apidocSignatureSpan">object-path.</span>insert (obj, path, value, at)](#apidoc.element.object-path.insert)
1.  [function <span class="apidocSignatureSpan">object-path.</span>push (obj, path)](#apidoc.element.object-path.push)
1.  [function <span class="apidocSignatureSpan">object-path.</span>set (obj, path, value, doNotReplace)](#apidoc.element.object-path.set)
1.  [function <span class="apidocSignatureSpan">object-path.</span>withInheritedProps (obj)](#apidoc.element.object-path.withInheritedProps)

#### [module object-path.withInheritedProps](#apidoc.module.object-path.withInheritedProps)
1.  [function <span class="apidocSignatureSpan">object-path.</span>withInheritedProps (obj)](#apidoc.element.object-path.withInheritedProps.withInheritedProps)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>coalesce (obj, paths, defaultValue)](#apidoc.element.object-path.withInheritedProps.coalesce)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>del (obj, path)](#apidoc.element.object-path.withInheritedProps.del)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>empty (obj, path)](#apidoc.element.object-path.withInheritedProps.empty)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>ensureExists (obj, path, value)](#apidoc.element.object-path.withInheritedProps.ensureExists)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>get (obj, path, defaultValue)](#apidoc.element.object-path.withInheritedProps.get)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>has (obj, path)](#apidoc.element.object-path.withInheritedProps.has)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>insert (obj, path, value, at)](#apidoc.element.object-path.withInheritedProps.insert)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>push (obj, path)](#apidoc.element.object-path.withInheritedProps.push)
1.  [function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>set (obj, path, value, doNotReplace)](#apidoc.element.object-path.withInheritedProps.set)



# <a name="apidoc.module.object-path"></a>[module object-path](#apidoc.module.object-path)

#### <a name="apidoc.element.object-path.coalesce"></a>[function <span class="apidocSignatureSpan">object-path.</span>coalesce (obj, paths, defaultValue)](#apidoc.element.object-path.coalesce)
- description and source-code
```javascript
coalesce = function (obj, paths, defaultValue) {
  var value;

  for (var i = 0, len = paths.length; i < len; i++) {
    if ((value = objectPath.get(obj, paths[i])) !== void 0) {
      return value;
    }
  }

  return defaultValue;
}
```
- example usage
```shell
...

//get deep property
objectPath.get(obj, "a.b");  //returns "d"
objectPath.get(obj, ["a", "dot.dot"]);  //returns "key"
objectPath.get(obj, 'a.\u1200');  //returns "unicode key"

//get the first non-undefined value
objectPath.coalesce(obj, ['a.z', 'a.d', ['a','b']], 'default');

//empty a given path (but do not delete it) depending on their type,so it retains reference to objects and arrays.
//functions that are not inherited from prototype are set to null.
//object instances are considered objects and just own property names are deleted
objectPath.empty(obj, 'a.b'); // obj.a.b is now ''
objectPath.empty(obj, 'a.c'); // obj.a.c is now []
objectPath.empty(obj, 'a'); // obj.a is now {}
...
```

#### <a name="apidoc.element.object-path.create"></a>[function <span class="apidocSignatureSpan">object-path.</span>create (options)](#apidoc.element.object-path.create)
- description and source-code
```javascript
function factory(options) {
  options = options || {}

  var objectPath = function(obj) {
    return Object.keys(objectPath).reduce(function(proxy, prop) {
      if(prop === 'create') {
        return proxy;
      }

<span class="apidocCodeCommentSpan">      /*istanbul ignore else*/
</span>      if (typeof objectPath[prop] === 'function') {
        proxy[prop] = objectPath[prop].bind(objectPath, obj);
      }

      return proxy;
    }, {});
  };

  function hasShallowProperty(obj, prop) {
    return (options.includeInheritedProps || (typeof prop === 'number' && Array.isArray(obj)) || hasOwnProperty(obj, prop))
  }

  function getShallowProperty(obj, prop) {
    if (hasShallowProperty(obj, prop)) {
      return obj[prop];
    }
  }

  function set(obj, path, value, doNotReplace){
    if (typeof path === 'number') {
      path = [path];
    }
    if (!path || path.length === 0) {
      return obj;
    }
    if (typeof path === 'string') {
      return set(obj, path.split('.').map(getKey), value, doNotReplace);
    }
    var currentPath = path[0];
    var currentValue = getShallowProperty(obj, currentPath);
    if (path.length === 1) {
      if (currentValue === void 0 || !doNotReplace) {
        obj[currentPath] = value;
      }
      return currentValue;
    }

    if (currentValue === void 0) {
      //check if we assume an array
      if(typeof path[1] === 'number') {
        obj[currentPath] = [];
      } else {
        obj[currentPath] = {};
      }
    }

    return set(obj[currentPath], path.slice(1), value, doNotReplace);
  }

  objectPath.has = function (obj, path) {
    if (typeof path === 'number') {
      path = [path];
    } else if (typeof path === 'string') {
      path = path.split('.');
    }

    if (!path || path.length === 0) {
      return !!obj;
    }

    for (var i = 0; i < path.length; i++) {
      var j = getKey(path[i]);

      if((typeof j === 'number' && isArray(obj) && j < obj.length) ||
        (options.includeInheritedProps ? (j in Object(obj)) : hasOwnProperty(obj, j))) {
        obj = obj[j];
      } else {
        return false;
      }
    }

    return true;
  };

  objectPath.ensureExists = function (obj, path, value){
    return set(obj, path, value, true);
  };

  objectPath.set = function (obj, path, value, doNotReplace){
    return set(obj, path, value, doNotReplace);
  };

  objectPath.insert = function (obj, path, value, at){
    var arr = objectPath.get(obj, path);
    at = ~~at;
    if (!isArray(arr)) {
      arr = [];
      objectPath.set(obj, path, arr);
    }
    arr.splice(at, 0, value);
  };

  objectPath.empty = function(obj, path) {
    if (isEmpty(path)) {
      return void 0;
    }
    if (obj == null) {
      return void 0;
    }

    var value, i;
    if (!(value = objectPath.get(obj, path))) {
      return void 0;
    }

    if (typeof value === 'string') {
      return objectPath.set(obj, path, '');
    } else if (isBoolean(value)) {
      return objectPath.set(obj, path, false);
    } else if (typeof value === 'number') {
      return objectPath.set(obj, path, 0);
    } else if (isArray(value)) {
      value.length = 0;
    } else if (isObject(value)) {
      for (i in value) {
        if (hasShallowProperty(value, i)) {
          delete value[i];
        }
      }
    } else {
      return objectPath.set(obj, path, null);
    }
  };

  objectPath.push = function (obj, path /*, values */){
    var arr = objectPath.get(obj, path);
    if (!isArray(arr)) {
      arr = [];
      objectPath.set(obj, path, arr);
    }

    arr.push.apply(arr, Array.prototype.slice.call(arguments, 2));
  };

  objectPath.coalesce = function (obj, paths, defaultValue) {
    var value;

    for (var i = 0, len = paths.length; i < len; i++) {
      if ((value = objectPath.get(obj, paths[i])) !== void 0) {
        return value;
      }
    }

    return defaultValue;
  };

  objectPath.get = function (obj, path, defaultValue){
    if (typeof path === 'number') {
      path = [path];
    }
    if (!path || path.length === 0) {
      return obj;
    }
    if (obj == null) {
      return defaultValue;
    }
    if (typeof path === 'str ...
```
- example usage
```shell
...

By default 'object-path' will only access an object's own properties. Look at the following example:

'''javascript
var proto = {
  notOwn: {prop: 'a'}
}
var obj = Object.create(proto);

//This will return undefined (or the default value you specified), because notOwn is
//an inherited property
objectPath.get(obj, 'notOwn.prop');

//This will set the property on the obj instance and not the prototype.
//In other words proto.notOwn.prop === 'a' and obj.notOwn.prop === 'b'
...
```

#### <a name="apidoc.element.object-path.del"></a>[function <span class="apidocSignatureSpan">object-path.</span>del (obj, path)](#apidoc.element.object-path.del)
- description and source-code
```javascript
function del(obj, path) {
  if (typeof path === 'number') {
    path = [path];
  }

  if (obj == null) {
    return obj;
  }

  if (isEmpty(path)) {
    return obj;
  }
  if(typeof path === 'string') {
    return objectPath.del(obj, path.split('.'));
  }

  var currentPath = getKey(path[0]);
  if (!hasShallowProperty(obj, currentPath)) {
    return obj;
  }

  if(path.length === 1) {
    if (isArray(obj)) {
      obj.splice(currentPath, 1);
    } else {
      delete obj[currentPath];
    }
  } else {
    return objectPath.del(obj[currentPath], path.slice(1));
  }

  return obj;
}
```
- example usage
```shell
...
objectPath.push(obj, "a.k", "o");

//ensure a path exists (if it doesn't, set the default value you provide)
objectPath.ensureExists(obj, "a.k.1", "DEFAULT");
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"

//deletes a path
objectPath.del(obj, "a.b"); // obj.a.b is now undefined
objectPath.del(obj, ["a","c",0]); // obj.a.c is now ['f']

//tests path existence
objectPath.has(obj, "a.b"); // true
objectPath.has(obj, ["a","d"]); // false

//bind object
...
```

#### <a name="apidoc.element.object-path.empty"></a>[function <span class="apidocSignatureSpan">object-path.</span>empty (obj, path)](#apidoc.element.object-path.empty)
- description and source-code
```javascript
empty = function (obj, path) {
  if (isEmpty(path)) {
    return void 0;
  }
  if (obj == null) {
    return void 0;
  }

  var value, i;
  if (!(value = objectPath.get(obj, path))) {
    return void 0;
  }

  if (typeof value === 'string') {
    return objectPath.set(obj, path, '');
  } else if (isBoolean(value)) {
    return objectPath.set(obj, path, false);
  } else if (typeof value === 'number') {
    return objectPath.set(obj, path, 0);
  } else if (isArray(value)) {
    value.length = 0;
  } else if (isObject(value)) {
    for (i in value) {
      if (hasShallowProperty(value, i)) {
        delete value[i];
      }
    }
  } else {
    return objectPath.set(obj, path, null);
  }
}
```
- example usage
```shell
...

//get the first non-undefined value
objectPath.coalesce(obj, ['a.z', 'a.d', ['a','b']], 'default');

//empty a given path (but do not delete it) depending on their type,so it retains reference to objects and arrays.
//functions that are not inherited from prototype are set to null.
//object instances are considered objects and just own property names are deleted
objectPath.empty(obj, 'a.b'); // obj.a.b is now ''
objectPath.empty(obj, 'a.c'); // obj.a.c is now []
objectPath.empty(obj, 'a'); // obj.a is now {}

//works also with arrays
objectPath.get(obj, "a.c.1");  //returns "f"
objectPath.get(obj, ["a","c","1"]);  //returns "f"
...
```

#### <a name="apidoc.element.object-path.ensureExists"></a>[function <span class="apidocSignatureSpan">object-path.</span>ensureExists (obj, path, value)](#apidoc.element.object-path.ensureExists)
- description and source-code
```javascript
ensureExists = function (obj, path, value){
  return set(obj, path, value, true);
}
```
- example usage
```shell
...
//will insert values in array
objectPath.insert(obj, "a.c", "m", 1); // obj.a.c = ["e", "m", "f"]

//push into arrays (and create intermediate objects/arrays)
objectPath.push(obj, "a.k", "o");

//ensure a path exists (if it doesn't, set the default value you provide)
objectPath.ensureExists(obj, "a.k.1", "DEFAULT");
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"

//deletes a path
objectPath.del(obj, "a.b"); // obj.a.b is now undefined
objectPath.del(obj, ["a","c",0]); // obj.a.c is now ['f']

//tests path existence
...
```

#### <a name="apidoc.element.object-path.get"></a>[function <span class="apidocSignatureSpan">object-path.</span>get (obj, path, defaultValue)](#apidoc.element.object-path.get)
- description and source-code
```javascript
get = function (obj, path, defaultValue){
  if (typeof path === 'number') {
    path = [path];
  }
  if (!path || path.length === 0) {
    return obj;
  }
  if (obj == null) {
    return defaultValue;
  }
  if (typeof path === 'string') {
    return objectPath.get(obj, path.split('.'), defaultValue);
  }

  var currentPath = getKey(path[0]);
  var nextObj = getShallowProperty(obj, currentPath)
  if (nextObj === void 0) {
    return defaultValue;
  }

  if (path.length === 1) {
    return nextObj;
  }

  return objectPath.get(obj[currentPath], path.slice(1), defaultValue);
}
```
- example usage
```shell
...
    'dot.dot': 'key'
  }
};

var objectPath = require("object-path");

//get deep property
objectPath.get(obj, "a.b");  //returns "d"
objectPath.get(obj, ["a", "dot.dot"]);  //returns "key"
objectPath.get(obj, 'a.\u1200');  //returns "unicode key"

//get the first non-undefined value
objectPath.coalesce(obj, ['a.z', 'a.d', ['a','b']], 'default');

//empty a given path (but do not delete it) depending on their type,so it retains reference to objects and arrays.
...
```

#### <a name="apidoc.element.object-path.has"></a>[function <span class="apidocSignatureSpan">object-path.</span>has (obj, path)](#apidoc.element.object-path.has)
- description and source-code
```javascript
has = function (obj, path) {
  if (typeof path === 'number') {
    path = [path];
  } else if (typeof path === 'string') {
    path = path.split('.');
  }

  if (!path || path.length === 0) {
    return !!obj;
  }

  for (var i = 0; i < path.length; i++) {
    var j = getKey(path[i]);

    if((typeof j === 'number' && isArray(obj) && j < obj.length) ||
      (options.includeInheritedProps ? (j in Object(obj)) : hasOwnProperty(obj, j))) {
      obj = obj[j];
    } else {
      return false;
    }
  }

  return true;
}
```
- example usage
```shell
...
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"

//deletes a path
objectPath.del(obj, "a.b"); // obj.a.b is now undefined
objectPath.del(obj, ["a","c",0]); // obj.a.c is now ['f']

//tests path existence
objectPath.has(obj, "a.b"); // true
objectPath.has(obj, ["a","d"]); // false

//bind object
var model = objectPath({
a: {
  b: "d",
  c: ["e", "f"]
...
```

#### <a name="apidoc.element.object-path.insert"></a>[function <span class="apidocSignatureSpan">object-path.</span>insert (obj, path, value, at)](#apidoc.element.object-path.insert)
- description and source-code
```javascript
insert = function (obj, path, value, at){
  var arr = objectPath.get(obj, path);
  at = ~~at;
  if (!isArray(arr)) {
    arr = [];
    objectPath.set(obj, path, arr);
  }
  arr.splice(at, 0, value);
}
```
- example usage
```shell
...
objectPath.set(obj, "a.h", "m"); // or objectPath.set(obj, ["a","h"], "m");
objectPath.get(obj, "a.h");  //returns "m"

//set will create intermediate object/arrays
objectPath.set(obj, "a.j.0.f", "m");

//will insert values in array
objectPath.insert(obj, "a.c", "m", 1); // obj.a.c = ["e", "m", "f"]

//push into arrays (and create intermediate objects/arrays)
objectPath.push(obj, "a.k", "o");

//ensure a path exists (if it doesn't, set the default value you provide)
objectPath.ensureExists(obj, "a.k.1", "DEFAULT");
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"
...
```

#### <a name="apidoc.element.object-path.push"></a>[function <span class="apidocSignatureSpan">object-path.</span>push (obj, path)](#apidoc.element.object-path.push)
- description and source-code
```javascript
push = function (obj, path){
  var arr = objectPath.get(obj, path);
  if (!isArray(arr)) {
    arr = [];
    objectPath.set(obj, path, arr);
  }

  arr.push.apply(arr, Array.prototype.slice.call(arguments, 2));
}
```
- example usage
```shell
...
//set will create intermediate object/arrays
objectPath.set(obj, "a.j.0.f", "m");

//will insert values in array
objectPath.insert(obj, "a.c", "m", 1); // obj.a.c = ["e", "m", "f"]

//push into arrays (and create intermediate objects/arrays)
objectPath.push(obj, "a.k", "o");

//ensure a path exists (if it doesn't, set the default value you provide)
objectPath.ensureExists(obj, "a.k.1", "DEFAULT");
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"

//deletes a path
objectPath.del(obj, "a.b"); // obj.a.b is now undefined
...
```

#### <a name="apidoc.element.object-path.set"></a>[function <span class="apidocSignatureSpan">object-path.</span>set (obj, path, value, doNotReplace)](#apidoc.element.object-path.set)
- description and source-code
```javascript
set = function (obj, path, value, doNotReplace){
  return set(obj, path, value, doNotReplace);
}
```
- example usage
```shell
...
objectPath.get(obj, "a.c.1");  //returns "f"
objectPath.get(obj, ["a","c","1"]);  //returns "f"

//can return a default value with get
objectPath.get(obj, ["a.c.b"], "DEFAULT");  //returns "DEFAULT", since a.c.b path doesn't exists, if omitted, returns undefined

//set
objectPath.set(obj, "a.h", "m"); // or objectPath.set(obj, ["a","h"], "m");
objectPath.get(obj, "a.h");  //returns "m"

//set will create intermediate object/arrays
objectPath.set(obj, "a.j.0.f", "m");

//will insert values in array
objectPath.insert(obj, "a.c", "m", 1); // obj.a.c = ["e", "m", "f"]
...
```

#### <a name="apidoc.element.object-path.withInheritedProps"></a>[function <span class="apidocSignatureSpan">object-path.</span>withInheritedProps (obj)](#apidoc.element.object-path.withInheritedProps)
- description and source-code
```javascript
withInheritedProps = function (obj) {
  return Object.keys(objectPath).reduce(function(proxy, prop) {
    if(prop === 'create') {
      return proxy;
    }

<span class="apidocCodeCommentSpan">    /*istanbul ignore else*/
</span>    if (typeof objectPath[prop] === 'function') {
      proxy[prop] = objectPath[prop].bind(objectPath, obj);
    }

    return proxy;
  }, {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.object-path.withInheritedProps"></a>[module object-path.withInheritedProps](#apidoc.module.object-path.withInheritedProps)

#### <a name="apidoc.element.object-path.withInheritedProps.withInheritedProps"></a>[function <span class="apidocSignatureSpan">object-path.</span>withInheritedProps (obj)](#apidoc.element.object-path.withInheritedProps.withInheritedProps)
- description and source-code
```javascript
withInheritedProps = function (obj) {
  return Object.keys(objectPath).reduce(function(proxy, prop) {
    if(prop === 'create') {
      return proxy;
    }

<span class="apidocCodeCommentSpan">    /*istanbul ignore else*/
</span>    if (typeof objectPath[prop] === 'function') {
      proxy[prop] = objectPath[prop].bind(objectPath, obj);
    }

    return proxy;
  }, {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.object-path.withInheritedProps.coalesce"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>coalesce (obj, paths, defaultValue)](#apidoc.element.object-path.withInheritedProps.coalesce)
- description and source-code
```javascript
coalesce = function (obj, paths, defaultValue) {
  var value;

  for (var i = 0, len = paths.length; i < len; i++) {
    if ((value = objectPath.get(obj, paths[i])) !== void 0) {
      return value;
    }
  }

  return defaultValue;
}
```
- example usage
```shell
...

//get deep property
objectPath.get(obj, "a.b");  //returns "d"
objectPath.get(obj, ["a", "dot.dot"]);  //returns "key"
objectPath.get(obj, 'a.\u1200');  //returns "unicode key"

//get the first non-undefined value
objectPath.coalesce(obj, ['a.z', 'a.d', ['a','b']], 'default');

//empty a given path (but do not delete it) depending on their type,so it retains reference to objects and arrays.
//functions that are not inherited from prototype are set to null.
//object instances are considered objects and just own property names are deleted
objectPath.empty(obj, 'a.b'); // obj.a.b is now ''
objectPath.empty(obj, 'a.c'); // obj.a.c is now []
objectPath.empty(obj, 'a'); // obj.a is now {}
...
```

#### <a name="apidoc.element.object-path.withInheritedProps.del"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>del (obj, path)](#apidoc.element.object-path.withInheritedProps.del)
- description and source-code
```javascript
function del(obj, path) {
  if (typeof path === 'number') {
    path = [path];
  }

  if (obj == null) {
    return obj;
  }

  if (isEmpty(path)) {
    return obj;
  }
  if(typeof path === 'string') {
    return objectPath.del(obj, path.split('.'));
  }

  var currentPath = getKey(path[0]);
  if (!hasShallowProperty(obj, currentPath)) {
    return obj;
  }

  if(path.length === 1) {
    if (isArray(obj)) {
      obj.splice(currentPath, 1);
    } else {
      delete obj[currentPath];
    }
  } else {
    return objectPath.del(obj[currentPath], path.slice(1));
  }

  return obj;
}
```
- example usage
```shell
...
objectPath.push(obj, "a.k", "o");

//ensure a path exists (if it doesn't, set the default value you provide)
objectPath.ensureExists(obj, "a.k.1", "DEFAULT");
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"

//deletes a path
objectPath.del(obj, "a.b"); // obj.a.b is now undefined
objectPath.del(obj, ["a","c",0]); // obj.a.c is now ['f']

//tests path existence
objectPath.has(obj, "a.b"); // true
objectPath.has(obj, ["a","d"]); // false

//bind object
...
```

#### <a name="apidoc.element.object-path.withInheritedProps.empty"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>empty (obj, path)](#apidoc.element.object-path.withInheritedProps.empty)
- description and source-code
```javascript
empty = function (obj, path) {
  if (isEmpty(path)) {
    return void 0;
  }
  if (obj == null) {
    return void 0;
  }

  var value, i;
  if (!(value = objectPath.get(obj, path))) {
    return void 0;
  }

  if (typeof value === 'string') {
    return objectPath.set(obj, path, '');
  } else if (isBoolean(value)) {
    return objectPath.set(obj, path, false);
  } else if (typeof value === 'number') {
    return objectPath.set(obj, path, 0);
  } else if (isArray(value)) {
    value.length = 0;
  } else if (isObject(value)) {
    for (i in value) {
      if (hasShallowProperty(value, i)) {
        delete value[i];
      }
    }
  } else {
    return objectPath.set(obj, path, null);
  }
}
```
- example usage
```shell
...

//get the first non-undefined value
objectPath.coalesce(obj, ['a.z', 'a.d', ['a','b']], 'default');

//empty a given path (but do not delete it) depending on their type,so it retains reference to objects and arrays.
//functions that are not inherited from prototype are set to null.
//object instances are considered objects and just own property names are deleted
objectPath.empty(obj, 'a.b'); // obj.a.b is now ''
objectPath.empty(obj, 'a.c'); // obj.a.c is now []
objectPath.empty(obj, 'a'); // obj.a is now {}

//works also with arrays
objectPath.get(obj, "a.c.1");  //returns "f"
objectPath.get(obj, ["a","c","1"]);  //returns "f"
...
```

#### <a name="apidoc.element.object-path.withInheritedProps.ensureExists"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>ensureExists (obj, path, value)](#apidoc.element.object-path.withInheritedProps.ensureExists)
- description and source-code
```javascript
ensureExists = function (obj, path, value){
  return set(obj, path, value, true);
}
```
- example usage
```shell
...
//will insert values in array
objectPath.insert(obj, "a.c", "m", 1); // obj.a.c = ["e", "m", "f"]

//push into arrays (and create intermediate objects/arrays)
objectPath.push(obj, "a.k", "o");

//ensure a path exists (if it doesn't, set the default value you provide)
objectPath.ensureExists(obj, "a.k.1", "DEFAULT");
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"

//deletes a path
objectPath.del(obj, "a.b"); // obj.a.b is now undefined
objectPath.del(obj, ["a","c",0]); // obj.a.c is now ['f']

//tests path existence
...
```

#### <a name="apidoc.element.object-path.withInheritedProps.get"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>get (obj, path, defaultValue)](#apidoc.element.object-path.withInheritedProps.get)
- description and source-code
```javascript
get = function (obj, path, defaultValue){
  if (typeof path === 'number') {
    path = [path];
  }
  if (!path || path.length === 0) {
    return obj;
  }
  if (obj == null) {
    return defaultValue;
  }
  if (typeof path === 'string') {
    return objectPath.get(obj, path.split('.'), defaultValue);
  }

  var currentPath = getKey(path[0]);
  var nextObj = getShallowProperty(obj, currentPath)
  if (nextObj === void 0) {
    return defaultValue;
  }

  if (path.length === 1) {
    return nextObj;
  }

  return objectPath.get(obj[currentPath], path.slice(1), defaultValue);
}
```
- example usage
```shell
...
    'dot.dot': 'key'
  }
};

var objectPath = require("object-path");

//get deep property
objectPath.get(obj, "a.b");  //returns "d"
objectPath.get(obj, ["a", "dot.dot"]);  //returns "key"
objectPath.get(obj, 'a.\u1200');  //returns "unicode key"

//get the first non-undefined value
objectPath.coalesce(obj, ['a.z', 'a.d', ['a','b']], 'default');

//empty a given path (but do not delete it) depending on their type,so it retains reference to objects and arrays.
...
```

#### <a name="apidoc.element.object-path.withInheritedProps.has"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>has (obj, path)](#apidoc.element.object-path.withInheritedProps.has)
- description and source-code
```javascript
has = function (obj, path) {
  if (typeof path === 'number') {
    path = [path];
  } else if (typeof path === 'string') {
    path = path.split('.');
  }

  if (!path || path.length === 0) {
    return !!obj;
  }

  for (var i = 0; i < path.length; i++) {
    var j = getKey(path[i]);

    if((typeof j === 'number' && isArray(obj) && j < obj.length) ||
      (options.includeInheritedProps ? (j in Object(obj)) : hasOwnProperty(obj, j))) {
      obj = obj[j];
    } else {
      return false;
    }
  }

  return true;
}
```
- example usage
```shell
...
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"

//deletes a path
objectPath.del(obj, "a.b"); // obj.a.b is now undefined
objectPath.del(obj, ["a","c",0]); // obj.a.c is now ['f']

//tests path existence
objectPath.has(obj, "a.b"); // true
objectPath.has(obj, ["a","d"]); // false

//bind object
var model = objectPath({
a: {
  b: "d",
  c: ["e", "f"]
...
```

#### <a name="apidoc.element.object-path.withInheritedProps.insert"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>insert (obj, path, value, at)](#apidoc.element.object-path.withInheritedProps.insert)
- description and source-code
```javascript
insert = function (obj, path, value, at){
  var arr = objectPath.get(obj, path);
  at = ~~at;
  if (!isArray(arr)) {
    arr = [];
    objectPath.set(obj, path, arr);
  }
  arr.splice(at, 0, value);
}
```
- example usage
```shell
...
objectPath.set(obj, "a.h", "m"); // or objectPath.set(obj, ["a","h"], "m");
objectPath.get(obj, "a.h");  //returns "m"

//set will create intermediate object/arrays
objectPath.set(obj, "a.j.0.f", "m");

//will insert values in array
objectPath.insert(obj, "a.c", "m", 1); // obj.a.c = ["e", "m", "f"]

//push into arrays (and create intermediate objects/arrays)
objectPath.push(obj, "a.k", "o");

//ensure a path exists (if it doesn't, set the default value you provide)
objectPath.ensureExists(obj, "a.k.1", "DEFAULT");
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"
...
```

#### <a name="apidoc.element.object-path.withInheritedProps.push"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>push (obj, path)](#apidoc.element.object-path.withInheritedProps.push)
- description and source-code
```javascript
push = function (obj, path){
  var arr = objectPath.get(obj, path);
  if (!isArray(arr)) {
    arr = [];
    objectPath.set(obj, path, arr);
  }

  arr.push.apply(arr, Array.prototype.slice.call(arguments, 2));
}
```
- example usage
```shell
...
//set will create intermediate object/arrays
objectPath.set(obj, "a.j.0.f", "m");

//will insert values in array
objectPath.insert(obj, "a.c", "m", 1); // obj.a.c = ["e", "m", "f"]

//push into arrays (and create intermediate objects/arrays)
objectPath.push(obj, "a.k", "o");

//ensure a path exists (if it doesn't, set the default value you provide)
objectPath.ensureExists(obj, "a.k.1", "DEFAULT");
var oldVal = objectPath.ensureExists(obj, "a.b", "DEFAULT"); // oldval === "d"

//deletes a path
objectPath.del(obj, "a.b"); // obj.a.b is now undefined
...
```

#### <a name="apidoc.element.object-path.withInheritedProps.set"></a>[function <span class="apidocSignatureSpan">object-path.withInheritedProps.</span>set (obj, path, value, doNotReplace)](#apidoc.element.object-path.withInheritedProps.set)
- description and source-code
```javascript
set = function (obj, path, value, doNotReplace){
  return set(obj, path, value, doNotReplace);
}
```
- example usage
```shell
...
objectPath.get(obj, "a.c.1");  //returns "f"
objectPath.get(obj, ["a","c","1"]);  //returns "f"

//can return a default value with get
objectPath.get(obj, ["a.c.b"], "DEFAULT");  //returns "DEFAULT", since a.c.b path doesn't exists, if omitted, returns undefined

//set
objectPath.set(obj, "a.h", "m"); // or objectPath.set(obj, ["a","h"], "m");
objectPath.get(obj, "a.h");  //returns "m"

//set will create intermediate object/arrays
objectPath.set(obj, "a.j.0.f", "m");

//will insert values in array
objectPath.insert(obj, "a.c", "m", 1); // obj.a.c = ["e", "m", "f"]
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
