namespace :build do
task :pdf do
`bundle exec asciidoctor-pdf -apdf-style=themes/custom-theme.yml -a pdf-fontsdir=themes/fonts DiegoDorta_CV.adoc -o output/DiegoDorta_CV.pdf`
end
task :html do
`bundle exec asciidoctor DiegoDorta_CV.adoc -o output/DiegoDorta_CV.html`
end
end
desc 'Build all default formats'
task :build => [ 'build:html', 'build:pdf' ]
