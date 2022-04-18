 
set(PWM_SOURCES mbed_PWMServoDriver.cpp) 
add_library(mbed_PWMServoDriver STATIC ${PWM_SOURCES})
target_link_libraries( mbed_PWMServoDriver mbed-os)

set(PWM_HEADER_DIR ${CMAKE_CURRENT_SOURCE_DIR} )
target_include_directories(mbed_PWMServoDriver PUBLIC ${PWM_HEADER_DIR})