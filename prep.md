Create project folder

```
cd desktop
mkdir group-project
cd group-project
```

Install express app into an empty folder

```
npx express-generator --no-view --force
```

Install packages

```
npm install
npm install nodemon --save-dev
```

Edit bin/www, change port to 3001

- Before
  - `var port = normalizePort(process.env.PORT || '3000');`
- After
  - `var port = normalizePort(process.env.PORT || '3001');`

Edit bin/www, add port output at bottom

- Before
  - `debug('Listening on ' + bind);`
- After
  - ```
    debug('Listening on ' + bind);
    console.log('Listening on ' + bind);
    ```

Edit package.json so that start command runs nodemon

- Before
  - `"start": "node ./bin/www"`
- After
  - `"start": "nodemon ./bin/www"`

Test it!
`npm start`

View it!
`localhost:3001`

Stop it!
`CTRL + C`

# React

create app

```
npx create-react-app client
```

remove /client/.git

update package.json

- Before
  - `"start": "react-scripts start",`
- After (windows)
  - `"start": "set PORT=3001 && react-scripts start",`
- After (mac)
  - `"start": "PORT=3001 && react-scripts start",`
