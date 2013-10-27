
$:.unshift File.dirname(__FILE__) + 'lib'
$:.unshift './lib', './spec'

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new
task :default => :spec

desc "Ejecutar las espectativas de la clase Fraccion"
task :local do
  sh "rspec -Ilib -Ispec spec/fraccion_spec.rb"
end


