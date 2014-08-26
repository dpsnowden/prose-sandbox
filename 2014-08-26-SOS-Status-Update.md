This document summarizes the current state of IOOS SOS work as of 2014-08-26.  It was drafted for the ODIP project but will serve other purposes.

# Standards and Technical Guidelines

List here the SOS standards, the templates, existing documentation using both old and new links.

NOTE: The IOOS technical documentation is undergoing reorganization.  Whenever possible this document provides both an old and new link to relevant documentation.

## Prior Standards 
From 2007 - 2011 IOOS coordinated a development effort focused on the SOS 1,0 family of standards (SOS 1.0, SWE, 1.0, SensorML 1.0, and O&M 1.0).  This development resulted in operational SOS services deployed at both the [NOAA National Data Buoy Center (NDBC)](http://sdf.ndbc.noaa.gov/sos/) and at the [NOAA Center for Operational Oceanographic Products and Services (CO-OPS)](http://opendap.co-ops.nos.noaa.gov/ioos-dif-sos/) that still exist today.  

The output provided by these services comes in several forms.  The output for a **GetCapabilities** request is standard OWS Common Capbilities.xml.  The output for the **DescribeSensor** request is SensorML 1.0 XML tailored to specific IOOS use cases.  This SensorML is basic in structure and minimal in content.  The output for a **GetObservation** request can take several forms, the most common form is a Comma (or Tab) Separated Value output ([Old Docs](https://geo-ide.noaa.gov/wiki/index.php?title=IOOS_Conventions_for_CSV_and_TSV_Encoding) || [New Docs](https://github.com/ioos/ioos-csv-tsv)).  An additional output format that is more descriptive and hence verbose is based on GML 3.1.1 and is described [here](http://www.ioos.noaa.gov/gml/schema.html).  Please note, the GML based output format has been deprecated and is no longer maintained, though the NDBC and CO-OPS servers still publish data using this format.

## Current Standards and Output Templates
Starting in about 2012, and based primarily on [community feedback](http://www.ioos.noaa.gov/library/ioos_dif_assmnt_report_final.pdf), IOOS began development of a new output format which was more succinct and better aligned with existing standards (esp the [Climate and Forecast Conventions for netCDF: Discrete Sampling Geometries](http://cfconventions.org/)).  The development process and older versions of the documentation are hosted on the [IOOSTech Google Code](https://code.google.com/p/ioostech/) site.  This site is being retired and will be replaced by a collection of individual Github repositories.  The top level repository will be published at http://ioos.github.io.  The SOS Guidelines and corresponding templates will be at the [sos-guidelines](https://github.com/ioos/sos-guidelines) repository.  

These templates are still based on the SOS 1.0 family of standards but rather than encoding the data elements from a **GetObservations** request as GML, SWE Common 1.0 is adopted instead.  The templates themselves are available at [old docs](https://code.google.com/p/ioostech/source/browse/#svn%2Ftrunk%2Ftemplates%2FMilestone1.0) and eventually at the new [home](https://github.com/ioos/sos-guidelines).  These templates are currently versioned as *Milestone 1.0*.  The versioning scheme is not intentionally kept in synch with the underlying OGC standards, though in this case both the IOOS templates and the underlying SOS standards are v1.0.

# Software Implementations

## i52N Stack
Include both the SOS server itself and the supporting harvesting and testing code.


## ncSOS
Unidata will integrate into THREDDS

## Generic Deployment Model
Explain the diagram that shows how a side by side deployment might look.


# Deployment Status
List links to Geoportal searches.  Don't try to link to all 



