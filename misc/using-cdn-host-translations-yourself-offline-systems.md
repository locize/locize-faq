# Using our CDN or using custom solutions

While you get most comfort out of using our CDN your environment might demand you to bundle the translations with your product (eg. offline usage in areas with restricted internet access).

Using our **CDN** has two big **advantages**:

- you can deploy updates to translations without the need to redeploy/rollout a new version of your application
- during development, testing you can set your versions to auto publishing. Doing so your translation changes are reflected immediately in your application and results in a lot easier development process.

# Download the translations

If your product demands to download the translations, because you need or prefer to host or bundle them yourself you can do so. Using our CDN is completely options and get only billed if you're using it.

Options to download the translations:

- Using our web applications
- Using the [API](https://docs.locize.com/api.html) or [locize-cli](https://docs.locize.com/cli.html)

**Recommendation**

We highly encourage you to at least use the CDN during development as it makes your work on translating your product a lot more efficient. Just bundle or change the [i18next backend implementation](https://www.i18next.com/plugins-and-utils.html#backends) during production.