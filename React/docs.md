# ------------Prepare environment-------------

1. install node
2. npm i -g create-react-app
3. create-react-app my-app or npx reate-react-app my-app (use npx if it's not accessible)
4. npm start

# -----------------TOOLS----------------------

## VScode Editor extensions

- Simple React Snippets
- Pretier
  add in vs-code-setting:
  `"editor.formatOnSave": true`
- Simple React Snippets

## Convert babel to react

-https://babeljs.io

## Debugger Browser

- React Developer Tools

# -------------------Explanations----------------

##Install React App (use this to hide complex configurations from babel)
npm i -g create-react-app
npm i -g create-react-app@xxxx <-------------When Specify versions

##Create react app environment
npx create-react-app my-app

npm start <----------- start the environment
npm eject <----------- to show complex configuration (cannot undone) and customize configurations

# -----------------ES6 Refresher--------------

- Use **let** and **const** only. **let** if you need to change the value. Use **var** only when **this** is not accessible or any valid reasons.
- **this** is not always available. Use **bind** instead.
- **bind** is to use when **this** is not accessible especially when wrapping some standalone javascript fuinctions.
- **Arrow function** (=>) don't rebind the this keywork.
- **array map** (colors.map) modified the array into new array values like concatenating in every array data.
- **Object destructuring** (const {name, age:a } = person;) to remove repeative initialization/codes.
- **Spread operators** (... [...colors] or {...persons}) is to combine arrays or objects into new set of data whether it is array or objects.
- **class** is to make a blueprint of the objects and easier to maintain.
- **inheritance** is to inherit other objects and omit redundant methods. Use **super** if both objects is using a constructor
- **modules** is set by private in default. Use **export** to make it public and use **import** to use it in other modules.
- **name and default exports** is to export all objects by name
  Default -> import ... from '';
  Named -> import { ... } from '';

# -------------------Components-------------------

Javascript will return the last condition when truthy
ex. true && 'hello' <----- Output: hello

- JSX: Javascript XML template
- Rendering Lists
- Conditional rendering
- Handling events

Handling Events - do not pass the functon reference
ex. <button onClick={this.handleIncrement}>Increment</button>

If it's needs to pass an argument needs to use the inline function for wrapper to pass the arguments
ex. <button onClick={ () => this.handleIncrement({product: 1})}>Increment</button>

Inside the class component use **constructor** to bind **this** object to a function.
Or use **arrow function** in order to retain the access to the **this** object

- Updating the state

In react if you want to update the value of an object, You cannot directly update like this **this.state.count++** instead use this **this.setState({count: this.state.count + 1})**

# -------------------Composing Components-------------------

Passing datat to components
ex:
Send value:
`<Counter value={counter.value}>`

Receive Value:
`this.props.value`

- State is localy and internally to the component. Private and invisible to other component

- props in the input to the component, It is read-only

13 - Stateless Functional Components.mp4

https://drive.google.com/file/d/13R2u29TA6o70JHUrP32gh6B9EkSiClTz/view?usp=drive_link
