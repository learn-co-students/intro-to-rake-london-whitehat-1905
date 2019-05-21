desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

desc 'contains the environment files (ie database connections ect)'
task :environment do
  require_relative './config/environment.rb'
end

desc 'brings up the console through pry'
task :console => :environment do
  #requires the environemtn else pry would have no database to let you access
  Pry.start
end

namespace :db do
  desc 'seeds the database'
  task :seed do
    require_relative "./db/seeds.rb"
  end

  desc 'creates the student table'
  task :migrate => :environment do
    Student.create_table
  end

end

namespace :greeting do
  task :hello do
    puts "hello from Rake!"
  end

  task :hola do
    puts "hola de Rake!"
  end
end