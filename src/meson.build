rasp_android_sources = [
  'main.c',
  'rasp_android-window.c',
  'rasp_android-application.c',
]

rasp_android_deps = [
  dependency('libadwaita-1', version: '>= 1.0'),
]

gnome = import('gnome')

rasp_android_sources += gnome.compile_resources('rasp_android-resources',
  'rasp_android.gresource.xml',
  c_name: 'rasp_android'
)

executable('rasp_android', rasp_android_sources,
  dependencies: rasp_android_deps,
  install: true,
)
