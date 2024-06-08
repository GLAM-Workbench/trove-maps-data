# trove-maps-data

This dataset contains metadata describing digitised maps in Trove, harvested from the Trove API and other sources.

These datasets were generated using notebooks in the [trove-maps](https://github.com/GLAM-Workbench/trove-maps/) repository.

For more information and documentation see the [Trove digitised maps metadata](https://glam-workbench.net/trove-maps/single-maps-data/) section of the [GLAM Workbench](https://glam-workbench.net).

## Dataset summary
- [single_maps.csv](https://github.com/GLAM-Workbench/trove-maps-data/raw/main/single_maps.csv) (14.8 MB, text/csv)
- [single_maps_coordinates.csv](https://github.com/GLAM-Workbench/trove-maps-data/raw/main/single_maps_coordinates.csv) (7.1 MB, text/csv)


## Dataset details

### [single_maps.csv](https://github.com/GLAM-Workbench/trove-maps-data/raw/main/single_maps.csv)

|                |                                                                                                                                                                                                                          |
|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| date harvested | 2024-06-08                                                                                                                                                                                                               |
| file size      | 14.8 MB                                                                                                                                                                                                                  |
| format         | text/csv                                                                                                                                                                                                                 |
| created by     | <a href='https://github.com/GLAM-Workbench/trove-maps/blob/None/Exploring-digitised-maps.ipynb'>Exploring digitised maps in Trove</a> ([documentation](https://glam-workbench.net/trove-maps/exploring-digitised-maps/)) |
| number of rows | 34844                                                                                                                                                                                                                    |

#### Columns

| name               | type    | description                                                                                                             |
|:-------------------|:--------|:------------------------------------------------------------------------------------------------------------------------|
| `identifier`       | string  | NLA identifier                                                                                                          |
| `title`            | string  | title of the map                                                                                                        |
| `url`              | string  | url to the map in the digitised file viewer                                                                             |
| `work_url`         | string  | url to the work in the Trove map category                                                                               |
| `date`             | string  | date published or created                                                                                               |
| `creators`         | string  | creators of the map                                                                                                     |
| `publication`      | string  | publication place, publisher, and publication date (if available)                                                       |
| `extent`           | string  | physical description of map                                                                                             |
| `copyright_status` | string  | copyright status based on available metadata (scraped from web page)                                                    |
| `scale`            | string  | map scale                                                                                                               |
| `coordinates`      | string  | map coordinates, either a point or a bounding box (format is 'W--E/N--S', eg: 'E 130⁰50'--E 131⁰00'/S 12⁰30'--S 12⁰40') |
| `filesize_string`  | string  | filesize string in MB                                                                                                   |
| `filesize`         | integer | size of TIFF file in bytes                                                                                              |
| `width`            | any     | width of TIFF in pixels                                                                                                 |
| `height`           | any     | height of TIFF in pixels                                                                                                |
| `copy_role`        | string  | code indicating type of download available                                                                              |

### [single_maps_coordinates.csv](https://github.com/GLAM-Workbench/trove-maps-data/raw/main/single_maps_coordinates.csv)

|                |                                                                                                                                                                                                              |
|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| date harvested | 2024-06-08                                                                                                                                                                                                   |
| file size      | 7.1 MB                                                                                                                                                                                                       |
| format         | text/csv                                                                                                                                                                                                     |
| created by     | <a href='https://github.com/GLAM-Workbench/trove-maps/blob/None/parse_coordinates.ipynb'>Parse map coordinates from metadata</a> ([documentation](https://glam-workbench.net/trove-maps/parse-coordinates/)) |
| number of rows | 28779                                                                                                                                                                                                        |

#### Columns

| name          | type   | description                                                                                                                         |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------|
| `title`       | string | title of the map                                                                                                                    |
| `url`         | string | url to the map in the digitised file viewer                                                                                         |
| `coordinates` | string | map coordinates as a string, either a point or a bounding box (format is 'W--E/N--S', eg: 'E 130⁰50'--E 131⁰00'/S 12⁰30'--S 12⁰40') |
| `east`        | number | east bounds of box                                                                                                                  |
| `west`        | number | west bounds of box                                                                                                                  |
| `north`       | number | north bounds of box                                                                                                                 |
| `south`       | number | south bounds of box                                                                                                                 |
| `latitude`    | number | point from coordinates or centre of box                                                                                             |
| `longitude`   | number | point from coordinates or centre of box                                                                                             |## Examples of use



----
Created by [Tim Sherratt](https://timsherratt.au) for the [GLAM Workbench](https://glam-workbench.net)