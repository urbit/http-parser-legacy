project('http-parser', 'c', version : '0.1.0')

version = meson.project_version()

inc = include_directories('./')
lib = static_library('http_parser', sources: ['http_parser.c'], version: version,
include_directories: inc,
c_args: [
'-Wall',
'-Wextra',
'-Werror',
'-Wno-unused-parameter',
'-O2'
])

http_parser_dep = declare_dependency(include_directories : inc,
  link_with : lib)
