source "https://rubygems.org"

# GitHub Pages gem - includes Jekyll and all supported plugins
gem "github-pages", group: :jekyll_plugins

# just-the-docs theme for local development
gem "just-the-docs"

# Windows and JRuby compatibility
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance booster for watching directories on Windows
gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]

# Lock http_parser.rb to v0.6.x on JRuby builds
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
