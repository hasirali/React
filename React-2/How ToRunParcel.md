# Create JSON

```
npm init -y
```

Installing Packages
``` 
npm install -D parcel
npm install react react-dom

```
run
```
npx parcel index.html
```

# Create HTML File

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Parcel App</title>
</head>
<body>
  <h1>Hello Parcel!</h1>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>React + Parcel App</title>
</head>
<body>
  <div id="root"></div>
  <script type="module" src="index.js"></script>
</body>
</html>
```

# Create index.js

```
import React from 'react';
import ReactDOM from 'react-dom';

const App = () => {
  return (
    <h1>Hello React + Parcel!</h1>
  );
};

ReactDOM.render(<App />, document.getElementById('root'));

```


# Script mai change

```

"scripts": {
    "start": "parcel index.html --hmr",
    "build": "parcel build index.html",
    "test": "jest"
  },

```
