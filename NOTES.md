# Local testing

`npm i docsify-cli now -D` // Local

package.json as follows.

```json
{
  "devDependencies": {
    "docsify-cli": "^4.4.4",
    "now": "^21.0.1"
  },
  "name": "mesh-finland",
  "scripts": {
    "start": "docsify serve docs",
    "deploy": "now -p"
  },
  "files": ["docs"],
  "docsify": {
    "config": {
      "basePath": "https://docsify.js.org/",
      "loadSidebar": true,
      "loadNavbar": true,
      "coverpage": true,
      "name": "docsify"
    }
  }
}
```

then

`npm start`

If last modified date on the page is wrong read this
`https://github.com/pfeak/docsify-updated?tab=readme-ov-file#question`
