guard :rspec, cli: '--color' do
  watch(%r{^spec/.+_spec\.rb$})
  watch(%r{^lib/(.+)\.rb$})     { |m| "spec/lib/#{m[1]}_spec.rb" }
  watch('spec/spec_helper.rb')  { "spec" }
end

guard 'livereload' do
  watch(%r{^spec/javascripts/.*/(.*)\.js})
  watch(%r{^spec/javascripts/(.*)\.js})
  watch(%r{^javascripts/.*/(.*)\.js})
  watch(%r{^javascripts/(.*)\.js})
end
