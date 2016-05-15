# render_list_geo.pl
Perl script for automatic rendering OSM tiles for renderd+mod_tile with using geographic coordinates (WGS-84)
###Usage:
```perl
./render_list_geo.pl -n <n> -z <z> -Z <Z> -x <x> -X <X> -y <y> -Y <Y>
```
```
where:
<n> - number of concurrent threads
<m> - layer name ( default )
<z> - render tiles from this zoom level
<Z> - render tiles to this zoom level
<x> - render tiles from this latitude
<X> - render tiles to this latitude
<y> - render tiles from this longitude
<Y> - render tiles to this longitude
```
###sample
```perl
#for Ukraine
./render_list_geo.pl -n 2 -z 6 -Z 15 -x 21.8 -X 40.7 -y 44.03 -Y 52.6
#Belgium (using three threads)
./render_list_geo.pl -n 3 -z 6 -Z 16 -x 2.5 -X 6.5 -y 49.4 -Y 51.6
#The Netherlands
./render_list_geo.pl -n 2 -m default -z 0 -Z 5 -y 50.758069 -x 3.275104 -Y 53.662826 -X 7.103310

```
