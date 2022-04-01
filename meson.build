project('gamejammeson', 'cpp',
    version: '0.1.2',
    default_options: ['cpp_std=c++20',
                      'default_library=static'])

version = meson.project_version()
varr = version.split('.')
cdata = configuration_data()
cdata.set('PROJECT_NAME', meson.project_name())
cdata.set('PROJECT_VERSION_MAJOR', varr[0])
cdata.set('PROJECT_VERSION_MINOR', varr[1])
cdata.set('PROJECT_VERSION_PATCH', varr[2])
cdata.set('PROJECT_VERSION_TWEAK', 0)

docopt_dep = dependency('docopt')
ftxui_dep = [dependency('ftxui-component')]
spdlog_dep = dependency('spdlog')
catch2_dep = dependency('catch2')

subdir('src')
subdir('test')
