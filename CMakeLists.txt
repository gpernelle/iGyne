cmake_minimum_required(VERSION 2.8.9)

project(iGyne)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/gpernelle/iGyne")
set(EXTENSION_CATEGORY "IGT")

set(EXTENSION_CONTRIBUTORS "Guillaume Pernelle,  Alireza Mehrtash, Lauren Barber, Nabgha Fahrat, Jan Egger, Tobias Penzkofer, Sandy Wells, Sam Song, Xiaojun Chen, Yi Gao, Antonio Damato, Tina Kapur, Akila Viswanathan")

set(EXTENSION_DESCRIPTION "iGyne: It is an open source software for MR-Guided Interstitial Gynecologic Brachytherapy. It enables on-time processing of the intra-operative MRI data via a DICOM connection to the scanner followed by a multi-stage registration of CAD models of the template and the obturator to the patient images. This allows the virtual placement of interstitial needles during the intervention, as well as the detection/labeling of needles in MR images")

set(EXTENSION_ICONURL "https://raw.github.com/gpernelle/iGyne/master/iGyne.png")
set(EXTENSION_SCREENSHOTURLS "https://raw.githubusercontent.com/gpernelle/iGyne/master/LabelingResults.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(iGyne)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
