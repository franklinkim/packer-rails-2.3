require 'colorize'

task :default do
  system "rake -T"
end

desc "Validate template.json"
task :validate do |t|
  puts "Validating template...".light_yellow
  system "packer validate template.json"
end

desc "Build from template.json"
task :build do |t|
  puts "Building box...".light_yellow
  system "packer build template.json"
end

desc "Add a built box to vagrant"
task :add, [:name, :path]  do |t, args|
  puts "Adding box #{args.name} from #{args.path}".light_yellow
  system "vagrant box add --name #{args.name} #{args.path}"
end
