locize serves flat or nested json depending on the keys in the resource.

Suppose, you have most keys in your translation following the nested scheme (e.g. "login.username", "login.label", etc), then locize serves a resource with nicely nested json:

```json
{
    "login": {
        "label": "Log in",
        "user": "User Name"
    }
}
```

If you now add a key that does contain a space, comma or question mark `/ |,|\?/`. (`"User not found!"`), then the resource returned by locize becomes flat:

```json
{
    "login.label": "Log in",
    "login.user": "User Name",
    "User not found!": "User not found!"
}
```

locize automatically transforms to this flat format if it detects that keys use natural language. This is the default behaviour.


*If you know that you always use flat format, you can select this in the project settings.*
![](/assets/publish_flat.png)