namespace :build do
task :pdf do
`bundle exec asciidoctor-pdf -apdf-style=themes/custom-theme.yml -a pdf-fontsdir=themes/fonts DiegoDorta_Resume.adoc -o output/DiegoDorta_Resume.pdf`
end
task :html do
`bundle exec asciidoctor DiegoDorta_Resume.adoc -o output/DiegoDorta_Resume.html`
end
end
desc 'Build all default formats'
task :build => [ 'build:html', 'build:pdf' ]
