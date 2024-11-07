# Flags Color API

Flags Color API is a JSON API that given an [ISO 3166](http://www.iso.org/iso/home/standards/country_codes.htm) `country_code`, let you get:
* `country_name`: Country name (English)
* `country_code`: Country code [ISO 3166](http://www.iso.org/iso/home/standards/country_codes.htm)
* `rgb`: Red Green Blue (RGB) color values
* `hex`: Hexadecimal color values
* `pantone`: [Pantone](https://www.pantone.com) color names

Example:
```shell
curl https://flags-color-api-ooanazvqci.now.sh/flags/fra
```
```json
{
  "country_name": "France",
  "country_code": "fra",
  "rgb": [{ "r": 0, "g": 85, "b": 164 },
          { "r": 255, "g":255, "b":255 },
          { "r": 239, "g": 65, "b": 53}],
  "hex": ["#0055A4", "#FFFFFF", "#EF4135"],
  "pantone": ["Reflex Blue C", "White", "Red 032 C"]
}
```

## Contribute: Add or edit a flag
If you'd like to add a new flag or fix an error, please feel free to either:
* Submit an issue
* Submit a pull request
* Contact me on Twitter: @vjo


=======

// Assuming we have a predefined list of flag colors 
```const flagColors = { 'bz': ['#00ABDF', '#FFFFFF', '#D52B1E'], // Belize 
'cr': ['#002B7F', '#FFFFFF', '#CE1126'], // Costa Rica
'sv': ['#0047AB', '#FFFFFF', '#0047AB'], // El Salvador
'gt': ['#4997D0', '#FFFFFF', '#4997D0'], // Guatemala
'hn': ['#0073CF', '#FFFFFF', '#0073CF'], // Honduras
'ni': ['#0067C7', '#FFFFFF', '#0067C7'], // Nicaragua
'pa': ['#005AA7', '#FFFFFF', '#D52B1E'] // Panama };```
