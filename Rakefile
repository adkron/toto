require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "toto-haml"
    gem.summary = %Q{the tiniest blog-engine in Oz}
    gem.description = %Q{the tiniest blog-engine in Oz.}
    gem.email = "amos.l.king@gmail.com"
    gem.homepage = "http://github.com/adkron/toto"
    gem.authors = ["cloudhead", "Amos King"]
    gem.add_development_dependency "riot"
    gem.add_dependency "builder"
    gem.add_dependency "rack"
    gem.add_dependency "rdiscount"
    gem.add_dependency "haml"
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: sudo gem install jeweler"
end

require 'rake/testtask'
Rake::TestTask.new(:test) do |test|
  test.libs << 'lib' << 'test'
  test.pattern = 'test/**/*_test.rb'
  test.verbose = true
end

task :test => :check_dependencies
task :default => :test
