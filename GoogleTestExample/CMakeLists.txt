set(GTEST_ROOT /var/project/gtest)
include_directories(
  /var/project/gtest/include
  )
add_executable(gtest_example gtest_example.cpp)
target_link_libraries(gtest_example
  pthread
  /var/project/gtest/build/libgtest.a
  /var/project/gtest/build/libgtest_main.a
  )

