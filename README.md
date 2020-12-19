# mobile.geodatabase

Sample mobile geodatabase, contains countries table (source http://www.naturalearthdata.com/downloads/10m-cultural-vectors/).

To use ST_Geometry functions do the following:

```
$ sqlite mobile.geodatabase
$ SELECT load_extension('./libstgeometry_sqlite.so','SDE_SQL_funcs_init');
$ select st_Area(shape) from countries;
```

Database support files: 

C:\Program Files (x86)\ArcGIS\Desktop10.3\DatabaseSupport\SQLite\Linux64
C:\Program Files (x86)\ArcGIS\Desktop10.3\DatabaseSupport\SQLite\Windows64
