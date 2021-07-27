# REACT OBJECT PROGRAMMING

## Add React and ReactDOM into the html file :

```
 https://unpkg.com/react@16/umd/react.development.js ==> React
 https://unpkg.com/react-dom@16/umd/react-dom.development.js ==> ReactDOM
```

## render()

```
<div id="react-root"></div>

<script>

ReactDOM.render( react.createElement (), getElemetById("react-root"))
React.createElement(ELEMENT, PROPRIETY, ELEMENT'S CHILDREN)

</script>
```

## render() with JSX

JSX = JavaScript Syntax Extension

### add babel

must add babel to write html code into a JavaScript code

````
https://unpkg.com/babel-standalone@6.26.0/babel.min.js  ==>  Babel

```

exemple :

```javascript
    <div id="react-root"></div>

    <script type="text/babel">
      ReactDOM.render(
        <h1> Hello world ! </h1>,
        document.getElementById("react-root")
      );
    </script>
````
