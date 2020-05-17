project('lemon', 'c', version : '59c5679')

# lemon, with -d available

prefix = get_option('prefix')
data_dir = get_option('datadir')
project_name = meson.project_name()
data_file = prefix / data_dir / project_name / 'lempar.c'

executable('lemon',
    'lemon.c',
    c_args : '-DLEMPAR="' + data_file + '"',
    install : true)

install_data('lempar.c')
