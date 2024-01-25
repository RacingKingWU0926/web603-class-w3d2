# web603-class-w3d2

## Getting started

### Step 1: Initiate A React App
Run
```bash
$ npx create-react-app crud-json-server
```

### Step 2: Install Dependencies and Check Configs
Run
```bash
$ npm i -D json-server concurrently
```

And then make sure that `crud-json-server/package.json` contains
```json
  "devDependencies": {
    "concurrently": "^8.2.2",
    "json-server": "^1.0.0-alpha.22"
  }
```
*(version might be different)*

and has `"json-server"` and `"dev"` added by you based on the instruction.
```json
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject",
    "json-server": "json-server --watch db.json --port 5000",
    "dev": "concurrently \"npm start\" \"npm run json-server\""
  }
```
