---
user: editdata
path: editdata/data-map
name: data-map
head: db0cb3201eba3048b03f591dcc7dd9be6f92e5ae
readme: "# data-map\n\nShow a dataset on a map.\n\n## Install\n\n```\nnpm install --save data-map\n```\n\n## Usage\n\n```\nvar h = require('virtual-dom/h')\n\nvar state = {\n  properties: {},\n  data: [\n    {\n      key: 'uuid',\n      value: {\n        pizza: true,\n        awesome: 'this string is awesome',\n        howManyPizzas: 27\n      }\n    }\n  ]\n} \n\nvar map = require('data-editor/map')({\n  zoom: 16,\n  center: [47.621958, -122.33636],\n  accessToken: 'your mapbox access token'\n})\n\nvar mapView = map.render(state)\nvar container = h('div.map-container', [mapView])\n```\n\n## See also\n\n- [data-editor](https://github.com/editdata/data-editor) – base editor that works with data-grid\n- [data-ui](https://github.com/editdata/data-ui) – a collection of resources & modules for building interfaces for managing data\n- [data-grid](https://github.com/editdata/data-grid) - simple & performant grid editor/viewer for data\n- [view-list](https://github.com/shama/view-list) – this project is a thin wrapper around the view-list module\n- [virtual-dom](https://github.com/Matt-Esch/virtual-dom) – data-grid & view-list are created using the virtual-dom module\n\n## License\n\n[MIT](LICENSE.md)"
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
  name: data-map
  version: 1.0.0
  description: ''
  main: index.js
  style: style.css
  scripts: {}
  repository:
    type: git
    url: 'git+https://github.com/editdata/data-map.git'
  author: sethvincent
  license: MIT
  bugs:
    url: 'https://github.com/editdata/data-map/issues'
  homepage: 'https://github.com/editdata/data-map#readme'
  dependencies:
    base-element: ^3.0.1
    component-emitter: ^1.2.0
    inherits: ^2.0.1
    leaflet: ^0.7.5
    mapbox.js: ^2.2.2
    virtual-leaflet: ^1.0.0
page: false
---

