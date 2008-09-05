# largely based on rakefile from osx-window-sizing - thanks!

require 'rubygems'
require 'rake'

desc "Compile scripts to .scpt files"
task :compile do
  puts "Compiling SpawnEclipse.applescript..."
  system "osacompile -o ./bin/SpawnEclipse.scpt ./lib/SpawnEclipse.applescript"
  puts "Done"
  puts
end
 
desc "Install scripts to your scripts folder"
task :install => :compile do
  puts "Copying scripts to your scripts folder"
  system "cp ./bin/*.scpt ~/Library/Scripts/"
  puts "Done"
  puts
end