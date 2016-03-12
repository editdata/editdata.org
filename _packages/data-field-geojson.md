---
user: editdata
path: editdata/data-field-geojson
name: data-field-geojson
head: 68f391d00c0362205f076c89a92311fbbed1e1d6
readme: >
  # data-field-geojson



  ## API



  ### createGeoJSONField



  Create a virtual-dom geojson data-field for use with
  [data-ui](https://github.com/editdata/data-ui).





  **Parameters**



  -   `options` **Object** an options object, including any properties you can
  pass to leaflet & virtual-dom/h

      -   `options.accessToken` **String** mapbox access token for using their
  API



      -   `options.tileLayer` **Object** Leaflet tilelayer, default is osm tiles



      -   `options.imagePath` **String** path to leaflet images



      -   `options.display` **Boolean** true for display mode, default is false
  for input mode







  **Examples**



  ```javascript

  var createGeoJSONField = require('data-field-geojson')

  var field = createGeoJSONField(options)

  field.render(h, {}, geojsonObject)

  ```









  ### field.render



  Render the virtual-dom geojson data-field.





  **Parameters**



  -   `h` **function** virtual-dom `h` function



  -   `properties` **Object** an options object, including any properties you can
  pass to leaflet & virtual-dom/h

      -   `properties.display` **Boolean** true for display mode, default is
  false for input mode



      -   `properties.value` **Object** a geojson Feature or Featurecollection



  -   `value` **Object** a geojson Feature or Featurecollection







  **Examples**



  ```javascript

  var createGeoJSONField = require('data-field-geojson')

  var field = createGeoJSONField(options)

  field.render(h, properties, geojsonObject)

  ```



  ## Installation



  ```sh

  npm install data-field-geojson --save

  ```



  Or install the [data-fields](https://github.com/editdata/data-fields) module:

  ```sh

  npm install data-fields --save

  ```



  Right now this module relies on leaflet v1.0.0-beta2, and you must build the
  dependency manually:



  ```

  cd node_modules/leaflet

  npm install

  npm run build

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
    contributions: 4
package:
  name: data-field-geojson
  version: 2.0.1
  author: sethvincent
  bugs:
    url: 'https://github.com/editdata/data-field-geojson/issues'
  dependencies:
    component-emitter: ^1.2.0
    data-field-classname: ^1.0.0
    leaflet: ^0.7.7
    leaflet-draw: ^0.2.3
    xtend: ^4.0.0
  devDependencies:
    budo: ^5.1.5
    data-editor: 'github:editdata/data-editor'
    data-form: 'github:editdata/data-form'
    documentation-readme: ^2.0.0
    standard: ^5.3.1
    tap-spec: ^4.1.0
    tape: ^4.2.2
    virtual-dom: ^2.1.1
    virtual-raf: ^2.0.3
  homepage: 'https://github.com/editdata/data-field-geojson'
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
    url: 'git+https://github.com/editdata/data-field-geojson.git'
  scripts:
    docs: 'documentation-readme README.md -s "API" -- index.js'
    example-basic: 'budo -d examples examples/basic.js:bundle.js --live'
    example-widget: 'budo -d examples examples/widget.js:bundle.js --live'
    example-form: 'budo -d examples examples/form.js:bundle.js --live'
    test: 'standard && tape tests/*.js | tap-spec'
  style: style.css
page: false
---

