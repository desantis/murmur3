project('murmur3', 'c', version : '0.1.0')

version = meson.project_version()

inc = include_directories('./')

lib = static_library('murmur3', sources: ['murmur3.c'], version: version,
include_directories: inc,
c_args: ['-Wall', '-ffast-math'],
install: false)

murmur3_dep = declare_dependency(include_directories : inc,
  link_with : lib)
