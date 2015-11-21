---
user: editdata
path: editdata/data-field-image
name: data-field-image
head: 9575e14d5d2a15d22444e1dcda6d30cb71bf348c
page: false
readme: >
  # data-field-image



  ## API



  ### createImageField



  Create a virtual-dom image data-field for use with
  [data-ui](https://github.com/editdata/data-ui).





  **Parameters**



  -   `options` **Object** options object

      -   `options.display` **Boolean** true for display mode, default is false
  for input mode







  **Examples**



  ```javascript

  var createImageField = require('data-field-image')

  var field = createImageField(options)

  var tree =  field.render(h, props, 'http://example.com/example.jpg')

  ```









  ### createImageField



  Render a virtual-dom image data-field.





  **Parameters**



  -   `h` **function** virtual-dom `h` function



  -   `properties` **Object** properties object for `h`

      -   `properties.display` **Boolean** true for display mode, default is
  false for input mode



      -   `properties.value` **String** any image url



  -   `value` **String** any image url







  **Examples**



  ```javascript

  var createImageField = require('data-field-image')

  var field = createImageField(options)

  var tree = field.render(h, props, 'http://example.com/example.jpg')

  ```





  ## Installation



  ```sh

  npm install data-field-image --save

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
  name: data-field-image
  version: 2.0.0
  author: sethvincent
  bugs:
    url: 'https://github.com/editdata/data-field-image/issues'
  dependencies:
    addhttp: ^1.0.0
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
  homepage: 'https://github.com/editdata/data-field-image'
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
    url: 'git+https://github.com/editdata/data-field-image.git'
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
---

