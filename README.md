# Generate lists of intersecting areas and information about them

Input:
1. Spatial data (points, polygons, etc.)
2. Spatial data to check for overlap, e.g. conservation areas, habitat zones

Output: Input spatial data with added columns about overlapping areas and their info

Principle:
User has spatial data that needs to be checked for e.g. conservation area overlap. User can put all input conservation area (or such) datasets
to a single folder, that is iterated layer by layer for a new "Areas" column that lists the name of the layers that intersect input data.
Additional variables can be inspected in similar manner, e.g. if the areas-datasets has a variable named "name", the folder can be iterated
to create a new column "names" that lists all the names mentioned in the overlapping conservation area.

Example additions to the dataframe

| Areas                                      | Names                           | Names2              | Codes         | Zones            |
|--------------------------------------------|---------------------------------|---------------------|---------------|------------------|
| natura_2000__spa_ahvenanmaa, yksityiset_suojelualueet | Signilskär-Märket naturreservat | Signilskär - Märket | SPAFI1400047  | Boreaalinen alue |
| natura_2000__sci_ahvenanmaa_aluemaiset     |                                 | Degersand           | SCIFI1400036  | Boreaalinen alue |
|                                            |                                 |                     |               | Boreaalinen alue |

Additional credits
Copilot
