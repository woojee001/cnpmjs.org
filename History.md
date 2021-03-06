
0.3.13 / 2014-03-27
==================

 * fix npm adduser update 409 bug
 * fix multiline coverage
 * show package engines. fixed #280
 * dont sync local package field. fix #295

0.3.12 / 2014-03-26
==================

 * fix result.successes not exist error
 * fix search list
 * add simple request for listall
 * only return package name in /-/all and /-/all/since, fixed #291
 * refine docs foloder
 * use module gmt_modified as etag. fix #288
 * fix typo, remove unused config in package.json
 * web page only list cnpm registry related info
 * use generator in qnfs

0.3.11 / 2014-03-20 
==================

  * use common.isMaintainer, fixed #283
  * update dependencies
  * use co-mocha for test, fixed #279
  * update thunkify-wrap, breaking change in thunkify-wrap
  * refactor SQLs by using multiline
  * use multiline to refactor sqls
  * ignore contributors

0.3.10 / 2014-03-16 
==================

  * Only /_session request send the authSession. fixed #223
  * sync npm user info when maintainers and contributors not exists. fixed #82
  * save npm user to mysql
  * password salt always be randoms
  * remove session access in /name and /name/version, fixed #274
  * fix update maintainer session error
  * update koa-middlewares
  * fix test, fix sync_by_install
  * use defer session
  * Support npm owner|author add [name] [pkg]. fixed #271

0.3.9 / 2014-03-14 
==================

  * custom user-agent
  * use co-urllib instead of thunkify urllib; fix mock http.request test cases
  * request limit custom message
  * add config.redis check
  * add koa-limit, fixed #267

0.3.8 / 2014-03-11 
==================

  * update middlewares, fixed missing charset bug #264

0.3.7 / 2014-03-11 
==================

  * show worker die date time
  * update to koa@0.5.1
  * hotfix for star user
  * fix yield gather, sync missing deps even no missing versions
  * fix return versions
  * fix makefile, remove eventproxy
  * refactor sync_module_worker
  * add make test-dev, fixed #259
  * change npm.js to generator
  * update urllib, proxy/npm.js use generator
  * sync_all and sync_exist to generator
  * change function to generator
  * need node >= v0.11.9

0.3.6 / 2014-03-06 
==================

  * install missing package should sync it from source npm. fixed #252
  * npm publish dont contains .jshint*
  * npm test run jshint
  * Add jshint check: $ make jshint
  * use `yield* next` instead of `yield next`
  * replace dist.u.qiniudn.com with cnpmjs.org/dist

0.3.5 / 2014-03-05 
==================

  * redirect /dist/xxx.tgz => http://dist.u.qiniudn.com/xxx.tgz fixed #249
  * redirect /name to /package/name when /name is 404. fixed #245
  * Add missing properies and sync missing star users. fixed #235

0.3.4 / 2014-03-04 
==================

  * add cov
  * use istanbul run test coverage
  * gzip support. fix #241
  * readme spelling patch (@stanzheng)
  * default readme to null, fixed #233
  * remove readme in versions

0.3.3 / 2014-02-28 
==================

  * Merge pull request #232 from cnpm/host-hotfix
  * get request host from request.headers
  * Merge pull request #231 from cnpm/bug-fix
  * fix deps display bug#230 and nsf.url TypeError#229

0.3.2 / 2014-02-28 
==================

  * update koa-sess and koa-redis
  * fix sync all test
  * remove nfs.downloadStream first, fix tmppath error
  * fix fengmk2/giturl#1 bug

0.3.1 / 2014-02-27 
==================

  * add etag fixed #224
  * travis ci install on source npm

