---
user: editdata
path: editdata/data-field-string
name: data-field-string
head: 2a95c2dc0241dff53f2c48ee77d8fe7d80a8fc05
readme: >
  # data-field-string



  ## API



  ### createStringField



  Create a virtual-dom string data-field for use with
  [data-ui](https://github.com/editdata/data-ui).





  **Parameters**



  -   `options` **Object** an options object, including any properties you can
  pass to virtual-dom/h

      -   `options.display` **Boolean** true for display mode, default is false
  for input mode







  **Examples**



  ```javascript

  var createStringField = require('data-field-string')

  var field = createStringField()

  var vtree = field.render(h, {}, 'example string')

  ```









  ### createStringField



  Create a virtual-dom string data-field for use with
  [data-ui](https://github.com/editdata/data-ui).





  **Parameters**



  -   `h` **function** virtual-dom `h` function



  -   `properties` **Object** an options object, including any properties you can
  pass to virtual-dom/h

      -   `properties.display` **Boolean** true for display mode, default is
  false for input mode



      -   `properties.value` **String** any string



  -   `value` **String** any string







  **Examples**



  ```javascript

  var createStringField = require('data-field-string')

  var field = createStringField()

  var vtree = field.render(h, {}, 'example string')

  ```



  ## Installation



  ```sh

  npm install data-field-string --save

  ```



  Or install the [data-fields](https://github.com/editdata/data-fields) module:

  ```sh

  npm install data-fields --save

  ```



  ## Tests



  ```sh

  npm install

  npm test

  ```





  ## See also



  -   [data-fields](https://github.com/editdata/data-fields) – all data fields
  packaged together.

  -   [data-ui](https://github.com/editdata/data-ui) – a collection of modules
  for managing data.



  ## License



  [MIT](LICENSE.md)
package:
  name: data-field-string
  version: 2.0.0
  author: sethvincent
  bugs:
    url: 'https://github.com/editdata/data-field-string/issues'
  dependencies:
    component-emitter: ^1.2.0
    data-field-classname: ^1.0.0
    xtend: ^4.0.0
  devDependencies:
    budo: ^5.1.5
    documentation-readme: ^2.0.0
    standard: ^5.3.1
    tap-spec: ^4.1.0
    tape: ^4.2.2
    virtual-dom: ^2.1.1
    virtual-raf: ^2.0.3
  homepage: 'https://github.com/editdata/data-field-string'
  keywords:
    - data
    - dom
    - editdata
    - element
    - html
    - virtual-dom
  license: MIT
  main: index.js
  repository:
    type: git
    url: 'git+https://github.com/editdata/data-field-string.git'
  scripts:
    docs: 'documentation-readme README.md -s "API" -- index.js'
    example-basic: budo examples/basic.js --live
    test: 'standard && tape tests/*.js | tap-spec'
  style: style.css
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
    contributions: 2
page: false
---

