require 'yaml'
require 'base64'
require 'erb'

COMPOSE_PATH = 'compose/'.freeze
CONFIG_PATH = 'config/app.yaml'.freeze

@config = YAML.load_file(CONFIG_PATH)

# Add your own tasks in files placed in lib/tasks ending in .rake
Dir.glob('lib/tasks/*.rake').each do |task|
  load task
end
