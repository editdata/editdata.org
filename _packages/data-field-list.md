---
user: editdata
path: editdata/data-field-list
name: data-field-list
head: f6d6412724565d03c967a5552dbebe7cec126e18
page: false
readme: >
  # data-field-list



  ## API



  ### createListField



  Create a virtual-dom list (object or array) data-field for use with
  [data-ui](https://github.com/editdata/data-ui).





  **Parameters**



  -   `options` **Object** an options object, including any properties you can
  pass to virtual-dom/h

      -   `options.display` **Boolean** true for display mode, default is false
  for input mode



      -   `options.keys` **Boolean** , false for array mode, default is true for
  object mode







  **Examples**



  ```javascript

  var createListField = require('data-field-string')

  var field = createListField()

  var tree = field.render(h, properties, ['a', 'b', 'c'])

  ```









  ### createListField



  Create a virtual-dom list (object or array) data-field for use with
  [data-ui](https://github.com/editdata/data-ui).





  **Parameters**



  -   `h` **function** virtual-dom `h` function



  -   `properties` **Object** an options object, including any properties you can
  pass to virtual-dom/h

      -   `properties.display` **Boolean** true for display mode, default is
  false for input mode



      -   `properties.keys` **Boolean** , false for array mode, default is true
  for object mode



      -   `properties.value` **Object** an array or flat object



      -   `properties.value` **Array** an array or flat object



  -   `value` **Object** an array or flat object



  -   `value` **Array** an array or flat object







  **Examples**



  ```javascript

  var createListField = require('data-field-string')

  var field = createListField()

  var tree = field.render(h, properties, ['a', 'b', 'c'])

  ```



  ## Installation



  ```sh

  npm install data-field-list --save

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
  name: data-field-list
  version: 2.0.0
  author: sethvincent
  bugs:
    url: 'https://github.com/editdata/data-field-list/issues'
  dependencies:
    component-emitter: ^1.2.0
    data-field-classname: ^1.0.0
    isarray: 0.0.1
    list-editor: ^1.0.1
    object-array-converter: ^1.0.0
    xtend: ^4.0.0
  devDependencies:
    budo: ^5.1.5
    documentation-readme: ^2.0.0
    standard: ^5.3.1
    tap-spec: ^4.1.0
    tape: ^4.2.2
    virtual-dom: ^2.1.1
    virtual-raf: ^2.0.3
  homepage: 'https://github.com/editdata/data-field-list'
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
    url: 'git+https://github.com/editdata/data-field-list.git'
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
    contributions: 3
---
