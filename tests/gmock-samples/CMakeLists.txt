cmake_minimum_required(VERSION 3.20.0)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(googlemock-samples)

set(GTURTLE_SAMPLES_SRC ../../../gturtle)
include_directories(${GTURTLE_SAMPLES_SRC})

target_sources(app PRIVATE
  ${GTURTLE_SAMPLES_SRC}/tests/test_turtle.cc
)

