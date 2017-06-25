# babel-plugin-transform-react-class-displayname
Babel plugin that injects class' name as `displayName` property.

## Install:

```
  npm i -D babel-plugin-transform-react-class-displayname
```

or

```
  yarn add babel-plugin-transform-react-class-displayname
```

## Usage:

via `.babelrc`

```
{
   "plugins": ["transform-react-class-displayname"],
}
```

via `cli`

```
babel --plugins gtransform-react-class-displayname script.js
```

Note:

If You want to use this plugin with `es2015` preset, you need to install [transform class properties plugin](https://babeljs.io/docs/plugins/transform-class-properties/)


## Example:

In:

```
  const component = class Class1 {
    static displayName = "Class1";
  };

  class Class2 {
    static displayName = "Class2";
  }
```

Out:

```
  const component = class Class1 {
    static displayName = "Class1";
  };

  class Class2 {
    static displayName = "Class2";
  }
```

