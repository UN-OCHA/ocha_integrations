![CI](https://github.com/UN-OCHA/ocha_integrations/workflows/CI/badge.svg)

# Common OCHA integrations for Drupal.

## Config to change.

Make sure to change the appname in the following config files

- ocha_disasters.settings.yml
- ocha_themes.settings.yml

HID contacts needs an API key to be usable.

## Modules

All modules use [pcb](https://www.drupal.org/project/pcb) for caching, and cache is updated using cron.

All modules have their own field type, formatter and widget.

### ocha_integrations

Base module for all other integrations.

Also provides extras for Search API and facets

- Encoder for pretty paths to output integer list items
- Show the current search string
- Adds reset search string link
- Adds reset facets link for pretty paths

### ocha_countries

Returns the list of countries from http://vocabulary.unocha.org.

### ocha_disasters

Returns the lisf of disasters from https://www.reliefweb.int including GLIDE number.

### ocha_global_coordination_groups

Returns the list of global coordination groups from http://vocabulary.unocha.org.

### ocha_hid_contacts

Returns contacts from https://humanitarian.id needs an API key.

### ocha_local_groups

Returns the list og local groups (aka bundles) from https://www.humanitarianresponse.info.

### ocha_locations

Returns the list of locations from https://www.humanitarianresponse.info up to admin level 3.

### ocha_organizations

Returns the list of organizations from https://www.humanitarianresponse.info.

### ocha_persons

Defines a person entity so you don't need to create a contact node type.

### ocha_population_type

Returns a list of popultaion types from https://www.humanitarianresponse.info.

### ocha_themes

Returns a list of themes from https://www.reliefweb.int.
