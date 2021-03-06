# Phabricator

## Installation

Add this line to your application's Gemfile:

    gem 'phabricator'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install phabricator

## Usage

### Projects

```ruby
# Find the project given a project name.
Phabricator::Project.find_by_name('Project')
```

### Tasks

```ruby
# Create a Maniphest task.
Phabricator::Maniphest::Task.create('title')

# Create a Maniphest task with more detail.
Phabricator::Maniphest::Task.create('title', 'description', ['Project'], 'normal')
```

### Contributing

Patches welcome! (:

For a list of Conduit methods available, see http://secure.phabricator.com/conduit.
