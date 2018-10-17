 # project name and programming language
    project('com.github.smotynb.helloworld', 'vala', 'c')

    # Create a new executable, list the files we want to compile, list the dependencies we need, and install
    executable(
        meson.project_name(),
        '~/Projects/gtk-hello/src/Application.vala',
        dependencies: [
            dependency('gtk+-3.0')
        ],
        install: true
    )

    #Install our .desktop file so the Applications Menu will see it
    install_data(
        join_paths('data', meson.helloworld() + '.desktop'),
        install_dir: join_paths(get_option('datadir'), 'applications')
    )

    #Install our .appdata.xml file so AppCenter will see it
    install_data(
        join_paths('data', meson.helloworld() + '.appdata.xml'),
        install_dir: join_paths(get_option('datadir'), 'metainfo')
    )