0.3.0 / 2014-02-27 
==================

  * fix typo and dont sync not exists pkgs
  * use koa-middlewares
  * fix signed cookie not work on npm@1.3.25; node --harmony-generators
  * fix opensearch test case
  * update koa bodyparser
  * logger.error(err) should send err stack email notice
  * json body parse limit and bug fix.
  * fix sync 404 reason not clear
  * all controllers to koa
  * controller/web/user.js to koa
  * change web connect to koa
  * use outputError
  * use yield exports.addPackageAndDist.call(this, next);
  * add end() when ws write end
  * fix yield coWrite
  * fix all the test of registry module.test.js
  * convert registry/module.js to koa type
  * fix auth middleware
  * finish registry user controller koa and update mm to support thunkify. fixed #196
  * change controllers/user.js to koa
  * thunkify all proxy
  * convert all middlewares to koa type
  * change regsitry sync to koa
  * addd koa-jsonp, koa-bodyparser, fix / controller
  * first koa run registry home page /
  * Merge pull request #212 from cnpm/fix-sync-404
  * return friendly 404 reason
  * Merge pull request #211 from cnpm/bug-fix
  * override json limit to default 10mb. fixed #209
  * fix #210 addPackageAndDist package version detect bug

0.2.27 / 2014-02-19 
==================

  * support json result in search, fixed #189

0.2.26 / 2014-02-19 
==================

  * npm publish also need to add deps

0.2.25 / 2014-02-19 
==================

  * max handle number of package.json `dependencies` property
  * Dependents support. fixed #190

0.2.24 / 2014-02-13 
==================

  * fix if delete all the versions
  * refactor remove module, fixed #186

0.2.23 / 2014-01-26 
==================

  * system admin can add, publish, remove the packages. fixed #176

0.2.22 / 2014-01-26 
==================

  * add keyword and search support keyword. #181

0.2.21 / 2014-01-24 
==================

  * refactor code styles on package.html
  * nav-tabs e.preventDefault
  * Show registry server error response. fixed #178
  * nav-tabs for package.html (@4simple)

0.2.20 / 2014-01-23 
==================

  * hotfix sync missing dependencies and readmes
  * fix sync readme error, fixed #174
  * add updateReadme in module

0.2.19 / 2014-01-22 
==================

  * npm install no need to check authorization header. fixed #171

0.2.18 / 2014-01-20 
==================

  * Support gitlab git url to display and click. fixed #160
  * fix redis crash

0.2.17 / 2014-01-17 
==================

  * custom logo url
  * hotfix layout bug

0.2.16 / 2014-01-16 
==================

  * fix publish-time bug

0.2.15 / 2014-01-16 
==================

  * add publish_time to debug

0.2.14 / 2014-01-16 
==================

  * add make autod
  * update publish_time, fixed #163

0.2.13 / 2014-01-15 
==================

  * markdown tmpl not support footer, need to wrap on app start

0.2.12 / 2014-01-15 
==================

  * add footer and npm client name customable

0.2.11 / 2014-01-15 
==================

  * package page contributor link to search, default is true

0.2.10 / 2014-01-14 
==================

  * fix #155 Content-Disposition wrong.

0.2.9 / 2014-01-14 
==================

  * support startkey=c and startkey="c"
  * support couch db search api. fixed #153
  * fix fork me image link
  * support sync by query.name

0.2.8 / 2014-01-14 
==================

  * dont show err stack on test env
  * add download link for package page

0.2.7 / 2014-01-13 
==================

  * add shasum when nfs.upload and hfs.uploadBuffer, fixed #148

0.2.6 / 2014-01-13 
==================

  * support custom session store, fixed #146

0.2.5 / 2014-01-13 
==================

  * add download timeout and unit test
  * use downloadStream() first
  * nfs download to a writeable stream.

0.2.4 / 2014-01-10 
==================

  * set main script to  index.js, fixed #142

0.2.3 / 2014-01-10 
==================

  * Dont show sync button on private package
  * Sync package as publish with no deps. fixed #138

0.2.2 / 2014-01-10 
==================

  * keep compatibility
  * qnfs upload only callback a url
  * compat remove package
  * set tarball url
  * new npm publish in one request, add _publish_in_cnpm
  * support unsure name ufs
  * contributors maybe a object
  * Object #<Object> has no method 'forEach' fixed #134
  * support custom config as a module, fixed issue #132
  * support npm new publish flow. fixed #129
  * add toString and constructor to test admin
  * fix #119 hasOwnProperty check admin bug.

