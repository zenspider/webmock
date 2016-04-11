source 'http://rubygems.org/'

gemspec
if ENV["EM_HTTP_REQUEST_0_X"]
  gem 'em-http-request', '~> 0.3.0'
end

group :development do
  gem 'rake', '~> 10.5.0' if RUBY_VERSION < '1.9.3'
  gem 'rake' if RUBY_VERSION >= '1.9.3'
end

group :test do
  gem 'minitest_tu_shim', '1.3.2'
end

platforms :jruby do
  gem 'jruby-openssl'
  gem 'manticore', '< 0.5.5'
end


gem 'curb', '< 0.9.2'  unless RUBY_PLATFORM =~ /java/ #https://github.com/taf2/curb/issues/296
