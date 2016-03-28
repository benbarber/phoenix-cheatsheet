# Phoenix Cheatsheet
A cheatsheet for the [Elixir](http://elixir-lang.org/) based [Phoenix framework](http://www.phoenixframework.org) because sometimes going through lots of documentation can be a little painful.

### Creating a new project
`$ mix phoenix.new [name] [args]`

The following arguments are available to pass when setting up your project:

`--no-brunch` Don’t install brunch, useful if you are building an API or don’t require any front end.

### Adding Hex packages and managing your applications dependencies
`$ mix deps.get` Installs any required hex packages

`$ mix deps.update --all` Updates the installed versions of any hex packages

### Generators
`$ mix phoenix.gen.html Post posts title:string body:text` Generates a resource

`$ mix phoenix.gen.json Post posts title:string body:text` Generates a JSON resource, useful if you are developing an API

`$ mix phoenix.gen.channel Room rooms` Generates a channel

`$ mix phoenix.gen.model Post posts title:string body:text` Generates a model and an associated migration

`$ mix ecto.gen.migration add_posts_table` Generates a migration file

### Running migrations
`$ mix ecto.create` Creates the required databases ready for any migrations to be run

`$ mix ecto.migrate` Run your applications migrations
