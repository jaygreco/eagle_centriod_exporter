# eagle_centriod_exporter

Easily export X,Y placement data for automated PCB assembly within EAGLE.

# Why?

The "Screaming Circuits" ULP that ships with EAGLE is in inches. What if you want mils or mm? What if you want to deliberately ignore parts marked as DNP?

# How?

Simply run export_centroid_mils.ulp or export_centroid_mm.ulp. To mark a part as NOPOP, create an attribute with name "BOM_DNP" and value "DNP". The export ULP will ignore it when creating the placement file.
