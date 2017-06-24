You can access translated languages:

```js
locizify.getLanguages(function(err, lngs) {
  console.warn(lngs);
});

// returns something like
{
  "en": {
    "name": "English",
    "nativeName": "English",
    "translated": {
       "latest": 1, // 100% translated
       "production": 1 // 100% translated
     }
  },
  "de": {
    "name": "German",
    "nativeName": "Deutsch",
    "translated": {
       "latest": 0.8, // 80% translated!!!
       "production":1 // 100% translated
     }
  }
}
```

With this informations you can feed a select or menu.