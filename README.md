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

```
https://unpkg.com/babel-standalone@6.26.0/babel.min.js  ==>  Babel
```

### use JSX

You must precise teh type into the `<script>` tag

```
    <script type="text/babel">
      ReactDOM.render(
        <h1> Hello world ! </h1>,
        document.getElementById("react-root")
      );
    </script>
```

## Create a component with `class`

For this we use `React.Component` who contains a `render()`method.
This method must `return` something.

exemple of a component with a `class`:

```react
class Hello extends React.Component {
        render() {
          return (
            <div>
              <h1> Hello word ! </h1>
              <p> I am Victor </p>
            </div>
          );
        }
      }
```

we can now use the name component into the ReactDOM instead of write all the HTML code :

```react
  ReactDOM.render(
        <Hello />,
        document.getElementById("react-root"));     
```
