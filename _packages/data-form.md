---
user: editdata
path: editdata/data-form
name: data-form
head: a994939810e777be790b5b90e7a06347c7d4d337
package:
  name: data-form
  version: 1.0.0
  description: ''
  main: index.js
  style: style.css
  scripts:
    docs: 'documentation-readme README.md -s "API" -- index.js'
    example-css: 'sheetify example/style.css > example/bundle.css'
    example: "budo example/index.js --dir example --live --onupdate 'npm run example-css'"
    test: 'tape test.js | tap-spec'
  repository:
    type: git
    url: 'git+https://github.com/editdata/data-form.git'
  keywords:
    - data-ui
  author: sethvincent
  license: MIT
  bugs:
    url: 'https://github.com/editdata/data-form/issues'
  homepage: 'https://github.com/editdata/data-form#readme'
  dependencies:
    base-element: ^3.0.1
    component-emitter: ^1.2.0
    data-editor: 'github:editdata/data-editor'
    data-fields: ^2.0.0
    data-format: 'github:editdata/data-format'
    inherits: ^2.0.1
  devDependencies:
    budo: ^5.1.5
    data-editor: 'github:editdata/data-editor'
    documentation-readme: ^2.1.0
readme: "#data-form\n\nGenerate a form from the row of a dataset and it's JSONSchema-style properties.\n\n## Install\n\n    npm i --save editdata/data-form\n\n## API\n\n### createDataForm\n\nCreate a form from the row of a dataset and its properties\n\n**Parameters**\n\n-   `options` **Object** \n    -   `options.header` **Boolean** \n    -   `options.header` **Object** virtual-dom vtree that should be used for the header\n\n### form.render\n\nCreate a form from the row of a dataset and its properties\n\n**Parameters**\n\n-   `state` **Object** \n    -   `state.activeRow` **Object** \n\n## License\n\n[MIT](LICENSE.md)\n"
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
    contributions: 5
page: false
---

