# offline-country-reverse-geocoder [![Build Status](https://travis-ci.org/daveross/offline-country-reverse-geocoder.svg?branch=master)](https://travis-ci.org/daveross/offline-country-reverse-geocoder)

Determine which country a lat/long point falls in

Essentially a PHP fork of https://github.com/bencampion/reverse-country-code

## Examples

```
echo 'Washington DC is in ' . \com\davidmichaelross\country_reverse_geocoder\get_country(-77.0164, 38.9047) . "\n";
echo 'Chicago is in ' . \com\davidmichaelross\country_reverse_geocoder\get_country(-87.6847, 41.8369) . "\n";
echo 'London is in ' . \com\davidmichaelross\country_reverse_geocoder\get_country( -0.12750, 51.50722 ) . "\n";
echo 'New Delhi is in ' . \com\davidmichaelross\country_reverse_geocoder\get_country( 77.12, 28.38 ) . "\n";
echo 'Sydney is in ' . \com\davidmichaelross\country_reverse_geocoder\get_country( 151.2073200, -33.8678500 ) . "\n";
```

##Dataset

This library uses the world borders dataset from [thematicmapping.org](http://thematicmapping.org/downloads/world_borders.php). The data is stored in a properties file within the jar file that maps country codes to Well Known Text format polygons and multi-polygons. The dataset was converted to Well Known Text format by [GIS Stack Exchange user, elrobis](http://gis.stackexchange.com/a/17441).

##License

This library is released under a [Creative Commons Attribution-Share Alike License](http://creativecommons.org/licenses/by-sa/3.0/).
