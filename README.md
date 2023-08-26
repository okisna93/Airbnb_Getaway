# Airbnb_Getaway

# Cabin Locations Visualization using Folium

This repository contains a Python script that visualizes cabin locations on a map using the Folium library.

## Description

The script utilizes the Folium library to create an interactive map showing the locations of different cabins. It reads cabin data from a CSV file, processes it, and then generates map markers for each cabin with pop-up labels displaying cabin names and numbers.

## Installation

To run this script, you'll need to have Python and the required libraries installed. You can install the necessary libraries using the following command:

```bash
pip install folium pandas
```

# Usage
Clone this repository to your local machine.

Make sure you have a CSV file named cabins_location.txt containing cabin location data in the format:

Lat,Long,CabinName
42.252360,-73.948978,Sima
42.252608,-73.949378,Eli
...
Run the script by executing the following command:

bash
python cabin_visualization.py
The script will generate an interactive HTML map (site_map.html) displaying cabin locations with pop-up labels.

Map Types
You can customize the map type by adding the following code snippet to the script:

folium.TileLayer('Stamen Terrain').add_to(site_map)
folium.TileLayer('Stamen Toner').add_to(site_map)
folium.TileLayer('Stamen Water Color').add_to(site_map)
folium.TileLayer('cartodbpositron').add_to(site_map)
folium.TileLayer('cartodbdark_matter').add_to(site_map)
folium.LayerControl().add_to(site_map)
Uncomment the map type you want to use and run the script again to generate the map with the desired style.

Feel free to contribute to this repository by adding new features or improving existing ones.
