# api documentation for  [gitgoodies (v1.0.1)](https://github.com/qw3rtman/gg)  [![npm package](https://img.shields.io/npm/v/npmdoc-gitgoodies.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gitgoodies) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gitgoodies.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gitgoodies)
#### Shortcuts for the Git Commands You Use Everyday.

[![NPM](https://nodei.co/npm/gitgoodies.png?downloads=true)](https://www.npmjs.com/package/gitgoodies)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gitgoodies/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gitgoodies_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gitgoodies/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gitgoodies/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gitgoodies/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Nimit Kalra",
        "email": "nimit@nimitkalra.com",
        "url": "http://nimitkalra.com"
    },
    "bin": {
        "gg": "bin/gg"
    },
    "bugs": {
        "url": "https://github.com/qw3rtman/gg/issues"
    },
    "dependencies": {
        "chalk": "^1.0.0",
        "cli": "^0.6.5",
        "latest-version": "^1.0.0",
        "request": "^2.53.0"
    },
    "deprecated": "Significantly less-buggy Shell version available (git.io/gitgoodies).",
    "description": "Shortcuts for the Git Commands You Use Everyday.",
    "devDependencies": {
        "jscs": "~1.11.3"
    },
    "directories": {},
    "dist": {
        "shasum": "f294fd3395cff97a3ec3f84d92781ed2cf1205f9",
        "tarball": "https://registry.npmjs.org/gitgoodies/-/gitgoodies-1.0.1.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "f19269d286f00ae9f1f4218647797a616a1f33fd",
    "homepage": "https://github.com/qw3rtman/gg",
    "keywords": [
        "git",
        "goodies",
        "gg",
        "cookbook",
        "shortcuts"
    ],
    "license": "MIT",
    "main": "lib/gg.js",
    "maintainers": [
        {
            "name": "qw3rtman",
            "email": "nimit@nimitkalra.com"
        }
    ],
    "name": "gitgoodies",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/qw3rtman/gg.git"
    },
    "scripts": {
        "test": "jscs -p airbnb lib bin"
    },
    "version": "1.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gitgoodies](#apidoc.module.gitgoodies)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>addAll ()](#apidoc.element.gitgoodies.addAll)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>addOptions (options, target)](#apidoc.element.gitgoodies.addOptions)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>addSingle (target)](#apidoc.element.gitgoodies.addSingle)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>branch (name)](#apidoc.element.gitgoodies.branch)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>checkout (branch)](#apidoc.element.gitgoodies.checkout)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>clone (repository)](#apidoc.element.gitgoodies.clone)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>cloneGitHub (repository)](#apidoc.element.gitgoodies.cloneGitHub)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>commit (message, addAll)](#apidoc.element.gitgoodies.commit)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>fetch ()](#apidoc.element.gitgoodies.fetch)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>fetchAll ()](#apidoc.element.gitgoodies.fetchAll)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>ignore (template)](#apidoc.element.gitgoodies.ignore)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>init ()](#apidoc.element.gitgoodies.init)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>log (file)](#apidoc.element.gitgoodies.log)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>pull ()](#apidoc.element.gitgoodies.pull)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>push ()](#apidoc.element.gitgoodies.push)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>repoCheck (callback)](#apidoc.element.gitgoodies.repoCheck)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>status ()](#apidoc.element.gitgoodies.status)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>upToDate (reportOnTrue, reportOnFalse)](#apidoc.element.gitgoodies.upToDate)
1.  [function <span class="apidocSignatureSpan">gitgoodies.</span>version ()](#apidoc.element.gitgoodies.version)



# <a name="apidoc.module.gitgoodies"></a>[module gitgoodies](#apidoc.module.gitgoodies)

#### <a name="apidoc.element.gitgoodies.addAll"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>addAll ()](#apidoc.element.gitgoodies.addAll)
- description and source-code
```javascript
addAll = function () {
  exec('git add -A');

  console.log(success('[✔] Added everything!'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.addOptions"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>addOptions (options, target)](#apidoc.element.gitgoodies.addOptions)
- description and source-code
```javascript
addOptions = function (options, target) {
  // TODO: Fix the Error Handling! Currently just ignores warnings
  exec('git add -' + options + ' ' + target, function(error, stdout, stderr) {
    if (typeof target === 'undefined') {// Then just add all.
      exports.addAll();
    } else {
      if (stderr.substring(0, 5) === 'fatal') {
        console.log(whoops('[✖] Could not add target specified. ') + chalk.red('Are you sure the target exists?'));
      } else {
        console.log(success('[✔] Added ' + target + '!'));
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.addSingle"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>addSingle (target)](#apidoc.element.gitgoodies.addSingle)
- description and source-code
```javascript
addSingle = function (target) {
  // TODO: Fix the Error handling! Currently just ignores warnings
  exec('git add ' + target, function(error, stdout, stderr) {
    if (typeof target === 'undefined') {// Then just add all.
      exports.addAll();
    } else {
      if (stderr.substring(0, 5) === 'fatal') {
        console.log(whoops('[✖] Could not add target specified. ') + chalk.red('Are you sure the target exists?'));
      } else {
        console.log(success('[✔] Added ' + target + '!'));
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.branch"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>branch (name)](#apidoc.element.gitgoodies.branch)
- description and source-code
```javascript
branch = function (name) {
  if (name === '' || typeof name === 'undefined') { // List branches.
    exec('git branch', function(error, stdout, stderr) {
      if (stdout === '') {
        console.log(notice('[~] No branches exist.'));
      }

      var branches = stdout.split('\n');
      for (var i = 0; i < branches.length - 1; i++) {
        if (branches[i].substring(0, 1) === '*') { // Current branch.
          console.log('|- ' + success.bold(branches[i].substring(2)));
        } else {
          console.log(chalk.dim('|- ' + branches[i].substring(2)));
        }
      }
    });
  } else { // Create branch and checkout.
    exec('git branch ' + name, function(error, stdout, stderr) {
      if (stderr.split(' ')[0] === 'fatal:') {
        if (stderr.substring(0, 21) === 'fatal: A branch named') { // Branch already exists.
          console.log(notice('[~] Branch \'' + name + '\' already exists.'));

          // Checkout branch.
          exports.checkout(name);
        } else if (stderr.slice(-24) === 'not a valid branch name.') { // Invalid branch name.
          console.log(notice('[~] \'' + name + '\' is an invalid branch name.'));
        } else if (stderr.substring(7, 30) === 'Not a valid object name') { // No branches exist.
          console.log(notice('[~] No branches exist.'));
        } else { // Generic error.
          console.log(whoops('[✖] Could not create new branch \'' + name + '\'.'));
        }
      } else {
        console.log(success('[✔] Created new branch \'' + name + '\'!'));

        // Switch to new branch.
        exports.checkout(name);
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.checkout"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>checkout (branch)](#apidoc.element.gitgoodies.checkout)
- description and source-code
```javascript
checkout = function (branch) {
  if (branch === '' || typeof branch === 'undefined') { // If no branch provided, list the branches.
    exports.branch();
  } else {
    exec('git checkout ' + branch, function(error, stdout, stderr) {
      switch (stderr.split(' ')[0]) {
        case 'Already':
          console.log(notice('[~] Already on branch \'' + branch + '\'.'));
          break;

        case 'Switched':
          console.log(success('[✔] Switched to branch \'' + branch + '\'!'));
          break;

        case 'error:': // Branch does not exist.
          console.log(notice('[~] Branch \'' + branch + '\' doesn\'t exist.'));
          console.log();

          exports.branch(branch);
          break;

        case 'fatal':
          console.log(notice('[~] No branches exist.'));
          break;
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.clone"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>clone (repository)](#apidoc.element.gitgoodies.clone)
- description and source-code
```javascript
clone = function (repository) {
  // Nothing to clone.
  if (repository === '' || typeof repository === 'undefined') {
    console.log(notice('[~] You must enter a repository URL or GitHub project (username/repository).'));
  } else {
    exec('git clone ' + repository, function(error, stdout, stderr) {
      if (stderr.substring(0, 7) === 'Cloning') {
        if (stderr.split('\n')[1].split(' ')[0] === 'fatal:') {
          console.log(whoops('[✖] Could not clone repository.'));
        } else {
          console.log(success('[✔] Cloned into ' + stderr.split('\n')[0].split(' ')[2]));
        }
      } else {
        if (stderr.substring(0, 23) === 'fatal: destination path') {
          console.log(notice('[~] Directory ' + stderr.split(' ')[3] + ' is not empty.'));
        } else {
          console.log(whoops('[✖] Could not clone repository.'));
        }
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.cloneGitHub"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>cloneGitHub (repository)](#apidoc.element.gitgoodies.cloneGitHub)
- description and source-code
```javascript
cloneGitHub = function (repository) {
  if (repository === '' || typeof repository === 'undefined') {
    exports.clone(repository);
  } else {
    exports.clone('https://github.com/' + repository + '.git');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.commit"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>commit (message, addAll)](#apidoc.element.gitgoodies.commit)
- description and source-code
```javascript
commit = function (message, addAll) {
  // No commit message.
  if (message === '' || typeof message === 'undefined') {
    console.log(notice('[~] You must enter a commit message.'));
  } else {
    if (addAll) {
      exports.addAll();
    }

    exec('git commit -m "' + message + '"', function(error, stdout, stderr) {
      if (stdout.substring(0, 1) === '[') {
        console.log(success('[✔] Committed!'));

        console.log();
        console.log('"' + underline(message) + '"');
      } else if (stdout.substring(0, 2) === 'On') {
        console.log(notice('[~] Everything already committed.'));
      } else {
        console.log(whoops('[✖] Could not commit changes.') + chalk.red(' Try again if there was a large amount of changes to add
.'));
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.fetch"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>fetch ()](#apidoc.element.gitgoodies.fetch)
- description and source-code
```javascript
fetch = function () {
  exec('git fetch', function(error, stdout, stderr) {
    if (stdout === '' && stderr === '') {
      console.log(success('[✔] Fetched!'));
    } else {
      console.log(whoops('[✖] Could not fetch commits.'));
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.fetchAll"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>fetchAll ()](#apidoc.element.gitgoodies.fetchAll)
- description and source-code
```javascript
fetchAll = function () {
  exec('git fetch --all', function(error, stdout, stderr) {
    if (stderr === '') {
      console.log(success('[✔] Fetched all!'));
    } else {
      console.log(whoops('[✖] Could not fetch commits.'));
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.ignore"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>ignore (template)](#apidoc.element.gitgoodies.ignore)
- description and source-code
```javascript
ignore = function (template) {
  var request = require('request');
  var fs = require('fs');

  if (template === '' || typeof template === 'undefined') {
    request('https://www.gitignore.io/api/list', function(error, response, body) {
      console.log('|- ' + body.replace(new RegExp(','.replace(/([.*+?^=!:${}()|\[\]\/\\])/g, '\\$1'), 'g'), '\n|- '));

      console.log(notice('[~] You must enter one of the templates or languages listed above.'));
    });
  } else {
    request('https://www.gitignore.io/api/' + template, function(error, response, body) {
      if (body.split('\n')[2].substring(0, 10) === '#!! ERROR:') { // Template doesn't exist.
        request('https://www.gitignore.io/api/list', function(error, response, body) {
          console.log('|- ' + body.replace(new RegExp(','.replace(/([.*+?^=!:${}()|\[\]\/\\])/g, '\\$1'), 'g'), '\n|- '));

          console.log(whoops('[✖] Template ' + template + ' does not exist. '));
          console.log(notice('[~] You must enter one of the templates or languages listed above.'));
        });
      } else { // Does exist!
        fs.appendFile('.gitignore', body, function(err) {
          if (err) {
            console.log(whoops('[✖] Could not create .gitignore for ' + template + '.'));
          } else {
            console.log(success('[✔] Created .gitignore for ' + template + '!'));
          }
        });
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.init"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>init ()](#apidoc.element.gitgoodies.init)
- description and source-code
```javascript
init = function () {
  exec('git init', function(error, stdout, stderr) {
    if (stdout.substring(0, 13) === 'Reinitialized') {
      console.log(notice('[~] Reinitialized existing Git repository.'));
    } else {
      console.log(success('[✔] Initialized new Git repository.'));
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.log"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>log (file)](#apidoc.element.gitgoodies.log)
- description and source-code
```javascript
log = function (file) {
  var fileName = '';
  var fs = require('fs');
  var logCommand;

  if (typeof file !== 'undefined' && file !== '') {
    // Testing if the file exists
    try {
      // Trying to open the file
      fs.openSync(file, 'r');
    } catch (ENOENT) {
      // If the file does not exist, we tell the user.
      console.log(whoops('[✖] File ' + file + ' does not exist. '));
      return;
    } finally {
      // We might have other read/write permission errors, etc.
      // But this is not what we are looking for
      // So ending here is good to continue, and we can process the git command
      fileName = ' ' + file;
    }
  }

  if (isWindows) {
    exec('git log --pretty=format:{^|commit^|:^|%H^|,%n^|author^|:^|%an:%ae^|,%n^|date^|:^|%ad^|,%n^|message^|:^|%f^|},' + fileName
, function(error, stdout, stderr) {
      stdout = '[' + stdout.replace(/\|/g, '"').slice(0, -1) + ']';

      if (stdout === '[]\n') { // No commits, so empty array is returned.
        console.log(notice('[~] No commits... yet! Commit with the \'gg c\' command.'));
      }

      var log = JSON.parse(stdout);
      log.reverse(); // Show newest at the bottom.

      for (var i = 0; i < log.length; i++) {
        console.log(); // New line between each commit.

        console.log(notice('[' + log[i].commit + ']'));

        var author = {
          name: log[i].author.split(':')[0].trim(),
          email: '<' + log[i].author.split(':')[1] + '>'
        };

        console.log('|- ' + chalk.gray(author.name) + ' ' + chalk.gray.dim(author.email));
        console.log('|- ' + chalk.gray.dim(log[i].date));
        console.log('|- ' + chalk.green(log[i].message.split('-').join(' ')));
      }
    });
  } else {
    // https://gist.github.com/textarcana/1306223
    exec('git log --pretty=format:\'{%n  "commit": "%H",%n  "author": "%an <%ae>",%n  "date": "%ad",%n  "message": "%f"%n},\'' +
fileName + ' $@ | perl -pe\'BEGIN{print "["}; END{print "]\n"}\' | perl -pe \'s/},]/}]/\'', function(error, stdout, stderr) {
      if (stdout === '[]\n') { // No commits, so empty array is returned.
        console.log(notice('[~] No commits... yet! Commit with the \'gg c\' command.'));
      }

      var log = JSON.parse(stdout);
      log.reverse(); // Show newest at the bottom.

      for (var i = 0; i < log.length; i++) {
        console.log(); // New line between each commit.

        console.log(notice('[' + log[i].commit + ']'));

        var author = {
          name: log[i].author.split('<')[0].trim(),
          email: '<' + log[i].author.split('<')[1]
        };

        console.log('|- ' + chalk.gray(author.name) + ' ' + chalk.gray.dim(author.email));
        console.log('|- ' + chalk.gray.dim(log[i].date));
        console.log('|- ' + chalk.green(log[i].message.split('-').join(' ')));
      }
    });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.pull"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>pull ()](#apidoc.element.gitgoodies.pull)
- description and source-code
```javascript
pull = function () {
  exec('git pull', function(error, stdout, stderr) {
    if (stdout.substring(0, 7) === 'Already') {
      console.log(notice('[~] Everything is already up-to-date.'));
    } else if (stdout.substring(0, 8) === 'Updating') {
      if (stdout.split('\n')[1] === 'error: Your local changes to the following files would be overwritten by merge:') {
        console.log(whoops('[✖] Could not pull commits.') + chalk.red(' (may have to pull using the ') + chalk.red.underline('standard
 git command') + chalk.red(' to handle merge conflicts.)'));
      } else {
        console.log(success('[✔] Pulled!'));
      }
    } else {
      // TODO: add handling for merge conflicts.
      console.log(whoops('[✖] Could not pull commits.') + chalk.red(' (may have to pull using the ') + chalk.red.underline('standard
 git command') + chalk.red(' to handle merge conflicts.)'));
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.push"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>push ()](#apidoc.element.gitgoodies.push)
- description and source-code
```javascript
push = function () {
  exec('git push', function(error, stdout, stderr) {
    if (stderr.split('\n')[0] === 'Everything up-to-date') {
      console.log(notice('[~] All commits already pushed.'));
    } else {
      if (stderr.split('\n')[1].split(' ')[0] === 'fatal:') {
        if (stderr.split('\n')[1].substring(0, 23) === 'fatal: unable to access') {
          console.log(whoops('[✖] Unable to access remote repository due to insufficient permissions.'));
        } else {
          console.log(whoops('[✖] Could not push commits.'));
        }
      } else if (stderr.split('\n')[0].split(' ')[0] === 'To') {
        if (stderr.split('\n')[1].split(' ')[1] === '!') { // Need to pull first.
          // TODO: add handling for non-fast-forwards (when you need to pull first, merge, and then push).
          console.log(notice('[~] Push rejected! Pull changes from remote first.'));
        } else {
          console.log(success('[✔] Pushed!'));
        }
      } else if (stderr.split('\n')[0].substring(0, 30) === 'warning: push.default is unset') {
        if (stderr.split('\n')[21] === 'Everything up-to-date') {
          console.log(notice('[~] All commits already pushed.'));
        } else {
          if (stderr.split('\n')[22].split(' ')[0] === 'fatal:') {
            if (stderr.split('\n')[22].substring(0, 23) === 'fatal: unable to access') {
              console.log(whoops('[✖] Unable to access remote repository due to insufficient permissions.'));
            } else {
              console.log(whoops('[✖] Could not push commits.'));
            }
          } else if (stderr.split('\n')[21].split(' ')[0] === 'To') {
            if (stderr.split('\n')[22].split(' ')[1] === '!') { // Need to pull first.
              // TODO: add handling for non-fast-forwards (when you need to pull first, merge, and then push).
              console.log(notice('[~] Push rejected! Pull changes from remote first.'));
            } else {
              console.log(success('[✔] Pushed!'));
            }
          } else { // Generic error.
            console.log(whoops('[✖] Could not push commits.'));
          }
        }
      } else { // Generic error.
        console.log(whoops('[✖] Could not push commits.'));
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.repoCheck"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>repoCheck (callback)](#apidoc.element.gitgoodies.repoCheck)
- description and source-code
```javascript
repoCheck = function (callback) {
  exec('git rev-parse', function(error, stdout, stderr) {
    if (stderr.length === 0) {
      return callback();
    }
    console.log(whoops('[✖] Not in a valid git repository! Run "gg i" to initialise one.'));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.status"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>status ()](#apidoc.element.gitgoodies.status)
- description and source-code
```javascript
status = function () {
  exec('git status', function(error, stdout, stderr) {
    var status = stdout.split('\n');

    // Branch.
    var branch;
    if (status[0].split(' ')[0] === 'HEAD') { // If HEAD is at a commit.
      branch = chalk.dim('branch  ') + chalk.gray.dim(' | ') + success(status[0].split(' ')[3]);
    } else {
      branch = chalk.dim('branch  ') + chalk.gray.dim(' | ') + success(status[0].split(' ')[2]);
    }

    console.log(branch);

    // Position in branch.
    var position;
    switch (status[1].split(' ')[3]) {
      case 'behind':
        position = 'position' + chalk.gray.dim(' | ') + notice(status[1].split(' ')[7] + ' commits behind (fetch or pull)');
        break;

      case 'for': // Quick hack to get it working when changes are not staged.
      case 'working': // Quick hack to get it working with freshly initialized git repositories.
      case 'up-to-date':
        position = chalk.dim('position') + chalk.gray.dim(' | ') + success('up-to-date');
        break;

      case 'ahead':
        position = 'position' + chalk.gray.dim(' | ') + notice(status[1].split(' ')[7] + ' commits ahead (push commits)');
        break;

      default:
        // TODO: add proper handling for freshly initialized git repositories.
        if (typeof status[1].split(' ')[3] === 'undefined') { // Quick hack to get it working with freshly initialized git repositories
.
          position = chalk.dim('position') + chalk.gray.dim(' | ') + success('up-to-date');
        } else if (status[1] === 'Changes to be committed:') {
          position = chalk.dim('position') + chalk.gray.dim(' | ') + success('up-to-date');
        } else {
          position = 'position' + chalk.gray.dim(' | ') + whoops('diverged');
        }
    }
    console.log(position);

    console.log();

    // Staging.
    var staging;
    if (status[2] === 'Initial commit') { // Fresh repository.
      switch (status[4]) {
        case 'Untracked files:':
          staging = 'staging ' + chalk.gray.dim(' | ') + notice('not all changes staged (add all changes)');
          break;

        case 'Changes to be committed:':
        case 'nothing to commit (create/copy files and use "git add" to track)':
          staging = chalk.dim('staging ') + chalk.gray.dim(' | ') + success('all changes staged');
          break;
      }
    } else if (status[1].substring(0, 14) === 'Your branch is') { // There's a remote origin.
      if (status[2] === '  (use "git pull" to update your local branch)' || status[2] === '  (use "git push" to publish your local
 commits)') {
        switch (status[4]) {
          case 'Changes not staged for commit:':
          case 'Untracked files:':
            staging = 'staging ' + chalk.gray.dim(' | ') + notice('not all changes staged (add all changes)');
            break;

          case 'Changes to be committed:':
          case 'nothing to commit, working directory clean':
            staging = chalk.dim('staging ') + chalk.gray.dim(' | ') + success('all changes staged');
            break;
        }
      } else {
        if (status[2] === '') {
          switch (status[3]) {
            case 'Changes not staged for commit:':
            case 'Untracked files:':
              staging = 'staging ' + chalk.gray.dim(' | ') + notice('not all changes staged (add all changes)');
              break;

            case 'Changes to be committed:':
            case 'nothing to commit, working directory clean':
              staging = chalk.dim('staging ') + chalk.gray.dim(' | ') + success('all changes staged');
              break;
          }
        } else {
          switch (status[2]) {
            case 'Changes not staged for commit:':
            case 'Untracked files:':
              staging = 'staging ' + chalk.gray.dim(' | ') + notice('not all changes staged (add all changes)');
              break;

            case 'Changes to be committed:':
            case 'nothing to commit, working directory clean':
              staging = chalk.dim('staging ') + chalk.gray.dim(' | ') + success('all changes staged');
              break; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.upToDate"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>upToDate (reportOnTrue, reportOnFalse)](#apidoc.element.gitgoodies.upToDate)
- description and source-code
```javascript
upToDate = function (reportOnTrue, reportOnFalse) {
  var package = require('../package.json');
  var currentVersion = package.version;

  var latestVersion = require('latest-version');
  latestVersion('gitgoodies', function(err, version) {
    if (version !== currentVersion) { // Not up to date.
      if (reportOnFalse) {
        console.log();
        console.log(notice('[~] This version of gg is not up-to-date.') + ' ' + chalk.yellow('Update with ' + chalk.bold('npm update
 -g gitgoodies') + '.'));
      }
    } else {
      if (reportOnTrue) {
        console.log();
        console.log(success('[✔] This version of gg is up-to-date.'));
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gitgoodies.version"></a>[function <span class="apidocSignatureSpan">gitgoodies.</span>version ()](#apidoc.element.gitgoodies.version)
- description and source-code
```javascript
version = function () {
  var package = require('../package.json');
  var version = package.version;

  console.log(success('gg') + ' version ' + notice(version));

  exports.upToDate(true, false);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
