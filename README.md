# Digitised maps in Trove

[![Frictionless](https://github.com/GLAM-Workbench/trove-maps-data/actions/workflows/frictionless.yaml/badge.svg)](https://repository.frictionlessdata.io/pages/dashboard.html?user=frictionlessdata&repo=repository-demo&flow=frictionless)

This repository contains metadata describing digitised maps in Trove. The methods used in creating the datasets are described in the [Trove Maps](https://glam-workbench.net/trove-maps/) section of the GLAM Workbench.

Files include:

* `single_maps_20230131.csv` – metadata harvested from Trove
* `single_maps_20230131_coordinates.csv` – coordinate strings in the metadata (points and bounding boxes) parsed and converted to decimal values

## `single_maps_20230131.csv`

Contains the following columns:

* `title` – title of the map
* `url` – url to the map in the digitised file viewer
* `work_url` – url to the work in the Trove map category
* `identifier` – NLA identifier
* `date` – date published or created
* `creators` – creators of the map
* `publication` – publication place, publisher, and publication date (if available)
* `extent` – physical description of map
* `copyright_status` – copyright status based on available metadata (scraped from web page)
* `scale` – map scale
* `coordinates` – map coordinates, either a point or a bounding box (format is 'W--E/N--S', eg: 'E 130⁰50'--E 131⁰00'/S 12⁰30'--S 12⁰40')
* `filesize_string` – filesize string in MB
* `filesize` – size of TIFF file in bytes
* `width` – width of TIFF in pixels
* `height` – height of TIFF in pixels
* `copy_role`

## `single_maps_20230131_coordinates.csv`

Contains the following metadata:

* `title` – title of the map
* `url` – url to the map in the digitised file viewer
* `coordinates` – map coordinates, either a point or a bounding box (format is 'W--E/N--S', eg: 'E 130⁰50'--E 131⁰00'/S 12⁰30'--S 12⁰40')

Points or centres derived from bounding box:

* `latitude`
* `longitude`

Bounds of box:

* `north`
* `south`
* `east`
* `west`


