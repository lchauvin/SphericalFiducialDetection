
#-----------------------------------------------------------------------------
set(MODULE_NAME SphericalFiducialDetection)

#-----------------------------------------------------------------------------
set(MODULE_INCLUDE_DIRECTORIES
  HoughTransform
  GaussianNoise
  )

set(MODULE_SRCS
  )

set(MODULE_TARGET_LIBRARIES
  ${ITK_LIBRARIES}
  )

#-----------------------------------------------------------------------------
SEMMacroBuildCLI(
  NAME ${MODULE_NAME}
  TARGET_LIBRARIES ${MODULE_TARGET_LIBRARIES}
  INCLUDE_DIRECTORIES ${MODULE_INCLUDE_DIRECTORIES}
  ADDITIONAL_SRCS ${MODULE_SRCS}
  )

