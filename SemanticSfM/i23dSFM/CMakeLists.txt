ADD_SUBDIRECTORY(cameras)
ADD_SUBDIRECTORY(exif)
ADD_SUBDIRECTORY(features)
ADD_SUBDIRECTORY(graph)
ADD_SUBDIRECTORY(image)
ADD_SUBDIRECTORY(linearProgramming)
ADD_SUBDIRECTORY(geometry)
ADD_SUBDIRECTORY(matching)
ADD_SUBDIRECTORY(matching_image_collection)
ADD_SUBDIRECTORY(multiview)
ADD_SUBDIRECTORY(numeric)
ADD_SUBDIRECTORY(robust_estimation)
ADD_SUBDIRECTORY(tracks)
ADD_SUBDIRECTORY(color_harmonization)
ADD_SUBDIRECTORY(system)
ADD_SUBDIRECTORY(sfm)
ADD_SUBDIRECTORY(stl)

#INSTALL RULES
INSTALL(
  DIRECTORY .
  DESTINATION include/i23dSFM
  COMPONENT headers
  FILES_MATCHING PATTERN "*.hpp" PATTERN "*.h"
)
