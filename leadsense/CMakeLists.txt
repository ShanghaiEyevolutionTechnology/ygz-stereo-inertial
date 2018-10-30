find_package(EvoBinoSDK REQUIRED)

include_directories(${EvoBinoSDK_INCLUDE_DIRS})

add_executable(leadsense leadsense.cpp)
target_link_libraries(leadsense ${STEREOCAMERA_LIBS} ${YGZ_LIBS} ${THIRD_PARTY_LIBS})

add_executable(leadsense_imu leadsense_imu.cpp)
target_link_libraries(leadsense_imu ${STEREOCAMERA_LIBS} ${YGZ_LIBS} ${THIRD_PARTY_LIBS})
