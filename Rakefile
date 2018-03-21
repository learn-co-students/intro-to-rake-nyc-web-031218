desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

task :"greeting:hello" do
  puts "hello from Rake!"
end

task :"greeting:hola" do
  puts "hola de Rake!"
end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seed the database with some dummy data'
    task :seed do
  require_relative './db/seeds.rb'
end
end

task :environment do
  require_relative './config/environment'
end
