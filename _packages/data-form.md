---
user: editdata
path: editdata/data-form
name: data-form
head: 075972319455fba97ec023acfdf039569799af8a
readme: >
  #data-form



  Generate a form from the row of a dataset and it's JSONSchema-style
  properties.



  [![npm](https://img.shields.io/npm/v/data-form.svg)](http://npmjs.com/data-form)



  ## Install



      npm i --save editdata/data-form



  ## API



  createDataForm(h, options)



  ### createDataForm



  Create a form from the row of a dataset and its properties



  **Parameters**

  - `h` **Function** DOM hyperscript function

  -   `options` **Object**

      -   `options.row` **Array** The row to be edited

      -   `options.properties` **Object** The row properties/column names

      -   `options.header` **Boolean**

      -   `options.header` **Object** virtual-dom vtree that should be used for
  the header

      -   `options.onclick` **Function** Event handler that fires when a field is
  clicked

      -   `options.oninput` **Function** Event handler that fires when a field is
  receiving input.  Receives the arguments `event`, `rowKey`, `propertyKey`,
  `inputValue`

      -   `options.onupdate` **Function** Event handler that fires whenever some
  data has changed.

      -   `options.ondestroy` **Function** Event handler that fires when user
  clicks the `destroy row` button.

      -   `options.onclose` **Function** Event handler that fires when user
  clicks the `close` button.



  ## License



  [MIT](LICENSE.md)
package:
  name: data-form
  version: 3.0.0
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
    data-fields: ^5.0.0
    data-format: ^1.0.0
    inherits: ^2.0.1
    virtual-hook: ^1.0.1
  devDependencies:
    browserify: ^13.0.0
    budo: ^8.1.0
    data-editor: 'github:editdata/data-editor'
    documentation-readme: ^2.1.0
    sheetify: ^4.1.0
    virtual-raf: ^3.0.0
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
    contributions: 11
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
    contributions: 10
page: false
---

