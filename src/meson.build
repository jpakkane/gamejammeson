configure_file(input: 'mygame-config.hpp.meson',
    output: 'mygame-config.hpp',
    configuration: cdata)

executable('intro', 'main.cpp',
    dependencies: [docopt_dep, ftxui_dep, spdlog_dep])
