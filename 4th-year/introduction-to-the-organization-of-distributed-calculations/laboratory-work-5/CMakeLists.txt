cmake_minimum_required(VERSION 3.5)

project(laboratory-work-5 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(laboratory-work-5 main.cpp
  dht/NodeTable.cpp dht/NodeTable.h
  dht/Node.cpp dht/Node.h
  utils/MessageUtils.cpp utils/MessageUtils.h
  utils/HashUtils.cpp utils/HashUtils.h
  storage/Storage.cpp storage/Storage.h
  utils/FileSystemUtils.h utils/FileSystemUtils.cpp)

target_link_libraries(laboratory-work-5 pthread -lssl -lcrypto)
