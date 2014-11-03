file(GLOB GPUJPEG_SRCS    "*.cpp" "*.cu")
file(GLOB GPUJPEG_HEADERS "*.h" "*.cuh")

cuda_add_library(GPUJPEG SHARED ${GPUJPEG_SRCS} ${GPUJPEG_HEADERS})

# Install Rules	
install (TARGETS GPUJPEG DESTINATION "bin")
    