# CMakeList.txt : projet CMake pour pong, incluez la source et définissez
# la logique spécifique au projet ici.
#
cmake_minimum_required (VERSION 3.8)

include_directories(Include)
link_directories(Lib/x64/)

# Ajoutez une source à l'exécutable de ce projet.
add_executable (pong "pong.cpp" "pong.h")

target_link_libraries(pong SDL2main SDL2)

#penser a copier la SDL2.dll en version 64b dans le dossier de l'executable