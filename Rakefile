namespace :greeting do
  desc 'outputs hello to the terminal'
    task :hello do
      puts "hello from Rake!"
    end
  
    desc 'outputs hola to the terminal'
    task :hola do
      puts "hola de Rake!"
    end

#     desc "outputs hey to the trminal"
#     task :hey do
#       puts "Hey!!!"
#     end
  end

#   # this is the heading
#   namespace :goodbye do 
#     desc "outputs bye"
#     task :bye do
#       puts "bye see you soon"
#     end
#   end



namespace :db do
  desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end

    desc "require files from environment"
    task :environment do
      require_relative './config/environment'
    end

    desc 'seed the database with some dummy data'
    task seed: :environment do
      require_relative './db/seeds'
    end
end
  

desc 'drop into the Pry console'
task console: :environment do
  Pry.start
end

desc "require files from environment"
    task :environment do
      require_relative './config/environment'
    end