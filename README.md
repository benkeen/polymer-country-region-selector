# polymer-country-region-selector

This a [Polymer](http://www.polymer-project.org/) component for adding country-region dropdowns to your forms. The
component automatically updates the region dropdown with whatever values are appropriate, based on the selection in the
country dropdown.

To make the component as independent as possible from your markup, you can choose to either let the component create
the region dropdown automatically (default), or target your own <select> field. The benefit to the latter is that you
have full control over exactly where the region field is placed in your markup.

### Demo



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
	regionBlankOption="-"
	regionEmptyLabel="Select Region"
	regionValue=""
	regionDropdownName="region" />
```

- **countryEmptyLabel** (default "Select Country"). This is the label for the country dropdown


### License

MIT


### Changelog

- **0.1.0** March 19, initial version.