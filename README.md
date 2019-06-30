# GeoServer configuration from you metadata catalogue

If you are describing where the spatial resources of your organization are in metadata records
(eg. network file path, database connection) use this job to automatically analyze the content
of your catalogue and publish your data in GeoServer.

The process support the following formats:

* shp
* sqlite
* geopackage
* postgis
* tiff

All files/tables MUST be visible to the GeoServer instances.

For one file resources, if an SLD is available next to the geo resource, then the SLD
is used to configure the layer style in GeoServer.

Information from the metadata (ie. title, abstract) are added to the layer configuration.

The process can start from scratch on each run or restart only on updated records since last run.
