project('bsdutils-extra', ['c'],
    version: '0.1.0',
    default_options: [
        'c_std=c99', 'warning_level=3', 'buildtype=plain'
    ],
    license: 'BSD-2-Clause',
    meson_version: '>=0.50'
)

libcrypto = dependency('libcrypto', required: true)

# Symlink installation script
install_link = meson.current_source_dir() / 'utils/install-link.sh'

subdir('src')
