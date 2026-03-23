cmake_minimum_required(VERSION 3.20.0)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(googletest-samples)

set(GTEST_SAMPLES_SRC ../../../googletest/googletest/samples/)
target_sources(app PRIVATE
  ${GTEST_SAMPLES_SRC}/sample1.cc
  ${GTEST_SAMPLES_SRC}/sample2.cc
  ${GTEST_SAMPLES_SRC}/sample3_unittest.cc
)
