load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

prebuilt_cxx_library(
  name = 'brigand',
  header_only = True,
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', 'brigand/**/*.hpp'),
    ('include/standalone', '**/*.hpp'),
  ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
