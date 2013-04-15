Mapping levees and their stability using the interwebs
=====================================================

Intro
------
In the Netherlands water security is probably the major water issue the country faces as 26% of the country and around 60% of the population is located below sea level, this becomes an issue of national security. 

.. image:: http://www.ijkdijk.nl/images/Grechtdijk2.jpg
[source: http://www.ijkdijk.nl/nl/livedijken/livedijk-utrecht]

Levees, or dikes, serve as a main protection against this water. In the year 2013 it no longer suffices to send people around to the dikes themselves. The levees are now equipped with all kinds of sensors as can be seen in the image below. Sensors are embedded in the levee to make an intelligent artifact.

Data Center
-----------
As a datum the IJkdijk foundation built a levee with all kinds of sensors that could and has been breached without any real danger. The data the sensors yielded now serves as a baseline (IJkdijk is Dutch for: Calibration Levee).

.. image:: http://www.beeldsite.nl/ijkdijk/20080928ijkdijk/slides/DSC04627.JPG

[source: http://www.ijkdijk.nl/en/experiments/macrostability]

If all levees are to be equipped with these sensors this will result in mountains of data to keep track of. At http://nelen-schuurmans.nl we tried to solve this part of the story. With the Dijk Data Service Center (levee data service center), we built a system to store and display all this data.

The sensor data is stored in Cassandra nodes (http://cassandra.apache.org/) with the metadata and the latest values cached in a Postgres/PostGIS database.

