source ENV['GEM_SOURCE'] || "https://rubygems.org"

group :development, :unit_tests do
  gem 'rake',                                              :require => false
  gem 'rspec',                                             :require => false
  gem 'rspec-puppet',                                      :require => false
  gem 'puppetlabs_spec_helper',                            :require => false
  gem 'metadata-json-lint',                                :require => false
  gem 'puppet-lint',                                       :require => false
  gem 'puppet-lint-unquoted_string-check',                 :require => false
  gem 'puppet-lint-empty_string-check',                    :require => false
  gem 'puppet-lint-spaceship_operator_without_tag-check',  :require => false
  gem 'puppet-lint-absolute_classname-check',              :require => false
  gem 'puppet-lint-undef_in_function-check',               :require => false
  gem 'puppet-lint-leading_zero-check',                    :require => false
  gem 'puppet-lint-trailing_comma-check',                  :require => false
  gem 'puppet-lint-file_ensure-check',                     :require => false
  gem 'puppet-lint-version_comparison-check',              :require => false
  gem 'puppet-lint-file_source_rights-check',              :require => false
  gem 'puppet-lint-alias-check',                           :require => false
  gem 'rspec-puppet-facts',                                :require => false
  gem 'ruby-augeas',                                       :require => false
  gem 'puppet-blacksmith',                                 :require => false if RUBY_VERSION !~ /^1\./
  gem 'json_pure', '< 2.0.2',                              :require => false
  gem 'ruby-augeas',                                       :require => false
end

group :system_tests do
  gem 'beaker',               :require => false
  gem 'beaker-rspec', '> 5',  :require => false
  gem 'beaker_spec_helper',   :require => false
  gem 'serverspec',           :require => false
  gem 'specinfra',            :require => false
end

if facterversion = ENV['FACTER_GEM_VERSION']
  gem 'facter', facterversion, :require => false
else
  gem 'facter', :require => false
end

if puppetversion = ENV['PUPPET_GEM_VERSION']
  gem 'puppet', puppetversion, :require => false
else
  gem 'puppet', :require => false
end

# vim:ft=ruby
