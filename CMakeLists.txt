cmake_minimum_required(VERSION 2.8.9)

project(MyFirstSlicerExtension)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/JunjieBai/MyFirstSlicerExtension")
set(EXTENSION_CATEGORY "learning")
set(EXTENSION_CONTRIBUTORS "Junjie Bai (UIowa)")
set(EXTENSION_DESCRIPTION "Junjie's first extension")
set(EXTENSION_ICONURL "https://raw.github.com/JunjieBai/MyFirstSlicerExtension/master/MyFirstSlicerExtension.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/MyFirstSlicerExtension/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(lineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
