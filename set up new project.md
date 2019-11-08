### setup new project

- `npm init -y`
- `npm install -D parcel-bundler sass eslint posthtml`
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
