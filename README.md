# Entity Data

This module allows other modules to associate data to entity instances.
It extends the mechanism used from Backdrop core to associate generic data to user accounts, but it uses a different
approach, similar to the one used by the
[`UserData`](https://api.drupal.org/api/drupal/core%21modules%21user%21src%21UserData.php/class/UserData/10)
class starting from Drupal 8.

- The data associated to an entity instance is only loaded on-demand, instead of being all loaded when the entity is
  loaded from the database
- The data is not automatically saved when the entity is saved, but it needs to be explicitly saved
- The data can be filtered by tags associated to each data item, or by module
- The data is automatically deleted when the related entity is deleted

This module exposes an API that other modules can use. Install it only when instructed to do so from a module
instructions.

## Requirements

This module requires Backdrop 1.26.0, or higher versions, and PHP 8.2.

Consult your server administrator or hosting provider if you are unsure about
these requirements.


## Installation

- Install this module using the official Backdrop CMS instructions at
  [Extend with Modules](https://docs.backdropcms.org/documentation/extend-with-modules).

- The module does not have a configuration page. It only exposes an API other modules or themes can use.


## Issues

Bugs and Feature requests should be reported in the
[issue queue](https://github.com/backdrop-contrib/entity_data/issues).


## Current Maintainers

- [kiamlaluno](https://github.com/kiamlaluno)


## License

This project is GPL v2 software.
See the LICENSE.txt file in this directory for complete text.
