---
user: editdata
path: editdata/data-editor
name: data-editor
head: f4e13b60c981033cda463c07a60c3a3921443285
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
    contributions: 29
readme: >-
  # data-editor



  An opinionated collection of methods for managing the state of browser-based
  data-editing applications.



  ## About



  ### Format



  ### Validate



  ### Rows



  ### Properties



  ### Metadata



  ## Install



  ```

  npm install --save data-editor

  ```



  ## API



  ## License

  [MIT](LICENSE.md)
package:
  name: data-editor
  version: 1.0.0
  description: an editor for tabular data built with virtual-dom and base-element
  main: index.js
  directories:
    test: tests
  scripts:
    test: 'tape tests/*.js | tap-spec'
    test-browser: 'budo tests/*.js -- -t [ envify --NODE_ENV development ]'
    example-grid-css: 'sheetify examples/grid/style.css > examples/grid/bundle.css'
    example-grid: "budo examples/grid/index.js --live --onupdate 'npm run example-grid-css' --dir examples/grid -- -t [ envify --NODE_ENV development ]"
    example-map-css: 'sheetify examples/map/style.css > examples/map/bundle.css'
    example-map: "budo examples/map/index.js --live --onupdate 'npm run example-map-css' --dir examples/map -- -t [ envify --NODE_ENV development ]"
  repository:
    type: git
    url: 'git+https://github.com/editdata/data-editor.git'
  keywords:
    - data
    - editor
  author: sethvincent
  license: MIT
  bugs:
    url: 'https://github.com/editdata/data-editor/issues'
  homepage: 'https://github.com/editdata/data-editor#readme'
  dependencies:
    clone: ^1.0.2
    component-emitter: ^1.2.0
    cuid: ^1.3.8
    is-my-json-valid: ^2.12.3
    type-of: ^2.0.1
    xtend: ^4.0.1
  devDependencies:
    budo: ^5.1.5
    data-form: 'github:editdata/data-form'
    data-grid: editdata/data-grid
    data-map: editdata/data-map
    documentation-readme: ^2.0.0
    envify: ^3.4.0
    level-js: ^2.2.2
    levelup: ^1.2.1
    mapbox.js: ^2.2.2
    request: ^2.64.0
    sheetify: ^2.0.3
    virtual-dom: ^2.1.1
    xhr: ^2.1.0
page: false
---

