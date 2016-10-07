# The Bird Clear Sky Model
The Bird Clear Sky Model, authored by Richard Bird, is a broadband algorithm which produces estimates of clear sky direct beam, hemispherical diffuse, and total hemispherical solar radiation on a horizontal surface. The Excel@ Spreadsheet implementation was done by Daryl Myers. The model is based on comparisons with results from rigourous radiative transfer codes. It is composed of simple algebraic expressions with 10 user provided inputs. Model results should be expected to agree within ± 10% with rigourous radiative transfer codes. The model computes hourly average solar radiation for every hour of the year, based on the 10 user input parameters; however variable atmospheric parameters such as Aerosol Optical Depth, Ozone, Water vapor are fixed for the entire year.


# References
Bird, R. E., and R. L. Hulstrom, Simplified Clear Sky Model for Direct and Diffuse Insolation on Horizontal Surfaces, Technical Report No. SERI/TR-642-761, Golden, CO: Solar Energy Research Institute, 1981

---
# Error Note
BEFORE 2101 GMT 08-16-2012

Users who downloaded the BIRD CLEAR SKY model spreadsheet before 08/16/2012 should correct Column H, the HOUR ANGLE CALCULATION. Cell H3, and all others in column H, where Hour angle is calculated, needed re-arrangement of parameters in the equation in order to calculate solar noon correctly. [NOTE: the value 12.5 represents shift of solar geometry calculations to midpoint of the hour ending at hour indicated]

The incorrect formula reads: 

        =15*((C3-12.5)+(($A$13)*15-($A$11))*(4/60)+G3/60)

The correct, simplified formula reads: 

        =15*(C3-12.5)+($A$11)-($A$13)*15+G3/4 

and will produce HA results different from the previous version.

The CORRECTED spreadsheet is available as of 8/16/2012; or users can make corrections by unprotecting the workbook and pasting the correct equation in column H.

To correct a version downloaded before 18:00 GMT on 08/16/2012: UNPROTECT the sheet (Password BIRD); edit H3 by inserting the correct equation, and copying down the column. Then Re-protect the sheet (best to use the same password, BIRD).

Our apologies for any inconvenience.

Click [here](http://rredc.nrel.gov/solar/models/clearsky/error_reports.html) to see all error reports.

---

# Download the model
The model is available via the [Renewable Resource Data Center (RReDC) website](http://rredc.nrel.gov/solar/models/clearsky/BIRD_08_16_2012.xls). It will be available via GitHub at a later date.

# History
This page was transferred to GitHub from [RReDC](http://rredc.nrel.gov/solar/models/clearsky/) on 7 October 2016 By Andrew Clifton.

# Disclaimer
Please see the [NREL disclaimer and copyright notice](http://www.nrel.gov/disclaimer.html).

