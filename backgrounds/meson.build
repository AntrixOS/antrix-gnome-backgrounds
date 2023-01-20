dataconf = configuration_data()
dataconf.set('BACKGROUNDDIR', backgrounddir)
dataconf.set('datadir', datadir)

backgrounds = [
  'adwaita-d.webp',
  'adwaita-l.webp',
  'blobs-d.svg',
  'blobs-l.svg',
  'design-is-rounded-rectangles-d.webp',
  'design-is-rounded-rectangles-l.webp',
  'drool-d.svg',
  'drool-l.svg',
  'dune-d.svg',
  'dune-l.svg',
  'field-d.svg',
  'field-l.svg',
  'keys-d.webp',
  'keys-l.webp',
  'sky-d.webp',
  'sky-l.webp',
  'nrg-d.webp',
  'nrg-l.webp',
  'skeltronaut-d.webp',
  'skeltronaut-l.webp',
  'astro-d.webp',
  'astro-l.webp',
  'astrochan.webp',
  'planeta.webp',
  'symbolic-d.webp',
  'symbolic-l.webp',
  'truchet-d.webp',
  'truchet-l.webp',
  'vnc-d.webp',
  'vnc-l.webp'
]

install_data(backgrounds, install_dir: backgrounddir)

foreach metadata : [
  'adwaita.xml',
  'blobs.xml',
  'drool.xml',
  'design-is-rounded-rectangles.xml', 
  'dune.xml',
  'field.xml',
  'keys.xml',
  'astro.xml',
  'nrg.xml',
  'astrochan.xml',
  'planeta.xml',
  'skeltronaut.xml',
  'sky.xml',
  'symbolic.xml',
  'truchet.xml',
  'vnc.xml']
  configure_file(
    input: metadata + '.in',
    output: metadata,
    configuration: dataconf,
    install: true,
    install_dir: metadatadir
  )
endforeach
