# bfs-fix

```
java -jar /Users/stefan/apps/ili2gpkg-5.0.1/ili2gpkg-5.0.1.jar --dbfile wahlresultate_ai.gpkg --defaultSrsCode 2056 --nameByTopic --strokeArcs --createFk --models CH_BFS_Wahlresultate_20231109 --modeldir "." --schemaimport
```

```
java -jar /Users/stefan/apps/ili2gpkg-5.0.1/ili2gpkg-5.0.1.jar --dbfile wahlresultate_ai.gpkg --models CH_BFS_Wahlresultate_20231109 --modeldir "." --disableValidation --export fubar.xtf
```

```
java -jar /Users/stefan/apps/ilivalidator-1.13.3/ilivalidator-1.13.3.jar fubar.xtf
```

## -----

```
java -jar /Users/stefan/apps/ili2gpkg-5.0.1/ili2gpkg-5.0.1.jar --dbfile hoheitsgebiete.gpkg --defaultSrsCode 2056 --nameByTopic --strokeArcs --createFk --models CH_Swisstopo_RealSwissBoundaries_20231113 --modeldir "." --schemaimport
```

```
java -jar /Users/stefan/apps/ili2gpkg-5.0.1/ili2gpkg-5.0.1.jar --dbfile hoheitsgebiete.gpkg --models CH_Swisstopo_RealSwissBoundaries_20231113 --modeldir "." --disableValidation --export hoheitsgebiete.xtf
```

```
java -jar /Users/stefan/apps/ilivalidator-1.13.3/ilivalidator-1.13.3.jar hoheitsgebiete.xtf
```

## ----

```
java -jar /Users/stefan/apps/ilivalidator-1.13.3/ilivalidator-1.13.3.jar --config config.ini hoheitsgebiete.xtf wahlresultate_ai.xtf
```