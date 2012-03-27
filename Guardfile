# Check for SASS updates and push them locally and into any built site
guard 'sass', :input => '_sass', :output => 'css', :style => :compact
guard 'sass', :input => '_sass', :output => '_site/css', :style => :compact

# Check for any other updates and refresh Jekyll in that case
guard 'rake', :task => 'jekyll' do
  watch(%r{^(_includes/|_posts/|_layouts/|_config\.yml|robots.txt|sitemap.xml|[^/]*\.(?:html|markdown|textile))})
end

# TODO: Watch for JS file changes and rebuild the JS section
# TODO: Implement jsmin of some type

# vim: filetype=ruby
