namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hello to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

task :console do
  puts "hola de Rake!"
end

namespace :db do
  task :migrate => :environment do
    puts "hola de Rake!"
  end

  task :environment do
    puts "hola de Rake!"
  end

  task :seed do
    require_relative './db/seeds.rb'
  end
end
