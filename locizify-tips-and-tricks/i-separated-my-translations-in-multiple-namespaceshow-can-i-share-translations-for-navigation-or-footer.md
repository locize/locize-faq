On init of locizify you can load additional namespaces (files).

```js
locizify.init({
  ns: ['common']
});
```

You can set an element and all it's children to use translations from a different namespace by setting i18next-options:

```html
<div i18next-options='{"ns": "common"}'>
  <p>different namespace common is used</p>
  <p>all the way down</p>
</div>
```