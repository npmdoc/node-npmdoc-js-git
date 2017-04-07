# api documentation for  [js-git (v0.7.8)](https://github.com/creationix/js-git#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-js-git.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-js-git) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-js-git.svg)](https://travis-ci.org/npmdoc/node-npmdoc-js-git)
#### Git Implemented in JavaScript

[![NPM](https://nodei.co/npm/js-git.png?downloads=true)](https://www.npmjs.com/package/js-git)

[![apidoc](https://npmdoc.github.io/node-npmdoc-js-git/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-js-git_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-js-git/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-js-git/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-js-git/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tim Caswell",
        "email": "tim@creationix.com"
    },
    "bugs": {
        "url": "https://github.com/creationix/js-git/issues"
    },
    "dependencies": {
        "bodec": "^0.1.0",
        "culvert": "^0.1.2",
        "git-sha1": "^0.1.2",
        "pako": "^0.2.5"
    },
    "description": "Git Implemented in JavaScript",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "52fa655ab61877d6f1079efc6534b554f31e5444",
        "tarball": "https://registry.npmjs.org/js-git/-/js-git-0.7.8.tgz"
    },
    "gitHead": "d78da0138969a368da74d0dfb9e3c5d88114b152",
    "homepage": "https://github.com/creationix/js-git#readme",
    "keywords": [
        "git",
        "js-git"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "creationix",
            "email": "tim@creationix.com"
        }
    ],
    "name": "js-git",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/creationix/js-git.git"
    },
    "scripts": {
        "test": "ls test/test-* | xargs -n1 node"
    },
    "version": "0.7.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module js-git](#apidoc.module.js-git)
