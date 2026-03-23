# GoogleTest and GoogleMock sample

This repo demonstrates how using gtest and gmock in zephyr.

This currently relies on a fork of GoogleTest that has few patches
for Zephyr. GoogleTest is already supported by twister but GoogleMock
needs some changes to work in Zephyr.

The samples anre in `tests` folder.
Basically, we are using it to test that GoogleTest and GoogleMock build
and run with Zephyr, but, it also serves as demonstrator.
