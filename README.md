# Install React App

- ## Step 1: Install Node.js and npm

Make sure you have Node.js and npm (Node Package Manager) installed on your computer. You can download them from the official Node.js website: https://nodejs.org/

- ## Step 2: Create a New React App
Open your terminal/command prompt and navigate to the directory where you want to create your React app. Then, run the following command to create a new React app:

```bash
  npx create-react-app my-react-app
```

Replace "my-react-app" with the name you want for your app.

- ## Step 3: Navigate to the App Directory
After the installation is complete, navigate into your app's directory:

```bash
  cd my-react-app
```

- ## Step 4: Start the Development Server
Once you're inside the app's directory, you can start the development server with the following command:

```bash
  npm start
```

This will start the server and open your React app in a new browser window at http://localhost:3000.

- ## Step 5: Explore the Created App
You can now explore the default React app that was created for you. Open a code editor (like Visual Studio Code) and navigate to the src folder. You'll find the main app component in src/App.js.

You can modify this component to build your app. As you make changes, the browser window will automatically refresh to reflect those changes.

- ## Step 6: Making Changes
You can modify the content of the src/App.js file to create your own React components, add styles, and customize your app's functionality.

# React components

- ## Understanding Components
In React, a component is a self-contained module that can have its own state and props (properties). There are two types of components: functional components and class components.

- ## Functional Components

```bash

import React from 'react';

function FunctionalComponent() {
  return (
    <div>
      <h1>Hello Raghavan !</h1>
      <p>This is a functional component.</p>
    </div>
  );
}

export default FunctionalComponent;

```

- ## Class Components

```bash

import React, { Component } from 'react';

class ClassComponent extends Component {
  render() {
    return (
      <div>
        <h1>Hello, {this.props.name}!</h1>
        <p>This is a class component.</p>
      </div>
    );
  }
}

export default ClassComponent;

```

- ## Using Components
Now that we have our components, let's use them in the main application.

```bash

import './App.css';
import ClassComponents from './Components/ClassComponents';
import FunctionComponents from './Components/FunctionComponents';

function App() {
  return (
    <div>
     <FunctionComponents/>
     <ClassComponents/>
    </div>
  );
}

export default App;


```