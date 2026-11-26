https://storage.googleapis.com/geomap-documents/GeoMap_Beta_User_Guide.pdf

## Subsurface favorability
Web based GIS platform for geothermal resources, including a subsurface favorability layer that calculated a favorability score ($1-5$) based on several geological inputs. The score recognise the local geology and tectonic processes significantly influence local heat flow, and is compiled through a consortium of subsurface geothermal experts.

- Shear wave speed at 100km depth (according to a global tomographic model from (Schaeffer and Lebedev 2013). There is a high spatial correlation between negative velocity perturbations and plate boundaries and deformations zones)
- Global heat flow in ($mW/m^2$)
- Active faults, merging fata from different datasets in QGIS
- Proximity to volcanoes and vents (using different datasets in QGIS)

![[Screenshot 2026-11-26 143433.png]]

Further, the subsurface favorability and slope of the local geography is merged through the equation $$subsurface-favourability*0.9+slope-score*0.1$$
Data was validated against existing geothermal sites the 
