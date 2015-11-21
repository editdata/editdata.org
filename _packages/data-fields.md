---
user: editdata
path: editdata/data-fields
name: data-fields
head: 1ef077634333c35a5a20c8c2950aa3b1b7feafa0
readme: "# data-fields \n\nA collection of data field modules for use with [data-ui](https://github.com/editdata/data-ui) modules.\n\n## Installation\n\n```sh\nnpm install data-fields --save\n```\n\n## API of each field\n\nAll fields have at least the following API:\n\n```\nfield.on('update', function (e, value) {\n  // update state of application with new value\n  state.value = value\n})\n\nfield.render(h, { value: state.value })\n```\n\n## Dependencies\n\n- [data-field-geojson](https://github.com/editdata/data-field-geojson)\n- [data-field-image](https://github.com/editdata/data-field-image)\n- [data-field-list](https://github.com/editdata/data-field-list)\n- [data-field-string](https://github.com/editdata/data-field-string)\n- [data-field-url](https://github.com/editdata/data-field-url)\n\n## License\n\nMIT\n"
package:
  name: data-fields
  version: 2.0.1
  description: ''
  main: index.js
  scripts: {}
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
    data-field-geojson: ^2.0.1
    data-field-image: ^2.0.0
    data-field-list: ^2.0.0
    data-field-string: ^2.0.0
    data-field-url: ^2.0.0
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
page: false
---

