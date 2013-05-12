Java-Jpeg-Geotag-Reader
=======================

Adapted from Metadata-Extractor by Drew Noakes, link: http://drewnoakes.com/code/exif/

This project will read the exif headers from a jpeg file and return a GeoTag class with the location and time the photo was taken. 

### Usage:

    JpegGeoTagReader jpegGeoTagReader = new JpegGeoTagReader();
    File photoFile   = new File(fileName);
    GeoTag geoTag    = jpegGeoTagReader.readMetadata(photoFile);     
    double altitude  = geoTag.getAltitude();
    double latitude  = geoTag.getLatitude();
    double longitude = geoTag.getLongitude();
