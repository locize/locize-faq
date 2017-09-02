We agree on the focus of locize is translation of software / applications / websites / etc. 
Project management plays a big role in the process of getting translations ready for the upcoming release.
We would more say it lets everyone focus on their job, i.e. developers in writing code instead of merging translation files, while translators can focus on the translation job.

### How to handle
What a project manager expects from being used to document translation, is uploading a document (word, eps, pdf whatever) and to be able to translate that.
Based on the different focus of locize you create a namespace which is our term for a technical set of translations. On that namespace you can start importing translations using technical formats (json, po, yaml, xliff, xml, ...). But developers will instrument their code so new segments will be added automatically by using the API or our [i18n framework](https://i18next.com). So there will be a constant flow of new segments during development and you can start immediately with the translations.
So in best case developers will only login to locize to fix typos in initial source language. 
From there the translation / terminology responsible (PM) will pick up and check consistency using the built in translation memory. After that he or she will ping the translators for translation / or order via included agencies / or export new segments and sent them for translation to their partners - import again what comes back from them.