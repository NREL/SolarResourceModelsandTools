# The Bird Simple Spectral Model

The [Bird Simple Spectral Model](http://rredc.nrel.gov/solar/pubs/spectral/model), authored by Dr. Richard Bird and Dr. Carol Riordan, computes clear sky spectral direct beam, hemispherical diffuse, and hemispherical total irradiances on a prescribed receiver plane - tilted or horizontal - at a single point in time. For tilted planes, the user specifies the incidence angle of the direct beam ([FORTRAN version](http://rredc.nrel.gov/solar/pubs/spectral/model/appendix.html)) or the tilt and azimuth of the plane (Excel@ and C versions). The wavelength spacing is irregular, covering 122 wavelengths from 305 nm to 4000 nm. Aerosol optical depth, total precipitable water vapor (cm), and equivalent ozone depth (cm) must be specified by the user. No variations in atmospheric constituents or structure are available. There is no separate computation of circumsolar radiation. The direct beam spectral irradiance is assumed to contain the circumsolar radiation within a 5° solid angle. No smoothing functions are provided.

# References

* Bird, R.E., and C. Riordan, Simple Solar Spectral Model for Direct and Diffuse Irradiance on Horizontal and Tilted Planes at the Earth's Surface for Cloudless Atmospheres, [Technical Report No. SERI/TR-215-2436](http://www.nrel.gov/docs/legosti/old/2436.pdf), Golden, CO: Solar Energy Research Institute, 1984
* Bird, R. E., and Riordan, C. J. (1986). "Simple Simple Solar Spectral Model for Direct and Diffuse Irradiance on Horizontal and Tilted Planes at the Earth's Surface for Cloudless Atmospheres." Journal of Climate and Applied Meteorology. Vol. 25(1), January 1986; pp. 87-97.

# Download the model

Three versions of the model are available on the RReDC:

* [spectrl2](http://rredc.nrel.gov/solar/models/spectral/spectrl2)
Version 2, revised 24 March 2004. 
A simple solar spectral model in C code based on SERI (now NREL) technical report SERI/TR-215-2436

* [SPCTRAL2](http://rredc.nrel.gov/solar/models/spectral/SPCTRAL2)
An Excel@ Spreadsheet implementation done by Daryl Myers using equations from the technical report.

* [SPCTRAL2_PC](http://rredc.nrel.gov/solar/models/spectral/SPCTRAL2_PC)
The original Bird SPCTRAL2 code listed in the Appendix of technical report SERI/TR-215-2436 was compiled using Lahey FORTRAN V 4.5 to create an executable for PC platform. This exectuable is available [here for download  in a ZIP file](http://rredc.nrel.gov/solar/models/spectral/SPCTRL2.ZIP) complete with auxiliary files for running the program.

# Suggested sources for model input parameters

Suggested links for most difficult to find input data (Aerosol Optical Depth Precipitable Water Vapor, Ozone) for Spectral modeling:

* [NASA AERONET](http://aeronet.gsfc.nasa.gov/) 
In particular the Climatology Tables give climalogical estimates of aerosol optical depths and precipitable water vapor.
* [NASA Ozone sounder data](http://jwocky.gsfc.nasa.gov/ozone/ozone_v8.html)

# History
This page was transferred to GitHub from [RReDC](http://rredc.nrel.gov/solar/models/spectral/) on 7 October 2016 By Andrew Clifton.

# Disclaimer
Please see the [NREL disclaimer and copyright notice](http://www.nrel.gov/disclaimer.html).
