Sometimes while consuming the API it returns with a status code 400, "Body not valid! The passed json is nested too deeply."

What's the reason for this error?

##### The locize API generally only accepts flat json.

For example this would not be a valid body:

```json
{
  "new": {
    "key": "default value"
  },
  "another": {
    "existing": {
      "key": "another changed value",
      "phrase": "another value"
    }
  }
}
```

this has to be sent like this:

```json
{
  "new.key": "default value",
  "another.existing.key": "another changed value",
  "another.existing.phrase": "another value"
}
```


##### optional context (the exception):
In case you want to also save a context information for a specific translation, you can define a nested object like this:


```json
{
  "new.key": {
    "value": "default value",
    "context": {
      "text": "description for this key"
    }
  },
  "another.existing.key": "another changed value",
  "another.existing.phrase": "another value"
}
```
`"default value"` is now defined as nested value for the `"new.key"` key. And next to the `"value"` property there is the `"context"` property containing an object having a `"text"` property describing the context for `"new.key"` key.



*For more information consult the [API documentation](https://docs.locize.com/api.html#updateremove-translations).*