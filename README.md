## Pedestrian Route Generator Works

This application creates a walking/running route that matches a target distance and elevation profile. Users provide a starting point, a distance, route type, and elevation preference. The generator tries multiple routes until it finds a route close to what was requested.

### Process
1. Take the input coordinate, target distance, route type, and elevation preference.
2. Randomly generates waypoints around the starting point/
3. Requests a walking route from OpenRouteService API using waypoints.
4. Measures the route distance and elevation gain.
5. Compare it to user preferences.
6. Repeats up to 10 times until preferences are met. 

### Outputs
- A GeoJSON route displayed on a Mapbox basemap.
- The measured distance.
- Elevation gain.

### Link
[Link to Route Generator](https://greg-kohler.github.io/routegenerator/)
