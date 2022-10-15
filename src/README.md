# React

React is a JavaScript library for building user interfaces.

## React.Component

They are sub-classes that take parameters (`props`) and return a *hiearchy of views* to display via the `render` method. 

The `render` method returns a description of what we'd like to see on the screen. React then takes the description and displays the result. 

`render` returns a React element. 

>> Most React developers use a special syntax called "JSX" which makes structures easier to write.

example in JSX:

```js
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}
```

>> JSX comes with the full power of JavaScript. You can put any JavaScript expressions within braces inside JSX. Each React element is a JavaScript object that you can store in a variable or pass around in your program.

## Execution
in the terminal: `npx create-react-app my-app`

```
cd my-app
cd src

# If you're using a Mac or Linux:
rm -f *

# Or, if you're on Windows:
del *

# Then, switch back to the project folder
cd ..
```

1. Add a file named index.css in the src/ folder with this CSS code.
2. Add a file named index.js in the src/ folder with this JS code.
3. Add these three lines to the top of index.js in the src/ folder:

```js
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
```

To start the app, in the terminal, in the project folder: `npm start`

in the browser: `http://localhost:3000/`