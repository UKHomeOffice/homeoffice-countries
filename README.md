# Typeahead Countries

Exports a list of non-EU countries or EU and non-EU countries for use with [Typeahead Aria](https://github.com/UKHomeOffice/typeahed-aria).

## Country List
Add [Typeahead Countries](https://github.com/UKHomeOffice/typeahead-countries) to the field in your HOF service that requires the list.

Example field in a HOF form service using the Typeahead:
```
'country-select'-step: {
  mixin: 'select',
  className: ['typeahead', 'js-hidden'],
  options: [''].concat(require('typeahead-countries').allCountries),
  legend: {
    className: 'visuallyhidden'
  },
  validate: ['required']
},
```

See [HOF Frontend Assets](https://github.com/UKHomeOfficeForms/hof-frontend-assets) for more details
