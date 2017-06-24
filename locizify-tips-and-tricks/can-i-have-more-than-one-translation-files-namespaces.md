Sure, there are multiple options to set the namespace:

### set a namespace on init

The simplest method is to set a different namespace on init:

```js
locizify.init({
  namespace: 'myNamespace'
});
```

### configure locizify to create a namespace per url

Another option is to separate namespaces per route - so each page gets a own translation file:

```js
locizify.init({
  namespaceFromPath: true
});
``` 