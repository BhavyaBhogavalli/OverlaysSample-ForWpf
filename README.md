 # Overlays Sample for Wpf



### Description
Discover how to use Overlays to build up your map, or to add existing basemaps to your application. 
The sample can show the following four basemaps:
  1. Google Maps
  2. Bing Maps
  3. World Kit Maps
  4. Open street Maps

It can display different styles of maps by setting the map type. Note: you do need to have Bing Maps API key and Google Maps API key to be able to use these two basemaps. 

Please refer to [Wiki](http://wiki.thinkgeo.com/wiki/map_suite_desktop_for_wpf) for the details.

![Screenshot](https://github.com/ThinkGeo/OverlaysSample-ForWpf/blob/master/Screenshot.png)

### Requirements
This sample makes use of the following NuGet Packages

[MapSuite 10.0.0](https://www.nuget.org/packages?q=ThinkGeo)

### About the Code
```csharp
map.MapUnit = GeographyUnit.Meter;
WorldStreetsAndImageryOverlay worldOverlay = new WorldStreetsAndImageryOverlay();
worldOverlay.IsVisible = false;
worldOverlay.Projection = WorldStreetsAndImageryProjection.SphericalMercator;
worldOverlay.MapType = WorldStreetsAndImageryMapType.Road;
map.Overlays.Add("World Kit Map", worldOverlay);

GoogleMapsOverlay googleMapOverlay = new GoogleMapsOverlay();
googleMapOverlay.IsVisible = false;
map.Overlays.Add("Google Maps", googleMapOverlay);

BingMapsOverlay bingMapOverlay = new BingMapsOverlay();
bingMapOverlay.ApplicationId = ""; //Please set your application id.
bingMapOverlay.IsVisible = false;
map.Overlays.Add("Bing Maps", bingMapOverlay);

OpenStreetMapOverlay osmOverlay = new OpenStreetMapOverlay();
osmOverlay.IsVisible = false;
map.Overlays.Add("Open Street Map", osmOverlay);
```

### Getting Help

- [Map Suite Desktop for Wpf Wiki Resources](http://wiki.thinkgeo.com/wiki/map_suite_desktop_for_wpf)
- [Map Suite Desktop for Wpf Product Description](https://thinkgeo.com/ui-controls#desktop-platforms)
- [ThinkGeo Community Site](http://community.thinkgeo.com/)
- [ThinkGeo Web Site](http://www.thinkgeo.com)

### Key APIs
This example makes use of the following APIs:

- [ThinkGeo.MapSuite.Wpf.WpfMap](http://wiki.thinkgeo.com/wiki/api/ThinkGeo.MapSuite.Wpf.WpfMap)
- [ThinkGeo.MapSuite.Wpf.GoogleMapsOverlay](http://wiki.thinkgeo.com/wiki/api/ThinkGeo.MapSuite.Wpf.GoogleMapsOverlay)
- [ThinkGeo.MapSuite.Wpf.BingMapsOverlay](http://wiki.thinkgeo.com/wiki/api/ThinkGeo.MapSuite.Wpf.BingMapsOverlay)
- [ThinkGeo.MapSuite.Wpf.OpenStreetMapOverlay](http://wiki.thinkgeo.com/wiki/api/ThinkGeo.Wpf.WinForms.OpenStreetMapOverlay)
- [ThinkGeo.MapSuite.Wpf.WorldStreetsAndImageryOverlay](http://wiki.thinkgeo.com/wiki/api/ThinkGeo.MapSuite.WinForms.WorldStreetsAndImageryOverlay)

### About Map Suite
Map Suite is a set of powerful development components and services for the .Net Framework.

### About ThinkGeo
ThinkGeo is a GIS (Geographic Information Systems) company founded in 2004 and located in Frisco, TX. Our clients are in more than 40 industries including agriculture, energy, transportation, government, engineering, software development, and defense.
