require 'bundler'
Bundler::GemHelper.install_tasks
Bundler.setup

require 'spree/testing_support/common_rake'

desc "Default Task"
task default: [:spec]

desc "Generates a dummy app for testing"
task :test_app do
  ENV['LIB_NAME'] = 'spree_related_products'
  Rake::Task['common:test_app'].invoke
end
