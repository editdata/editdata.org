---
user: editdata
path: editdata/data-grid
name: data-grid
head: e7332fd16a17594be8dc1cfa23869b96c6176242
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
    contributions: 23
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
    contributions: 2
package:
  name: data-grid
  version: 1.2.0
  description: ''
  main: index.js
  style: style.css
  scripts:
    bundle-example: 'sheetify example/style.css > example/bundle.css'
    example: "budo example/index.js --dir example --live --onupdate 'npm run bundle-example'"
  repository:
    type: git
    url: 'git+https://github.com/editdata/data-grid.git'
  author: sethvincent
  license: MIT
  bugs:
    url: 'https://github.com/editdata/data-grid/issues'
  homepage: 'https://github.com/editdata/data-grid#readme'
  dependencies:
    base-element: ^3.0.1
    data-editor: 'github:editdata/data-editor'
    data-fields: 'github:editdata/data-fields'
    extend: ^3.0.0
    inherits: ^2.0.1
    vdom-thunk: ^3.0.0
    view-list: ^2.0.0
  devDependencies:
    budo: ^6.0.1
    data-editor: 'github:editdata/data-editor'
    data-form: 'github:editdata/data-form'
    sheetify: ^2.0.3
    virtual-raf: ^2.0.3
readme: >-
  # data-grid



  Simple & performant grid editor/viewer for data.



  ## See also



  - [data-editor](https://github.com/editdata/data-editor) – base editor that
  works with data-grid

  - [data-ui](https://github.com/editdata/data-ui) – a collection of resources
  & modules for building interfaces for managing data

  - [view-list](https://github.com/shama/view-list) – this project is a thin
  wrapper around the view-list module

  - [virtual-dom](https://github.com/Matt-Esch/virtual-dom) – data-grid
  & view-list are created using the virtual-dom module



  ## License



  [MIT](LICENSE.md)
page: false
---

