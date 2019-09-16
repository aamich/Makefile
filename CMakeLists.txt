cmake_minimum_required (VERSION 2.6)
project (Tutorial)
add_executable(Tutorial tutorial.cxx)

########################################
# to build release

mkdir Release
cd Release
cmake -DCMAKE_BUILD_TYPE=Release ..
make

##########################################
#And for Debug (again from the root of the project):

mkdir Debug
cd Debug
cmake -DCMAKE_BUILD_TYPE=Debug ..
make
