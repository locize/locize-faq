Depends on your chosen i18n format:

**i18next** -&gt; You can add plurals like for example in english:![](/assets/plurals/i18next.png)using suffix \`\_plural\` to define the plural form. All the plural forms for your target languages will be mapped automatically eg. adding for arabic keys 

key\_0, key\_1, key\_2, key\_3, key\_4, key\_5

To find those plural suffixes for other languages \(in case your reference language is not english\) you can look them up here: 

[https://jsfiddle.net/jamuhl/3sL01fn0/\#tabs=result](https://jsfiddle.net/jamuhl/3sL01fn0/#tabs=result)

  


**ICU** -&gt; plurals are part of the translation -&gt; all conversions to target language are done by locize.  
![](/assets/plurals/icu.png)



**i18n-js** -&gt; uses plural keys in form key.OTHER where the .SUFFIX is from [http://www.unicode.org/cldr/charts/latest/supplemental/language\_plural\_rules.html\#en](http://www.unicode.org/cldr/charts/latest/supplemental/language_plural_rules.html#en) \(same as for i18next converting to target language is done by locize\)![](/assets/plurals/i18njs.png)

