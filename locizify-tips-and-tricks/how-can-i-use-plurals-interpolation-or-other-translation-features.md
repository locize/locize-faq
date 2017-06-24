You can pass i18next-options:

Interpolation:

```html
<div i18next-options='{"foo": "bar"}'>
  foo {{bar}}
  <p i18next-options='{"foo2": "bar2"}'>foo {{foo}}; foo2 {{foo2}}</p>
</div>
```

*Options get inherited from parent to child nodes.*

Plural:

```html
<p i18next-options='{"count": 2}'>plural {{count}} items</p>
```

Learn more about translation features: [i18next.t](https://www.i18next.com/essentials.html)