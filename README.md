# polymer-country-region-selector

This a [Polymer](http://www.polymer-project.org/) component for adding country-region dropdowns to your forms. The
component automatically updates the region dropdown with whatever values are appropriate, based on the selection in the
country dropdown.

To make the component as independent as possible from your markup, you can choose to either let the component create
the region dropdown automatically (default), or target your own &lt;select&gt; field. The benefit to the latter is that you
have full control over exactly where the region field is placed in your markup. The default behavior is to just create
the country and region dropdowns next to one another.

### Demo

Check out [http://benkeen.github.io/polymer-country-region-selector/](http://benkeen.github.io/polymer-country-region-selector/).
That contains a bunch of examples of how to configure the component as you want.

### Settings

Here's the list of configurable settings and their default values. Pretty much every is customizable - if you
come across something that isn't, let me know!

```
<country-region-selector
	countryEmptyLabel="Select Country"
	countryValue=""
	countryUseShortcode="false"
	countryDropdownName="country"
	targetRegionDropdownId=""
	regionEmptyLabel="Select Region"
	regionBlankOption="-"
	regionValue=""
	regionDropdownName="region" />
```

- **countryEmptyLabel** - (default "Select Country"). This is the default label for the country dropdown.
- **countryValue** - this lets you specify the default selected country when the page loads.
- **countryUseShortcode** - this determines the value attributes of the select box. By default, the values are the
same as the label - the full country name. If you set this to true, it uses the ISO 3166 2-character short code of
the country.
- **countryDropdownName** - this governs the name attribute of the country dropdown.
- **targetRegionDropdownId** - (default blank). This setting lets you choose to target your own region &lt;select&gt; field
in your markup. If it's set, the component won't create its own region dropdown but modify your own field instead. It
should be the ID of  the element.
- **regionEmptyLabel** - (default "Select Region"). This is used for the default value in the region dropdown, once the
user selects a particular country.
- **regionBlankOption** - (default "-"). This is what appears in the region dropdown prior to the user selecting a
country. It's the only option in the region dropdown at that point.
- **regionValue** - this lets you define the default value of the region on page load. Note: you MUST also have the
countryValue to have been set as well, and the regionValue must belong to the selected country.
- **regionDropdownName** - (default "region"). The name attribute of the region field.

### License

MIT

### Changelog

- **0.1.1** June 22, minor update for Bower
- **0.1.0** May 26, initial version.