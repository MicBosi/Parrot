# Hermes

An updated *Robin's Nest*

![An updated Robin's Nest](img/preview.png "An updated Robin's Nest")

Just for fun I've refactored Robin Nixon's book *Learning PHP, MySQL, & JavaScript* [mini social network final example](http://lpmj.net/) based on current PHP standards:

- PSR-1 and PSR-2 code
- Fixed invalid html strings from '' to ""
- Use jQuery
- PHP and HTML now mostly separated
- Database login/password stored in env variables not in source code
- All pages are viewed through single entry point: index.php
- Removed repeated html header and footer -> consolidated into header.php and footer.php
- Isolated top-level code into init.php:
  *Files SHOULD either declare symbols (classes, functions, constants, etc.) or cause side-effects (e.g. generate output, change .ini settings, etc.) but SHOULD NOT do both.*
- Consolidated all configuration in config.php
- Separated content pages (in *pages* dir) from logic pages
- .js and .css in their own directories
- removed ending ?> when not necessary

## Leftovers
- More ``echo <<< _END`` cleanup to do
- More invalid html strings from '' to "" cleanup to do
- More php/html separation to do

## Exercises For The Future
- Streamlined usage flow:
	- go to login page after log out
	- go to profile page after log in
	- log in after sign up
- Use Laravel for db connection, session management and REST API impl
- Make it into a single page app driven by REST API
- Flux/React front end
