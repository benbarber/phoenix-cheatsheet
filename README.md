# Phoenix Cheatsheet
A cheatsheet for the Elixir based Phoenix framework because sometimes going through lots of documentation can be a little painfull when you are looking for somthing specific, this is the case especially when you are just starting out learning a new technology stack.

### Creating a new project
`$ mix phoenix.new [name] [args]`

The following arguments are available to pass when setting up your project:

`--no-brunch` - dont install brunch, usefull if you are building an API or dont require any front end.

### Adding Hex packages and managing your dependencies
`$ mix deps.get` - Installs any required hex packages

`$ mix deps.update` - Update the installed versions of any hex packages

### Generators
`$ mix phoenix.gen.resource Post posts title:string body:text` - Generates a resource
