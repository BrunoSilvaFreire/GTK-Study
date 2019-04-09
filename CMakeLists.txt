cmake_minimum_required(VERSION 3.13)
project(GTK_Study)

include_directories("$ENV{VCPKG_HOME}/installed/x64-windows/include")
link_directories("$ENV{VCPKG_HOME}/installed/x64-windows/lib")
link_libraries(gtk-3.0 glib-2.0 gobject-2.0 gdk-3.0 gmodule-2.0 gio-2.0 gthread-2.0)
set(CMAKE_CXX_STANDARD 17)
add_executable(gtk_study main.cpp)
