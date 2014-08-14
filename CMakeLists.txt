# added a root level CMakeLists.txt 
# to make this repo work with cmakes externalproject module
CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT ( openexr_root )

add_subdirectory(IlmBase)
INCLUDE_DIRECTORIES ( 
  IlmBase/Iex 
  IlmBase/IexMath 
  IlmBase/Imath 
  IlmBase/Half 
  IlmBase/config 
  IlmBase/IlmThread)
add_subdirectory(OpenEXR)