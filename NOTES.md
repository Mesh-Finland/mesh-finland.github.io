## Local testing


`npm i docsify-cli now -D`  // Local



package.json as follows.
```
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
  "files": [
    "docs"
  ],
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

`node start`