0.2.0 / 2013-12-27 
==================

  * remove to lower case
  * fix #127 execSync and execsync.
  * add contributors list on package page
  * mv blanket to config
  * sync typeerror fix #statusCode
  * add disturl
  * fix #122 admin security bug
  * fixed #121, let pkg 404 as success
  * fix sql insert error
  * fix typos

0.1.3 / 2013-12-20
==================

  * add favicon
  * Fix auth middleware bug (@alsotang)
  * make sure all packages name are lower case
  * select ids from tag
  * fix nodejsctl
  * fix #112 missing versions and time no sync
  * remove restart command
  * fix sync missing packages error
  * fix web/readme.md, add install
  * fix #109 pkg no times and no versions bug.

0.1.2 / 2013-12-19
==================

  * fix times not exists canot sync bug. fixed #101
  * support npm run command
  * remove before_install and install in travis, fixed #102
  * split all sub queries, fixed #104
  * fix doc, fixed #103
  * fix search too slow.
  * dont email sync log level info
  * only sync missing packages at first time
  * update dependencies
  * sync all will sync all the missing packages, fixed #97

0.1.0 / 2013-12-12
==================

  * add sync title
  * add favicon. fixed #69
  * refine sync page, fiexd #70
  * add app version
  * add test for sync
  * refine sync page
  * registry and web all use controllers/sync.js
  * sync from web, fixed #58
  * saving missing descriptions
  * add package download info. fixed #63
  * add avatar
  * use dependecies, fixed #issue62
  * support open search, fixed #60
  * make sure publish_time and author is same to source npm registry. fixed #56
  * add test for search
  * add a simple search by mysql like
  * fix This version of MySQL doesn't yet support 'LIMIT & IN/ALL/ANY/SOME subquery. fixed #54
  * update install doc, use nodejsctl to start
  * must add limit on list by author sql
  * fix sql, change test to fit my local database, fixed #46
  * use registry.cnpmjs.org
  * add install document and total package info on home page. fix #42
  * add module_id to tag table. #46
  * skip error version. fixed #43
  * sync may make a user do not exist in database, but have modules in registry
  * add user page
  * fix set license
  * ignore 404 on sync. fixed #39
  * fix module page, add test
  * update urllib to 0.5.5
  * version and tag
  * add module page
  * fix download url
  * first get tag, then try version
  * support sync triggle by install, finish #31
  * addTag error return 500
  * just one download field
  * add download total info on home page
  * add download count
  * versions empty and also check missing tags
  * remove tags on unpublish
  * add module tag. fix #6
  * add [done] flag to check sync done on client
  * get sync log #29
  * fix test in module
  * rm tmp file on down request error
  * add time for debug str
  * fix pkg not exists null bug
  * use sync module woker to handle sync process. fixed #19
  * if private mode enable, only admin can publish module
  * add alias in readme
  * fix sql, add sort by name
  * fix sql
  * add api to support npm search and auto completion
  * add npm and cnpm image
  * add registry total info on home page
  * fix mods bug in module.removeAll, change module.update => module.removeWithVersions
  * add test, fix bug. fixed #18
  * spoort unpublish
  * add web page index readme
  * switchable nfs #21
  * change file path to match npm file path
  * use qn cdn to store tarball file fixed #16
  * add GET /:name/:version, fixed #3
  * add module controller test cases; fix next module not exists logic bug.
  * publish module flow finish #11
  * add test for controllers/registry/user.js
  * add test for middleware/auth
  * add test for proxy/user
  * remove index.js
  * fix typo
  * add redis as session store
  * fix nodejsctl mod
  * add start time
  * add home page
  * remove session controller
  * adduser() finish fixed #5
  * rm app.js and routes.js
  * Mock npm adduser server response, fixing #5
  * adjust project dir, separate registry and web server
  * Init rest frame for cnpmjs.org
  * init
