---
user: editdata
path: editdata/list-editor
name: list-editor
head: 67236681d6b2ba2d890cac9aa219b5ad43becdce
page: false
readme: >
  # list-editor



  A virtual-dom element for editing a small list of items. The list can be an
  array or flat object.



  [![npm](https://img.shields.io/npm/v/list-editor.svg)](http://npmjs.com/list-editor)



  ## Example



  ```js

  var raf = require('virtual-raf')

  var listEditor = require('list-editor')



  function render (state) {

    function removeItem (e, items) {

      state.items = items

      tree.update(state)

    }



    function onsubmit (e, items, item) {

      state.items = items

      tree.update(state)

    }



    function oninput (e, value) {}



    state.removeItem = removeItem

    state.onsubmit = onsubmit

    state.oninput = oninput



    return listEditor(h, state)

  }



  var tree = raf({ items: {}, keys: true }, render, require('virtual-dom'))

  document.body.appendChild(tree())

  ```



  ## License

  MIT
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
    contributions: 7
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
    contributions: 6
package:
  name: list-editor
  version: 2.0.0
  description: a virtual-dom element for editing a small list of items
  main: index.js
  dependencies:
    get-form-data: ^1.2.2
    is-object: ^1.0.1
    isarray: 0.0.1
    object-array-converter: ^1.0.0
    xtend: ^4.0.0
  devDependencies:
    virtual-dom: ^2.1.1
    virtual-raf: ^2.0.3
  scripts:
    example: budo example.js --live
  repository:
    type: git
    url: 'git+https://github.com/editdata/list-editor.git'
  author: sethvincent
  license: MIT
  bugs:
    url: 'https://github.com/editdata/list-editor/issues'
  homepage: 'https://github.com/editdata/list-editor#readme'
---

