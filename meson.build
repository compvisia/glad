project('glad', 'cpp', default_options : ['cpp_std=c++20'])

src_files = files(
  'src/glad.cpp',
  'include/glad/glad.h',
  'include/KHR/khrplatform.h',
)

glad_inc = include_directories: include_directories('include')
glad_lib = static_library('glad', src_files, include_directories: glad_inc)

glad_dep = declare_dependency(link_with: glad_lib, include_directories: glad_inc)
