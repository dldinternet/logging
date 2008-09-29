
load 'tasks/setup.rb'

ensure_in_path 'lib'
require 'logging'

task :default => 'test:run'

PROJ.name = 'logging'
PROJ.summary = 'A flexible and extendable logging library for Ruby'
PROJ.authors = 'Tim Pease'
PROJ.email = 'tim.pease@gmail.com'
PROJ.url = 'http://logging.rubyforge.org/'
PROJ.rubyforge.name = 'logging'
PROJ.rdoc.dir = 'doc/rdoc'
#PROJ.rdoc.remote_dir = 'rdoc'
PROJ.rdoc.remote_dir = ''
PROJ.version = Logging::VERSION

PROJ.exclude << %w[^tags$ ^tasks/archive ^coverage]
PROJ.rdoc.exclude << '^data'

PROJ.ann.email[:server] = 'smtp.gmail.com'
PROJ.ann.email[:port] = 587

depend_on 'flexmock'
depend_on 'lockfile'

# EOF
