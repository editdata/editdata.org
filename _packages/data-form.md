---
user: editdata
path: editdata/data-form
name: data-form
head: 19a76e361e2ca133995f9e776b1632eef9cf5e20
readme: >
  #data-form



  Generate a form from the row of a dataset and it's JSONSchema-style
  properties.



  ## Install



      npm i --save editdata/data-form



  ## API



  ### createDataForm



  Create a form from the row of a dataset and its properties



  **Parameters**



  -   `options` **Object**

      -   `options.row` **Array** The row to be edited

      -   `options.properties` **Object** The row properties/column names

      -   `options.header` **Boolean**

      -   `options.header` **Object** virtual-dom vtree that should be used for
  the header



  ## License



  [MIT](LICENSE.md)
package:
  name: data-form
  version: 1.0.0
  description: ''
  main: index.js
  style: style.css
  scripts:
    docs: 'documentation-readme README.md -s "API" -- index.js'
    example: budo example/index.js --dir example --live
    test: 'tape test.js | tap-spec'
  repository:
    type: git
    url: 'git+https://github.com/editdata/data-form.git'
  keywords:
    - data-ui
  author: sethvincent
  license: MIT
  bugs:
    url: 'https://github.com/editdata/data-form/issues'
  homepage: 'https://github.com/editdata/data-form#readme'
  dependencies:
    base-element: ^3.0.1
    component-emitter: ^1.2.0
    data-fields: 'github:editdata/data-fields'
    data-format: 'github:editdata/data-format'
    inherits: ^2.0.1
    virtual-hook: ^1.0.1
  devDependencies:
    browserify: ^13.0.0
    budo: ^8.1.0
    data-editor: 'github:editdata/data-editor'
    documentation-readme: ^2.1.0
    sheetify: ^4.1.0
contributors:
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
    contributions: 5
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
    contributions: 5
page: false
---

