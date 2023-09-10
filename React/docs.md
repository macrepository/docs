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
    ``"editor.formatOnSave": true``
- Simple React Snippets

## Convert babel to react

-https://babeljs.io

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

Stop at 3-your first react components.mp4
