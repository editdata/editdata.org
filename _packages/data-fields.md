---
user: editdata
path: editdata/data-fields
name: data-fields
head: 97251127ef29f4b494f39c68868d44248fe8c758
package:
  name: data-fields
  version: 3.0.1
  description: ''
  main: index.js
  scripts:
    lint: standard
    test: 'npm run lint && zuul -- ./tests/*.js'
    test-local: 'npm run lint && zuul --local 8080 -- ./tests/*.js'
    budo: budo examples/index.js --dir examples --live
    example: 'npm run build-example && npm run budo'
    build-example: 'npm run build-example-js & npm run build-example-css '
    build-example-js: 'browserify examples/index.js > examples/bundle.js'
    build-example-css: postcss -u autoprefixer -o examples/bundle.css examples/index.css
    deploy: 'npm run build-example && gh-pages -d examples'
  repository:
    type: git
    url: 'git+https://github.com/editdata/data-fields.git'
  keywords:
    - virtual-dom
    - data
    - element
    - dom
  author: sethvincent
  license: MIT
  bugs:
    url: 'https://github.com/editdata/data-fields/issues'
  homepage: 'https://github.com/editdata/data-fields#readme'
  dependencies:
    addhttp: ^1.0.0
    data-field-classname: ^1.0.0
    leaflet: ^0.7.7
    leaflet-draw: ^0.2.4
    list-editor: ^1.0.2
    object-array-converter: ^1.0.0
    xtend: ^4.0.1
  devDependencies:
    autoprefixer: ^6.3.3
    browserify: ^13.0.0
    budo: ^8.1.0
    data-form: ^1.1.1
    gh-pages: ^0.11.0
    postcss-cli: ^2.5.1
    standard: ^6.0.7
    tap-spec: ^4.1.1
    tape: ^4.5.1
    virtual-dom: ^2.1.1
    virtual-raf: ^3.0.0
    zuul: ^3.10.0
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
    contributions: 14
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
    contributions: 4
