cmake_minimum_required(VERSION 3.0)

project(install_a_project)
add_subdirectory(src bin)
install(FILES ${PROJECT_BINARY_DIR}/bin/install_a_project 
  DESTINATION bin
  PERMISSIONS OWNER_EXECUTE GROUP_EXECUTE
  )  