1.  [function <span class="apidocSignatureSpan">js-git.</span>indexed_db (repo, prefix)](#apidoc.element.js-git.indexed_db)
1.  [function <span class="apidocSignatureSpan">js-git.</span>walkers (repo)](#apidoc.element.js-git.walkers)
1.  [function <span class="apidocSignatureSpan">js-git.</span>websql_db (repo, prefix)](#apidoc.element.js-git.websql_db)
1.  object <span class="apidocSignatureSpan">js-git.</span>config_codec
1.  object <span class="apidocSignatureSpan">js-git.</span>modes
1.  object <span class="apidocSignatureSpan">js-git.</span>object_codec
1.  object <span class="apidocSignatureSpan">js-git.</span>pack_codec
1.  object <span class="apidocSignatureSpan">js-git.</span>pkt_line

#### [module js-git.config_codec](#apidoc.module.js-git.config_codec)
1.  [function <span class="apidocSignatureSpan">js-git.config_codec.</span>decode (text)](#apidoc.element.js-git.config_codec.decode)
1.  [function <span class="apidocSignatureSpan">js-git.config_codec.</span>encode (config)](#apidoc.element.js-git.config_codec.encode)

#### [module js-git.indexed_db](#apidoc.module.js-git.indexed_db)
1.  [function <span class="apidocSignatureSpan">js-git.</span>indexed_db (repo, prefix)](#apidoc.element.js-git.indexed_db.indexed_db)
1.  [function <span class="apidocSignatureSpan">js-git.indexed_db.</span>init (callback)](#apidoc.element.js-git.indexed_db.init)
1.  [function <span class="apidocSignatureSpan">js-git.indexed_db.</span>loadAs (type, hash, callback)](#apidoc.element.js-git.indexed_db.loadAs)
1.  [function <span class="apidocSignatureSpan">js-git.indexed_db.</span>saveAs (type, body, callback, forcedHash)](#apidoc.element.js-git.indexed_db.saveAs)

#### [module js-git.modes](#apidoc.module.js-git.modes)
1.  [function <span class="apidocSignatureSpan">js-git.modes.</span>isBlob (mode)](#apidoc.element.js-git.modes.isBlob)
1.  [function <span class="apidocSignatureSpan">js-git.modes.</span>isFile (mode)](#apidoc.element.js-git.modes.isFile)
1.  [function <span class="apidocSignatureSpan">js-git.modes.</span>toType (mode)](#apidoc.element.js-git.modes.toType)
1.  number <span class="apidocSignatureSpan">js-git.modes.</span>blob
1.  number <span class="apidocSignatureSpan">js-git.modes.</span>commit
1.  number <span class="apidocSignatureSpan">js-git.modes.</span>exec
1.  number <span class="apidocSignatureSpan">js-git.modes.</span>file
1.  number <span class="apidocSignatureSpan">js-git.modes.</span>sym
1.  number <span class="apidocSignatureSpan">js-git.modes.</span>tree

#### [module js-git.object_codec](#apidoc.module.js-git.object_codec)
1.  [function <span class="apidocSignatureSpan">js-git.object_codec.</span>deframe (buffer, decode)](#apidoc.element.js-git.object_codec.deframe)
1.  [function <span class="apidocSignatureSpan">js-git.object_codec.</span>frame (obj)](#apidoc.element.js-git.object_codec.frame)
1.  [function <span class="apidocSignatureSpan">js-git.object_codec.</span>treeMap (key)](#apidoc.element.js-git.object_codec.treeMap)
1.  [function <span class="apidocSignatureSpan">js-git.object_codec.</span>treeSort (a, b)](#apidoc.element.js-git.object_codec.treeSort)
1.  object <span class="apidocSignatureSpan">js-git.object_codec.</span>decoders
1.  object <span class="apidocSignatureSpan">js-git.object_codec.</span>encoders

#### [module js-git.pack_codec](#apidoc.module.js-git.pack_codec)
1.  [function <span class="apidocSignatureSpan">js-git.pack_codec.</span>decodePack (emit)](#apidoc.element.js-git.pack_codec.decodePack)
1.  [function <span class="apidocSignatureSpan">js-git.pack_codec.</span>encodePack (emit)](#apidoc.element.js-git.pack_codec.encodePack)
1.  [function <span class="apidocSignatureSpan">js-git.pack_codec.</span>parseEntry (chunk)](#apidoc.element.js-git.pack_codec.parseEntry)

#### [module js-git.pkt_line](#apidoc.module.js-git.pkt_line)
1.  [function <span class="apidocSignatureSpan">js-git.pkt_line.</span>deframer (emit)](#apidoc.element.js-git.pkt_line.deframer)
1.  [function <span class="apidocSignatureSpan">js-git.pkt_line.</span>framer (emit)](#apidoc.element.js-git.pkt_line.framer)

#### [module js-git.walkers](#apidoc.module.js-git.walkers)
1.  [function <span class="apidocSignatureSpan">js-git.</span>walkers (repo)](#apidoc.element.js-git.walkers.walkers)
1.  [function <span class="apidocSignatureSpan">js-git.walkers.</span>walk (seed, scan, loadKey, compare)](#apidoc.element.js-git.walkers.walk)

#### [module js-git.websql_db](#apidoc.module.js-git.websql_db)
1.  [function <span class="apidocSignatureSpan">js-git.</span>websql_db (repo, prefix)](#apidoc.element.js-git.websql_db.websql_db)
1.  [function <span class="apidocSignatureSpan">js-git.websql_db.</span>init (callback)](#apidoc.element.js-git.websql_db.init)
1.  [function <span class="apidocSignatureSpan">js-git.websql_db.</span>loadAs (type, hash, callback)](#apidoc.element.js-git.websql_db.loadAs)
1.  [function <span class="apidocSignatureSpan">js-git.websql_db.</span>loadRaw (hash, callback)](#apidoc.element.js-git.websql_db.loadRaw)
1.  [function <span class="apidocSignatureSpan">js-git.websql_db.</span>saveAs (type, body, callback)](#apidoc.element.js-git.websql_db.saveAs)
1.  [function <span class="apidocSignatureSpan">js-git.websql_db.</span>saveRaw (hash, buffer, callback)](#apidoc.element.js-git.websql_db.saveRaw)



# <a name="apidoc.module.js-git"></a>[module js-git](#apidoc.module.js-git)

#### <a name="apidoc.element.js-git.indexed_db"></a>[function <span class="apidocSignatureSpan">js-git.</span>indexed_db (repo, prefix)](#apidoc.element.js-git.indexed_db)
- description and source-code
```javascript
function mixin(repo, prefix) {
  if (!prefix) throw new Error("Prefix required");
  repo.refPrefix = prefix;
  repo.saveAs = saveAs;
  repo.loadAs = loadAs;
  repo.readRef = readRef;
  repo.updateRef = updateRef;
  repo.hasHash = hasHash;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.walkers"></a>[function <span class="apidocSignatureSpan">js-git.</span>walkers (repo)](#apidoc.element.js-git.walkers)
- description and source-code
```javascript
walkers = function (repo) {
  repo.logWalk = logWalk;   // (ref) => stream<commit>
  repo.treeWalk = treeWalk; // (treeHash) => stream<object>
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.websql_db"></a>[function <span class="apidocSignatureSpan">js-git.</span>websql_db (repo, prefix)](#apidoc.element.js-git.websql_db)
- description and source-code
```javascript
function mixin(repo, prefix) {
  if (!prefix) throw new Error("Prefix required");
  repo.refPrefix = prefix;
  repo.saveAs = saveAs;
  repo.saveRaw = saveRaw;
  repo.loadAs = loadAs;
  repo.loadRaw = loadRaw;
  repo.readRef = readRef;
  repo.updateRef = updateRef;
  repo.hasHash = hasHash;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js-git.config_codec"></a>[module js-git.config_codec](#apidoc.module.js-git.config_codec)

#### <a name="apidoc.element.js-git.config_codec.decode"></a>[function <span class="apidocSignatureSpan">js-git.config_codec.</span>decode (text)](#apidoc.element.js-git.config_codec.decode)
- description and source-code
```javascript
function decode(text) {
  var config = {};
  var section;
  text.split(/[\r\n]+/).forEach(function (line) {
    var match = line.match(/\[([^ \t"\]]+) *(?:"([^"]+)")?\]/);
    if (match) {
      section = config[match[1]] || (config[match[1]] = {});
      if (match[2]) {
        section = section[match[2]] = {};
      }
      return;
    }
    match = line.match(/([^ \t=]+)[ \t]*=[ \t]*(.+)/);
    if (match) {
      section[match[1]] = match[2];
    }
  });
  return config;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.config_codec.encode"></a>[function <span class="apidocSignatureSpan">js-git.config_codec.</span>encode (config)](#apidoc.element.js-git.config_codec.encode)
- description and source-code
```javascript
function encode(config) {
  var lines = [];
  Object.keys(config).forEach(function (name) {
    var obj = config[name];
    var deep = {};
    var values = {};
    var hasValues = false;
    Object.keys(obj).forEach(function (key) {
      var value = obj[key];
      if (typeof value === 'object') {
        deep[key] = value;
      }
      else {
        hasValues = true;
        values[key] = value;
      }
    });
    if (hasValues) {
      encodeBody('[' + name + ']', values);
    }

    Object.keys(deep).forEach(function (sub) {
      var child = deep[sub];
      encodeBody('[' + name + ' "' + sub + '"]', child);
    });
  });

  return lines.join("\n") + "\n";

  function encodeBody(header, obj) {
    lines.push(header);
    Object.keys(obj).forEach(function (name) {
      lines.push( "\t" + name + " = " + obj[name]);
    });
  }

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js-git.indexed_db"></a>[module js-git.indexed_db](#apidoc.module.js-git.indexed_db)

#### <a name="apidoc.element.js-git.indexed_db.indexed_db"></a>[function <span class="apidocSignatureSpan">js-git.</span>indexed_db (repo, prefix)](#apidoc.element.js-git.indexed_db.indexed_db)
- description and source-code
```javascript
function mixin(repo, prefix) {
  if (!prefix) throw new Error("Prefix required");
  repo.refPrefix = prefix;
  repo.saveAs = saveAs;
  repo.loadAs = loadAs;
  repo.readRef = readRef;
  repo.updateRef = updateRef;
  repo.hasHash = hasHash;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.indexed_db.init"></a>[function <span class="apidocSignatureSpan">js-git.indexed_db.</span>init (callback)](#apidoc.element.js-git.indexed_db.init)
- description and source-code
```javascript
function init(callback) {

  db = null;
  var request = indexedDB.open("tedit", 1);

  // We can only create Object stores in a versionchange transaction.
  request.onupgradeneeded = function(evt) {
    var db = evt.target.result;

    if (evt.dataLoss && evt.dataLoss !== "none") {
      return callback(new Error(evt.dataLoss + ": " + evt.dataLossMessage));
    }

    // A versionchange transaction is started automatically.
    evt.target.transaction.onerror = onError;

    if(db.objectStoreNames.contains("objects")) {
      db.deleteObjectStore("objects");
    }
    if(db.objectStoreNames.contains("refs")) {
      db.deleteObjectStore("refs");
    }

    db.createObjectStore("objects", {keyPath: "hash"});
    db.createObjectStore("refs", {keyPath: "path"});
  };

  request.onsuccess = function (evt) {
    db = evt.target.result;
    callback();
  };
  request.onerror = onError;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.indexed_db.loadAs"></a>[function <span class="apidocSignatureSpan">js-git.indexed_db.</span>loadAs (type, hash, callback)](#apidoc.element.js-git.indexed_db.loadAs)
- description and source-code
```javascript
function loadAs(type, hash, callback) {
  if (!callback) return loadAs.bind(this, type, hash);
  loadRaw(hash, function (err, entry) {
    if (!entry) return callback(err);
    if (type !== entry.type) {
      return callback(new TypeError("Type mismatch"));
    }
    callback(null, entry.body, hash);
  });
}
```
- example usage
```shell
...

We can read objects back one at a time using 'loadAs'.

'''js
// Reading the file "greeting.txt" from a commit.

// We first read the commit.
var commit = yield repo.loadAs("commit", commitHash);
// We then read the tree using 'commit.tree'.
var tree = yield repo.loadAs("tree", commit.tree);
// We then read the file using the entry hash in the tree.
var file = yield repo.loadAs("blob", tree["greeting.txt"].hash);
// file is now a binary buffer.
'''
...
```

#### <a name="apidoc.element.js-git.indexed_db.saveAs"></a>[function <span class="apidocSignatureSpan">js-git.indexed_db.</span>saveAs (type, body, callback, forcedHash)](#apidoc.element.js-git.indexed_db.saveAs)
- description and source-code
```javascript
function saveAs(type, body, callback, forcedHash) {
  if (!callback) return saveAs.bind(this, type, body);
  var hash;
  try {
    var buffer = codec.frame({type:type,body:body});
    hash = forcedHash || sha1(buffer);
  }
  catch (err) { return callback(err); }
  var trans = db.transaction(["objects"], "readwrite");
  var store = trans.objectStore("objects");
  var entry = { hash: hash, type: type, body: body };
  var request = store.put(entry);
  request.onsuccess = function() {
    // console.warn("SAVE", type, hash);
    callback(null, hash, body);
  };
  request.onerror = function(evt) {
    callback(new Error(evt.value));
  };
}
```
- example usage
```shell
...

In this example, we'll create a blob, create a tree containing that blob, create
a commit containing that tree.  This shows how to create git objects manually.

'''js
// First we create a blob from a string.  The 'formats' mixin allows us to
// use a string directly instead of having to pass in a binary buffer.
var blobHash = yield repo.saveAs("blob", "Hello World\n");

// Now we create a tree that is a folder containing the blob as 'greeting.txt'
var treeHash = yield repo.saveAs("tree", {
  "greeting.txt": { mode: modes.file, hash: blobHash }
});

// With that tree, we can create a commit.
...
```



# <a name="apidoc.module.js-git.modes"></a>[module js-git.modes](#apidoc.module.js-git.modes)

#### <a name="apidoc.element.js-git.modes.isBlob"></a>[function <span class="apidocSignatureSpan">js-git.modes.</span>isBlob (mode)](#apidoc.element.js-git.modes.isBlob)
- description and source-code
```javascript
isBlob = function (mode) {
  return (mode & masks.blob) === masks.mask;
}
```
- example usage
```shell
...

    function onRootTree(err, hash) {
if (!hash) return callback(err);
repo.pathToEntry(hash, path, onEntry);
    }

    function onEntry(err, entry) {
if (!entry || !modes.isBlob(entry.mode)) return callback(err);

repo.loadAs("blob", entry.hash, function (err, content) {
  if (!content) return callback(err);
  if (entry.mode === modes.sym) {
    content = options.decrypt(content);
  }
  callback(null, content);
...
```

#### <a name="apidoc.element.js-git.modes.isFile"></a>[function <span class="apidocSignatureSpan">js-git.modes.</span>isFile (mode)](#apidoc.element.js-git.modes.isFile)
- description and source-code
```javascript
isFile = function (mode) {
  return (mode & masks.file) === masks.mask;
}
```
- example usage
```shell
...
  var entry = cached[parts[index]];
  if (!entry) return callback();
  mode = entry.mode;
  hash = entry.hash;
  index++;
  continue;
}
if (modes.isFile(mode)) return callback();
return callback(null, {
  last: {
    mode: mode,
    hash: hash,
    path: parts.slice(0, index).join("/"),
    rest: parts.slice(index).join("/"),
  }
...
```

#### <a name="apidoc.element.js-git.modes.toType"></a>[function <span class="apidocSignatureSpan">js-git.modes.</span>toType (mode)](#apidoc.element.js-git.modes.toType)
- description and source-code
```javascript
toType = function (mode) {
  if (mode === modes.commit) return "commit";
  if (mode === modes.tree) return "tree";
  if ((mode & masks.blob) === masks.mask) return "blob";
  return "unknown";
}
```
- example usage
```shell
...
    path: "/"
  };
  return callback(null, walk(tree, treeScan, treeLoadKey, treeCompare));
}

function treeLoadKey(entry, callback) {
  if (entry.mode !== modes.tree) return callback(null, entry);
  var type = modes.toType(entry.mode);
  return repo.loadAs(type, entry.hash, function (err, body) {
    if (err) return callback(err);
    entry.body = body;
    return callback(null, entry);
  });
}
...
```



# <a name="apidoc.module.js-git.object_codec"></a>[module js-git.object_codec](#apidoc.module.js-git.object_codec)

#### <a name="apidoc.element.js-git.object_codec.deframe"></a>[function <span class="apidocSignatureSpan">js-git.object_codec.</span>deframe (buffer, decode)](#apidoc.element.js-git.object_codec.deframe)
- description and source-code
```javascript
function deframe(buffer, decode) {
  var space = indexOf(buffer, 0x20);
  if (space < 0) throw new Error("Invalid git object buffer");
  var nil = indexOf(buffer, 0x00, space);
  if (nil < 0) throw new Error("Invalid git object buffer");
  var body = bodec.slice(buffer, nil + 1);
  var size = parseDec(buffer, space + 1, nil);
  if (size !== body.length) throw new Error("Invalid body length.");
  var type = bodec.toRaw(buffer, 0, space);
  return {
    type: type,
    body: decode ? decoders[type](body) : body
  };
}
```
- example usage
```shell
...

function loadAs(type, hash, callback) {
  if (!callback) return loadAs.bind(repo, type, hash);
  loadRaw(hash, function (err, raw) {
    if (raw === undefined) return callback(err);
    var body;
    try {
      raw = codec.deframe(raw);
      if (raw.type !== type) throw new TypeError("Type mismatch");
      body = codec.decoders[raw.type](raw.body);
    }
    catch (err) { return callback(err); }
    callback(null, body);
  });
}
...
```

#### <a name="apidoc.element.js-git.object_codec.frame"></a>[function <span class="apidocSignatureSpan">js-git.object_codec.</span>frame (obj)](#apidoc.element.js-git.object_codec.frame)
- description and source-code
```javascript
function frame(obj) {
  var type = obj.type;
  var body = obj.body;
  if (!bodec.isBinary(body)) body = encoders[type](body);
  return bodec.join([
    bodec.fromRaw(type + " " + body.length + "\0"),
    body
  ]);
}
```
- example usage
```shell
...
  });
}

function saveAs(type, body, callback) {
  if (!callback) return saveAs.bind(repo, type, body);
  var raw, hash;
  try {
    raw = codec.frame({
      type: type,
      body: codec.encoders[type](body)
    });
    hash = sha1(raw);
  }
  catch (err) { return callback(err); }
  saveRaw(hash, raw, function (err) {
...
```

#### <a name="apidoc.element.js-git.object_codec.treeMap"></a>[function <span class="apidocSignatureSpan">js-git.object_codec.</span>treeMap (key)](#apidoc.element.js-git.object_codec.treeMap)
- description and source-code
```javascript
function treeMap(key) {
<span class="apidocCodeCommentSpan">  /*jshint validthis:true*/
</span>  var entry = this[key];
  return {
    name: key,
    mode: entry.mode,
    hash: entry.hash
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.object_codec.treeSort"></a>[function <span class="apidocSignatureSpan">js-git.object_codec.</span>treeSort (a, b)](#apidoc.element.js-git.object_codec.treeSort)
- description and source-code
```javascript
function treeSort(a, b) {
  var aa = (a.mode === modes.tree) ? a.name + "/" : a.name;
  var bb = (b.mode === modes.tree) ? b.name + "/" : b.name;
  return aa > bb ? 1 : aa < bb ? -1 : 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js-git.pack_codec"></a>[module js-git.pack_codec](#apidoc.module.js-git.pack_codec)

#### <a name="apidoc.element.js-git.pack_codec.decodePack"></a>[function <span class="apidocSignatureSpan">js-git.pack_codec.</span>decodePack (emit)](#apidoc.element.js-git.pack_codec.decodePack)
- description and source-code
```javascript
function decodePack(emit) {

  var state = $pack;
  var sha1sum = sha1();
  var inf = inflateStream();

  var offset = 0;
  var position = 0;
  var version = 0x4b434150; // PACK reversed
  var num = 0;
  var type = 0;
  var length = 0;
  var ref = null;
  var checksum = "";
  var start = 0;
  var parts = [];


  return function (chunk) {
    if (chunk === undefined) {
      if (num || checksum.length < 40) throw new Error("Unexpected end of input stream");
      return emit();
    }

    for (var i = 0, l = chunk.length; i < l; i++) {
      // console.log([state, i, chunk[i].toString(16)]);
      if (!state) throw new Error("Unexpected extra bytes: " + bodec.slice(chunk, i));
      state = state(chunk[i], i, chunk);
      position++;
    }
    if (!state) return;
    if (state !== $checksum) sha1sum.update(chunk);
    var buff = inf.flush();
    if (buff.length) {
      parts.push(buff);
    }
  };

  // The first four bytes in a packfile are the bytes 'PACK'
  function $pack(byte) {
    if ((version & 0xff) === byte) {
      version >>>= 8;
      return version ? $pack : $version;
    }
    throw new Error("Invalid packfile header");
  }

  // The version is stored as an unsigned 32 integer in network byte order.
  // It must be version 2 or 3.
  function $version(byte) {
    version = (version << 8) | byte;
    if (++offset < 4) return $version;
    if (version >= 2 && version <= 3) {
      offset = 0;
      return $num;
    }
    throw new Error("Invalid version number " + num);
  }

  // The number of objects in this packfile is also stored as an unsigned 32 bit int.
  function $num(byte) {
    num = (num << 8) | byte;
    if (++offset < 4) return $num;
    offset = 0;
    emit({version: version, num: num});
    return $header;
  }

  // n-byte type and length (3-bit type, (n-1)*7+4-bit length)
  // CTTTSSSS
  // C is continue bit, TTT is type, S+ is length
  function $header(byte) {
    if (start === 0) start = position;
    type = byte >> 4 & 0x07;
    length = byte & 0x0f;
    if (byte & 0x80) {
      offset = 4;
      return $header2;
    }
    return afterHeader();
  }

  // Second state in the same header parsing.
  // CSSSSSSS*
  function $header2(byte) {
    length |= (byte & 0x7f) << offset;
    if (byte & 0x80) {
      offset += 7;
      return $header2;
    }
    return afterHeader();
  }

  // Common helper for finishing tiny and normal headers.
  function afterHeader() {
    offset = 0;
    if (type === 6) {
      ref = 0;
      return $ofsDelta;
    }
    if (type === 7) {
      ref = "";
      return $refDelta;
    }
    // console.log({type: type,length: length})
    return $body;
  }

  // Big-endian modified base 128 number encoded ref offset
  function $ofsDelta(byte) {
    ref = byte & 0x7f;
    if (byte & 0x80) return $ofsDelta2;
    return $body;
  }

  function $ofsDelta2(byte) {
    ref = ((ref + 1) << 7) | (byte & 0x7f);
    if (byte & 0x80) return $ofsDelta2;
    return $body;
  }

  // 20 byte raw sha1 hash for ref
  function $refDelta(byte) {
    ref += toHex(byte);
    if (++offset < 20) return $refDelta;
    return $body;
  }

  // Common helper for generating 2-character hex numbers
  function toHex(num) {
    return num < 0x10 ? "0" + num.toString(16) : num.toString(16);
  }

  // Common helper for emitting all three object shapes
  function emitObject() {
    var body = bodec.join(parts);
    if (body.length !== length) {
      throw new Error("Body length mismatch");
    }
    var item = {
      type: numToType[type],
      size: length,
      body: body,
      offset: start
    };
    if (ref) item.ref = ref;
    parts.length = 0;
    start = 0;
    offset = 0;
    type = 0;
    length = 0;
    ref = null;
    emit(item);
  }

  // Feed the deflated code to the inflate engine
  function $body(byte, i, chunk) {
    if (inf.write(byte)) return $body;
    var buf = inf.flush();
    if (buf.length !== length) throw new Error("Length mismatch, expected " + length + " got " + buf.length);
    inf.recycle();
    if (buf.length) {
      parts.push(buf);
    }
    emitObject();
    // If thi ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.pack_codec.encodePack"></a>[function <span class="apidocSignatureSpan">js-git.pack_codec.</span>encodePack (emit)](#apidoc.element.js-git.pack_codec.encodePack)
- description and source-code
```javascript
function encodePack(emit) {
  var sha1sum = sha1();
  var left;
  return function (item) {
    if (item === undefined) {
      if (left !== 0) throw new Error("Some items were missing");
      return emit();
    }
    if (typeof item.num === "number") {
      if (left !== undefined) throw new Error("Header already sent");
      left = item.num;
      write(packHeader(item.num));
    }
    else if (typeof item.type === "string" && bodec.isBinary(item.body)) {
      // The header must be sent before items.
      if (typeof left !== "number") throw new Error("Headers not sent yet");

      // Make sure we haven't sent all the items already
      if (!left) throw new Error("All items already sent");

      // Send the item in packstream format
      write(packFrame(item));

      // Send the checksum after the last item
      if (!--left) {
        emit(bodec.fromHex(sha1sum.digest()));
      }
    }
    else {
      throw new Error("Invalid item");
    }
  };
  function write(chunk) {
    sha1sum.update(chunk);
    emit(chunk);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.pack_codec.parseEntry"></a>[function <span class="apidocSignatureSpan">js-git.pack_codec.</span>parseEntry (chunk)](#apidoc.element.js-git.pack_codec.parseEntry)
- description and source-code
```javascript
function parseEntry(chunk) {
  var offset = 0;
  var byte = chunk[offset++];
  var type = numToType[(byte >> 4) & 0x7];
  var size = byte & 0xf;
  var left = 4;
  while (byte & 0x80) {
    byte = chunk[offset++];
    size |= (byte & 0x7f) << left;
    left += 7;
  }
  size = size >>> 0;
  var ref;
  if (type === "ref-delta") {
    ref = bodec.toHex(bodec.slice(chunk, offset, offset += 20));
  }
  else if (type === "ofs-delta") {
    byte = chunk[offset++];
    ref = byte & 0x7f;
    while (byte & 0x80) {
      byte = chunk[offset++];
      ref = ((ref + 1) << 7) | (byte & 0x7f);
    }
  }

  var body = inflate(bodec.slice(chunk, offset));
  if (body.length !== size) {
    throw new Error("Size mismatch");
  }
  var result = {
    type: type,
    body: body
  };
  if (typeof ref !== "undefined") {
    result.ref = ref;
  }
  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js-git.pkt_line"></a>[module js-git.pkt_line](#apidoc.module.js-git.pkt_line)

#### <a name="apidoc.element.js-git.pkt_line.deframer"></a>[function <span class="apidocSignatureSpan">js-git.pkt_line.</span>deframer (emit)](#apidoc.element.js-git.pkt_line.deframer)
- description and source-code
```javascript
function deframer(emit) {
  var state = 0;
  var offset = 4;
  var length = 0;
  var data;
  var more = true;

  return function (item) {

    // Forward the EOS marker
    if (item === undefined) return emit();

    // Once we're in pack mode, everything goes straight through
    if (state === 3) return emit(item);

    // Otherwise parse the data using a state machine.
    for (var i = 0, l = item.length; i < l; i++) {
      var byte = item[i];
      if (state === 0) {
        var val = fromHexChar(byte);
        if (val === -1) {
          if (byte === PACK[0]) {
            offset = 1;
            state = 2;
            continue;
          }
          state = -1;
          throw new SyntaxError("Not a hex char: " + String.fromCharCode(byte));
        }
        length |= val << ((--offset) * 4);
        if (offset === 0) {
          if (length === 4) {
            offset = 4;
            more = emit("");
          }
          else if (length === 0) {
            offset = 4;
            more = emit(null);
          }
          else if (length > 4) {
            length -= 4;
            data = bodec.create(length);
            state = 1;
          }
          else {
            state = -1;
            throw new SyntaxError("Invalid length: " + length);
          }
        }
      }
      else if (state === 1) {
        data[offset++] = byte;
        if (offset === length) {
          offset = 4;
          state = 0;
          length = 0;
          if (data[0] === 1) {
            more = emit(bodec.slice(data, 1));
          }
          else if (data[0] === 2) {
            more = emit({progress: bodec.toUnicode(data, 1)});
          }
          else if (data[0] === 3) {
            more = emit({error: bodec.toUnicode(data, 1)});
          }
          else {
            more = emit(bodec.toUnicode(data).trim());
          }
        }
      }
      else if (state === 2) {
        if (offset < 4 && byte === PACK[offset++]) {
          continue;
        }
        state = 3;
        more = emit(bodec.join([PACK, bodec.subarray(item, i)]));
        break;
      }
      else {
        throw new Error("pkt-line decoder in invalid state");
      }
    }

    return more;
  };

}
```
- example usage
```shell
...
var bodyWrite = pktLine.framer(function (chunk) {
  bodyParts.push(chunk);
});
headers["Content-Type"] = "application/x-" + serviceName + "-request";
socket.take(onWrite);

var verified = 0;
var parseResponse = pktLine.deframer(function (line) {
  if (verified === 2) {
    socket.put(line);
  }
  else if (verified === 0) {
    if (line !== "# service=" + serviceName) {
      throw new Error("Illegal service response");
    }
...
```

#### <a name="apidoc.element.js-git.pkt_line.framer"></a>[function <span class="apidocSignatureSpan">js-git.pkt_line.</span>framer (emit)](#apidoc.element.js-git.pkt_line.framer)
- description and source-code
```javascript
function framer(emit) {
  return function (item) {
    if (item === undefined) return emit();
    if (item === null) {
      return emit(bodec.fromRaw("0000"));
    }
    if (typeof item === "string") {
      item = bodec.fromUnicode(item);
    }
    return emit(bodec.join([frameHead(item.length + 4), item]));
  };
}
```
- example usage
```shell
...
// Send the initial request to start the connection.
var headers = {};
if (auth) headers.Authorization = auth;
request("GET", gitUrl + "/info/refs?service=" + serviceName, headers, onResponse);

// Prep for later requests
var bodyParts = [];
var bodyWrite = pktLine.framer(function (chunk) {
  bodyParts.push(chunk);
});
headers["Content-Type"] = "application/x-" + serviceName + "-request";
socket.take(onWrite);

var verified = 0;
var parseResponse = pktLine.deframer(function (line) {
...
```



# <a name="apidoc.module.js-git.walkers"></a>[module js-git.walkers](#apidoc.module.js-git.walkers)

#### <a name="apidoc.element.js-git.walkers.walkers"></a>[function <span class="apidocSignatureSpan">js-git.</span>walkers (repo)](#apidoc.element.js-git.walkers.walkers)
- description and source-code
```javascript
walkers = function (repo) {
  repo.logWalk = logWalk;   // (ref) => stream<commit>
  repo.treeWalk = treeWalk; // (treeHash) => stream<object>
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.walkers.walk"></a>[function <span class="apidocSignatureSpan">js-git.walkers.</span>walk (seed, scan, loadKey, compare)](#apidoc.element.js-git.walkers.walk)
- description and source-code
```javascript
function walk(seed, scan, loadKey, compare) {
  var queue = [seed];
  var working = 0, error, cb;
  return {read: read, abort: abort};

  function read(callback) {
    if (!callback) return read;
    if (cb) return callback(new Error("Only one read at a time"));
    if (working) { cb = callback; return; }
    var item = queue.shift();
    if (!item) return callback();
    try { scan(item).forEach(onKey); }
    catch (err) { return callback(err); }
    return callback(null, item);
  }

  function abort(callback) { return callback(); }

  function onError(err) {
    if (cb) {
      var callback = cb; cb = null;
      return callback(err);
    }
    error = err;
  }

  function onKey(key) {
    working++;
    loadKey(key, onItem);
  }

  function onItem(err, item) {
    working--;
    if (err) return onError(err);
    var index = queue.length;
    while (index && compare(item, queue[index - 1])) index--;
    queue.splice(index, 0, item);
    if (!working && cb) {
      var callback = cb; cb = null;
      return read(callback);
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js-git.websql_db"></a>[module js-git.websql_db](#apidoc.module.js-git.websql_db)

#### <a name="apidoc.element.js-git.websql_db.websql_db"></a>[function <span class="apidocSignatureSpan">js-git.</span>websql_db (repo, prefix)](#apidoc.element.js-git.websql_db.websql_db)
- description and source-code
```javascript
function mixin(repo, prefix) {
  if (!prefix) throw new Error("Prefix required");
  repo.refPrefix = prefix;
  repo.saveAs = saveAs;
  repo.saveRaw = saveRaw;
  repo.loadAs = loadAs;
  repo.loadRaw = loadRaw;
  repo.readRef = readRef;
  repo.updateRef = updateRef;
  repo.hasHash = hasHash;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.websql_db.init"></a>[function <span class="apidocSignatureSpan">js-git.websql_db.</span>init (callback)](#apidoc.element.js-git.websql_db.init)
- description and source-code
```javascript
function init(callback) {

  db = openDatabase('tedit', '1.0', 'tedit local data', 10 * 1024 * 1024);
  db.transaction(function (tx) {
    tx.executeSql(
      'CREATE TABLE IF NOT EXISTS objects (hash unique, body blob)'
    );
    tx.executeSql(
      'CREATE TABLE IF NOT EXISTS refs (path unique, value text)'
    );
  }, function () {
    console.error(arguments);
    callback(new Error("Problem initializing database"));
  }, function () {
    callback();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-git.websql_db.loadAs"></a>[function <span class="apidocSignatureSpan">js-git.websql_db.</span>loadAs (type, hash, callback)](#apidoc.element.js-git.websql_db.loadAs)
- description and source-code
```javascript
function loadAs(type, hash, callback) {
<span class="apidocCodeCommentSpan">  /*jshint: validthis: true */
</span>  if (!callback) return loadAs.bind(this, type, hash);
  loadRaw(hash, function (err, buffer) {
    if (!buffer) return callback(err);
    var parts, body;
    try {
      parts = codec.deframe(buffer);
      if (parts.type !== type) throw new Error("Type mismatch");
      body = codec.decoders[type](parts.body);
    }
    catch (err) {
      return callback(err);
    }
    callback(null, body);
  });
}
```
- example usage
```shell
...

We can read objects back one at a time using 'loadAs'.

'''js
// Reading the file "greeting.txt" from a commit.

// We first read the commit.
var commit = yield repo.loadAs("commit", commitHash);
// We then read the tree using 'commit.tree'.
var tree = yield repo.loadAs("tree", commit.tree);
// We then read the file using the entry hash in the tree.
var file = yield repo.loadAs("blob", tree["greeting.txt"].hash);
// file is now a binary buffer.
'''
...
```

#### <a name="apidoc.element.js-git.websql_db.loadRaw"></a>[function <span class="apidocSignatureSpan">js-git.websql_db.</span>loadRaw (hash, callback)](#apidoc.element.js-git.websql_db.loadRaw)
- description and source-code
```javascript
function loadRaw(hash, callback) {
<span class="apidocCodeCommentSpan">  /*jshint: validthis: true */
</span>  if (!callback) return loadRaw.bind(this, hash);
  var sql = 'SELECT * FROM objects WHERE hash=?';
  db.readTransaction(function (tx) {
    tx.executeSql(sql, [hash], function (tx, result) {
      if (!result.rows.length) return callback();
      var item = result.rows.item(0);
      var buffer;
      try {
        buffer = inflate(bodec.fromBase64(item.body));
      }
      catch (err) {
        return callback(err);
      }
      callback(null, buffer);
    }, function (tx, error) {
      callback(new Error(error.message));
    });
  });
}
```
- example usage
```shell
...
    return checkDelta(item);
  }
  return saveValue(item);
}

function resolveDelta(item) {
  if (opts.onProgress) deltaProgress();
  return repo.loadRaw(item.ref, function (err, buffer) {
    if (err) return onDone(err);
    if (!buffer) return onDone(new Error("Missing base image at " + item.ref));
    var target = codec.deframe(buffer);
    item.type = target.type;
    item.body = applyDelta(item.body, target.body);
    return saveValue(item);
  });
...
```

#### <a name="apidoc.element.js-git.websql_db.saveAs"></a>[function <span class="apidocSignatureSpan">js-git.websql_db.</span>saveAs (type, body, callback)](#apidoc.element.js-git.websql_db.saveAs)
- description and source-code
```javascript
function saveAs(type, body, callback) {
<span class="apidocCodeCommentSpan">  /*jshint: validthis: true */
</span>  if (!callback) return saveAs.bind(this, type, body);
  var hash, buffer;
  try {
    buffer = codec.frame({type:type,body:body});
    hash = sha1(buffer);
  }
  catch (err) { return callback(err); }
  this.saveRaw(hash, buffer, callback);
}
```
- example usage
```shell
...

In this example, we'll create a blob, create a tree containing that blob, create
a commit containing that tree.  This shows how to create git objects manually.

'''js
// First we create a blob from a string.  The 'formats' mixin allows us to
// use a string directly instead of having to pass in a binary buffer.
var blobHash = yield repo.saveAs("blob", "Hello World\n");

// Now we create a tree that is a folder containing the blob as 'greeting.txt'
var treeHash = yield repo.saveAs("tree", {
  "greeting.txt": { mode: modes.file, hash: blobHash }
});

// With that tree, we can create a commit.
...
```

#### <a name="apidoc.element.js-git.websql_db.saveRaw"></a>[function <span class="apidocSignatureSpan">js-git.websql_db.</span>saveRaw (hash, buffer, callback)](#apidoc.element.js-git.websql_db.saveRaw)
- description and source-code
```javascript
function saveRaw(hash, buffer, callback) {
<span class="apidocCodeCommentSpan">  /*jshint: validthis: true */
</span>  if (!callback) return saveRaw.bind(this, hash, buffer);
  var sql = 'INSERT INTO objects (hash, body) VALUES (?, ?)';
  db.transaction(function (tx) {
    var text;
    try {
      text = bodec.toBase64(deflate(buffer));
    }
    catch (err) {
      return callback(err);
    }
    tx.executeSql(sql, [hash, text], function () {
      callback(null, hash);
    });
  });
}
```
- example usage
```shell
...
    // So I will only implement it when I have concrete data to test against.
    console.error({
      list: pending[hash],
      item: item
    });
    throw "TODO: pending value was found, resolve it";
  }
  return repo.saveRaw(hash, buffer, onSave);
}

function onSave(err) {
  if (err) return callback(err);
  packChannel.take(onRead);
}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
