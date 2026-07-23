# fylr-plugin-detail-map

A fylr plugin that shows the files of a record on a map in the detail view. Files with GPS coordinates in their technical metadata appear as markers at their capture location. Each marker shows a small preview of the file. A click on a marker opens the file in the asset browser. In fullscreen mode a click enlarges the preview instead. A double click centers the map on the marker.

Other plugins can place additional markers on the map. The location and gazetteer custom data type plugins use this to show their positions.

## Configuration

### Base configuration

The plugin is configured in the base configuration in the group "Map".

* **Show map in detail**: enables the map in the detail view.
* **Display with**: selects the tile provider, either "OpenStreetMaps" or "Mapbox".
* **Mapbox Token**: the access token for the Mapbox API. It is only needed when "Mapbox" is selected.

With Mapbox tiles the map offers a menu. Users can switch between street and satellite view and between local and English labels.

### Field settings

Every file field can be excluded from the map. Open the mask settings of the field and disable the option "Show in map" in the group "Map". By default all file fields are shown on the map.
