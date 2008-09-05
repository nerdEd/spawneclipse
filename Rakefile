# largely based on rakefile from osx-window-sizing - thanks!

require 'rubygems'
require 'rake'

desc "Compile SpawnEclipse to .app file"
task :compile do
  puts "Compiling SpawnEclipse.applescript..."
  system "osacompile -o ./bin/SpawnEclipse.app ./lib/SpawnEclipse.applescript"
  puts "Done"
  puts
end
 
desc "Install SpawnEclipse to your applications folder"
task :install => :compile do
  puts "Copying scripts to your scripts folder"
  system "cp ./bin/*.app ~/Applications/"
  puts "Done"
end