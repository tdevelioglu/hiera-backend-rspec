require 'rake'
require 'hiera-backend-rspec'
require 'rspec/core/rake_task'
require 'cane/rake_task'

task :default => [:spec, :quality]

RSpec::Core::RakeTask.new do |t|
  t.pattern = 'spec/**/*_spec.rb'
end

Cane::RakeTask.new(:quality) do |cane|
  cane.canefile = '.cane'
end
