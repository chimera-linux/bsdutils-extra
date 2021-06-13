project('bsdutils-extra', ['c'],
    version: '0.1.0',
    default_options: [
        'c_std=c99', 'warning_level=3', 'buildtype=plain'
    ],
    license: 'BSD-2-Clause',
    meson_version: '>=0.50'
)

libcrypto = dependency('libcrypto', required: true)
pthread = dependency('threads')

# Symlink installation script
install_link = meson.current_source_dir() / 'utils/install-link.sh'

conf_data = configuration_data()

conf_data.set('PROJECT_VERSION', '"' + meson.project_version() + '"')

configure_file(output: 'config.h', configuration: conf_data)

inc_main = include_directories('.')

subdir('src')
