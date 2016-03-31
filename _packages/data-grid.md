---
user: editdata
path: editdata/data-grid
name: data-grid
head: 65740b034c01a1893435671310f4773f66ca5d10
contributors:
  - login: sethvincent
    id: 164214
    avatar_url: 'https://avatars.githubusercontent.com/u/164214?v=3'
    gravatar_id: ''
    url: 'https://api.github.com/users/sethvincent'
    html_url: 'https://github.com/sethvincent'
    followers_url: 'https://api.github.com/users/sethvincent/followers'
    following_url: 'https://api.github.com/users/sethvincent/following{/other_user}'
    gists_url: 'https://api.github.com/users/sethvincent/gists{/gist_id}'
    starred_url: 'https://api.github.com/users/sethvincent/starred{/owner}{/repo}'
    subscriptions_url: 'https://api.github.com/users/sethvincent/subscriptions'
    organizations_url: 'https://api.github.com/users/sethvincent/orgs'
    repos_url: 'https://api.github.com/users/sethvincent/repos'
    events_url: 'https://api.github.com/users/sethvincent/events{/privacy}'
    received_events_url: 'https://api.github.com/users/sethvincent/received_events'
    type: User
    site_admin: false
    contributions: 25
  - login: kvnneff
    id: 3835556
    avatar_url: 'https://avatars.githubusercontent.com/u/3835556?v=3'
    gravatar_id: ''
    url: 'https://api.github.com/users/kvnneff'
    html_url: 'https://github.com/kvnneff'
    followers_url: 'https://api.github.com/users/kvnneff/followers'
    following_url: 'https://api.github.com/users/kvnneff/following{/other_user}'
    gists_url: 'https://api.github.com/users/kvnneff/gists{/gist_id}'
    starred_url: 'https://api.github.com/users/kvnneff/starred{/owner}{/repo}'
    subscriptions_url: 'https://api.github.com/users/kvnneff/subscriptions'
    organizations_url: 'https://api.github.com/users/kvnneff/orgs'
    repos_url: 'https://api.github.com/users/kvnneff/repos'
    events_url: 'https://api.github.com/users/kvnneff/events{/privacy}'
    received_events_url: 'https://api.github.com/users/kvnneff/received_events'
    type: User
    site_admin: false
    contributions: 8
package:
  name: data-grid
  version: 1.2.1
  description: ''
  main: index.js
  style: style.css
  scripts:
    lint: standard
    budo: "budo example/index.js --dir example --live --onupdate 'npm run build-example'"
    example: npm run budo
    build-example: 'npm run build-example-js & npm run build-example-css'
    build-example-js: 'browserify example/index.js > example/bundle.js'
    build-example-css: 'postcss -u autoprefixer -u postcss-import example/style.css > example/bundle.css'
    deploy: 'npm run build-example && gh-pages -d example'
  repository:
    type: git
    url: 'git+https://github.com/editdata/data-grid.git'
  author: sethvincent
  license: MIT
  bugs:
    url: 'https://github.com/editdata/data-grid/issues'
  homepage: 'https://github.com/editdata/data-grid#readme'
  dependencies:
    data-fields: ^3.0.0
    extend: ^3.0.0
    vdom-thunk: ^3.0.0
    view-list: ^2.0.0
  devDependencies:
    autoprefixer: ^6.3.3
    browserify: ^13.0.0
    budo: ^8.1.0
    data-form: ^1.1.2
    data-format: ^1.0.1
    gh-pages: ^0.11.0
    postcss-cli: ^2.5.1
    postcss-import: ^8.0.2
    standard: ^6.0.8
    virtual-app: ^3.0.0
readme: >
  # data-grid



  Simple & performant grid editor/viewer for data.



  [![npm](https://img.shields.io/npm/v/data-grid.svg)](http://npmjs.com/data-grid)



  [View an online demo.](http://about.editdata.org/data-grid/)



  ## See also



  - [data-ui](https://github.com/editdata/data-ui) – a collection of resources
  & modules for building interfaces for managing data

  - [view-list](https://github.com/shama/view-list) – this project is a thin
  wrapper around the view-list module

  - [virtual-dom](https://github.com/Matt-Esch/virtual-dom) – data-grid
  & view-list are created using the virtual-dom module



  ## License



  [MIT](LICENSE.md)
page: 'http://about.editdata.org/data-grid/'
---

