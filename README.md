# polymer-country-region-selector

This a [Polymer](http://www.polymer-project.org/) component for adding country-region dropdowns to your forms. The
component automatically updates

To make the component as independent as possible from your markup, you can choose to either


### Settings

```
<country-region-selector
	country-empty-label="Select Country"
	country-value="CA"
	country-shortcode="true"
	region-dropdown-id=""
	region-blank-option="--"
	region-empty-label="Select Region"
	region-value="British Columbia" />
```

### Regular HTML attributes
You can add whatever additional HTML attributes you want, just like it's a standard HTML element, e.g.

```
<country-region-selector
	...
	id="countryField"
	onclick="alert('Country selected!')"
	class="whatevs-man"
	...
	/>
```
