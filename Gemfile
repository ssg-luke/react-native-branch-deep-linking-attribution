source "https://rubygems.org"

gem "cocoapods", [">= 1.7.1", "< 2.0.0"]
gem "fastlane", "~> 2.69"
gem "travis"

plugins_path = File.join(File.dirname(__FILE__), 'fastlane', 'Pluginfile')
eval_gemfile(plugins_path) if File.exist?(plugins_path)
