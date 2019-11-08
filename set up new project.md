### setup new project

- `npm init -y`
- `npm install -D parcel-bundler sass eslint posthtml`
- erstelle `.htmlhintrc`
  mit Inhalt: 
  ```
  {
    "doctype-first": false; 
}
```

-erstelle `.nowignore``
  mit Inhalt: 
  ```
  cache
dist
node_modules
```

- erstelle `git ignore`mit "node_modules, .cache, dist, .DS_Store"
- dev script package json
  ```
  "scripts": {
    "dev": "parcel src/*.html",
    "build": "parcel build src/*.html",
    "test": "jest",
    "test-watch": "jest --watch"
  },
  ```
- erstelle `src` ordner
- `npm run dev`
