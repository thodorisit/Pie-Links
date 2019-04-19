![My image](https://thodorisit.github.io/Pie-Links/source/logo.png)
# Pie-Links

Check out the teaser : https://thodorisit.github.io/Pie-Links/source/

# Instructions
```
Create an empty html file, with the basic tags (head,body).
Create your meta tags. Eg.
  - <meta charset="utf-8">
  - <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1.0">
```
```
Include the pie-links.js script.
This script tag should be included between the <head> tags in your HTML document.
```
```
Open the pie-links.js file and replace the default data in the data object.
```
# Data Object
```
var data = {
	'general' : {
		'logoSrc' : './logo.png',
		'pageBackgroundColor' : '#EDEDED',
		'linkBackgroundColor' : '#eec643',
		'linkTextColor' : '#0A0A0A',
		'searchState' : 'active',
		'searchInputPlaceholder' : 'Search...',
		'noResultNotice' : 'No results...'
	},
	'links' : [
		{
			'name' : "Facebook",
			'url' : "https://facebook.com",
			'openUrlType' : 'new',
			'searchTerms': ['facebook','social media','one']
		},
		{
			'name' : "Instagram",
			'url' : "https://instagram.com",
			'openUrlType' : 'self',
			'searchTerms': ['instagram','social media','two']
		},
		{
			'name' : "Website",
			'url' : "https://website.com",
			'openUrlType' : 'self',
			'searchTerms': ['Website','three']
		}
	]
};
```

# FEATURES

- Logo
```
Change the logo by replacing the path:
- data.general.logoSrc
```

- Website Background Color
```
Change the background color by replacing the hex color code:
- data.general.pageBackgroundColor
```

- Button Link Background Color
```
Change the background color of buttons by replacing the hex color code:
- data.general.linkBackgroundColor
```

- Button Link Font-Text Color
```
Change the font color of buttons by replacing the hex color code:
- data.general.linkTextColor
```

## Search Input
In many cases you might want to have the visitors search through the links. To enable the search feature (as shown on the default Data Object) set 
```
data.general.searchState to "active"
```
Change the search input default text by replacing the string:
```
data.general.searchInputPlaceholder
```
Change the string of "No search results" by replacing the string:
```
data.general.noResultNotice
```

# Links
In order to add/remove links, edit the subarrays of
```
data.links
```

### Link example
```
{
  'name' : "Website",
  'url' : "https://website.com",
  'openUrlType' : 'self',
  'searchTerms': ['Website','three']
}
```
- The "name" string is the text that will be placed on the button-link.
- The "url" string is the destination of the button-link.
- If you want the link to be opened in a new window set "openUrlType" to "new"
- If you have enabled the Search Feature, fill the "searchTerms" array with your prefered keywords, by which the visitor can search through the links.