readme: >
  # data-fields



  Render fields for various types of input.



  [![npm](https://img.shields.io/npm/v/data-fields.svg)](http://npmjs.com/data-fields)



  ## Installation



  ```sh

  npm install data-fields --save

  ```



  ## API



  * [string](#string)

  * [number](#number)

  * [url](#url)

  * [list](#list)

  * [image](#image)

  * [geoJSON](#geoJSON)



  ### <a name="string"></a> fields.string(h, options[, value])



  Create a field to display text.  If `editable` is set to true the text will be
  placed inside a `textarea` element.



  **Arguments**

    * `h` - A `hyperscript` style DOM builder

    * `options` - Options object.

      * `options.editable` - `Boolean` - Set whether the value is editable or
  not. Defaults to true.

      * `options.size` - `String` - Set the size of the field. Defaults to
  `normal`, other possible choices are `small` and `large`.

      * `options.value` - `String` - The value of the field.

      * `options.*` - Extra properties will be passed to the DOM builder when
  creating the field.

    * `value` - `String` - Value of the field.  Takes precedence over
  `options.value`



  **Example**



  ```js

  var fields = require('data-fields')

  var h = require('virtual-dom/h')

  var stringField = fields.string(h, { className: 'MyField' }, 'Some string')

  ```



  ### <a name="number"></a> fields.number(h, options[, value])



  Create a field to display a number.  If `editable` is set to true the value
  will be placed inside an `input` element with `type` set to `number`.



  **Arguments**

    * `h` - A `hyperscript` style DOM builder

    * `options` - Options object.

      * `options.editable` - `Boolean` - Set whether the value is editable or
  not. Defaults to true.

      * `options.value` - `Number` - The value of the field.

      * `options.*` - Extra properties will be passed to the DOM builder when
  creating the field.

    * `value` - `Number` - Value of the field.  Takes precedence over
  `options.value`



  **Example**



  ```js

  var fields = require('data-fields')

  var h = require('virtual-dom/h')

  var numberField = fields.number(h, { className: 'MyField' }, 1000)

  ```



  ### <a name="url"></a> fields.url(h, options[, value])



  Create a field to display a url.  If `editable` is set to true the url will be
  placed inside an `input` element.  If `editable` is set to false the url will
  be displayed as an `a` element.



  **Arguments**

    * `h` - A `hyperscript` style DOM builder

    * `options` - Options object.

      * `options.editable` - `Boolean` - Set whether the value is editable or
  not. Defaults to true.

      * `options.value` - `String` - The value of the field.

      * `options.*` - Extra properties will be passed to the DOM builder when
  creating the field.

    * `value` - `String` - Value of the field.  Takes precedence over
  `options.value`



  **Example**



  ```js

  var fields = require('data-fields')

  var h = require('virtual-dom/h')

  var urlField = fields.url(h, { className: 'MyField' }, 'http://example.com')

  ```



  ### <a name="list"></a> fields.list(h, options[, value])



  Create a field to display a list, either from an array or an object.  If
  `editable` is set to true
  [list-editor](https://github.com/editdata/list-editor) will be used to display
  the list.



  **Arguments**

    * `h` - A `hyperscript` style DOM builder

    * `options` - Options object.

      * `options.editable` - `Boolean` - Set whether the value is editable or
  not. Defaults to true.

      * `options.value` - `Array|Object` - The value of the field.

      * `options.*` - Extra properties will be passed to the DOM builder when
  creating the field.

    * `value` - `Array|Object` - Value of the field.  Takes precedence over
  `options.value`.



  **Example**



  ```js

  var fields = require('data-fields')

  var h = require('virtual-dom/h')

  var listField = fields.list(h, { className: 'MyField' }, ['a', 'b', 'c'])

  ```



  ### <a name="image"></a> fields.image(h, options[, value])



  Create a field to display an image.  If `editable` is set to true the image's
  path will be placed inside an `input` field.  If `editable` is set to false the
  image itself will be displayed.



  **Arguments**

    * `h` - A `hyperscript` style DOM builder

    * `options` - Options object.

      * `options.editable` - `Boolean` - Set whether the value is editable or
  not. Defaults to true.

      * `options.value` - `String` - The value of the field.

      * `options.*` - Extra properties will be passed to the DOM builder when
  creating the field.

    * `value` - `String` - Value of the field.  Takes precedence over
  `options.value`



  **Example**



  ```js

  var fields = require('data-fields')

  var h = require('virtual-dom/h')

  var imageField = fields.image(h, { className: 'MyField' },
  'http://example.com/example.jpg')

  ```



  ### <a name="geoJSON"></a> fields.geoJSON(h, options[, value])



  Create a field to display geoJSON data on a [leaflet](http://leafletjs.com/)
  map.  If `editable` is set to true the map will include drawing controls.



  **Arguments**

    * `h` - A `hyperscript` style DOM builder

    * `options` - Options object.

      * `options.accessToken` - `String` - Mapbox access token if you'd like to
  use Mapbox.

      * `options.tileLayer` - `String` - Leaflet tile layer to use.

      * `options.imagePath` - `String` - Path to leaflet images.

      * `options.editable` - `Boolean` - Set whether the value is editable or
  not. Defaults to true.

      * `options.value` - `Object` - The value of the field.

      * `options.*` - Extra properties will be passed to the DOM builder when
  creating the field.

    * `value` - `Object` - Value of the field.  Takes precedence over
  `options.value`



  **Example**



  ```js

  var fields = require('data-fields')

  var h = require('virtual-dom/h')



  var geoJSON = {

    type: 'Feature',

    geometry: {

      type: 'Point',

      coordinates: [-122.33636, 47.621958]

    }

  }



  var geoField = fields.geoJSON(h, { className: 'MyField' }, geoJSON)

  ```





  ## Tests



  ```sh

  npm install

  npm test

  ```



  ## License



  [MIT](LICENSE.md)
page: 'http://about.editdata.org/data-fields/'
---

