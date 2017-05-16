cmake_minimum_required(VERSION 3.0)

include("cmake/HunterGate.cmake")
HunterGate(
    URL "https://github.com/ruslo/hunter/archive/v0.18.58.tar.gz"
    SHA1 "3b39effc5ee1af4ef7487eabb1b0a7a7e10a7b3e"
    LOCAL
)

project(foo)

hunter_add_package(TIFF)
find_package(TIFF CONFIG REQUIRED)
