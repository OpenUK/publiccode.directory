# Federated database 'entry' meta-files of resources

A main centralised index file links to federated entry files which contain the information of a particular resource. These 'entry' files can then be managed by the software maintainer or a 3rd party, therefore sharing the upkeep of the records.

An entry represents software, policies, resources and case studies.

# Sample entries

Sample entry files are available in this repo. Details of the fields processed in the file are listed below.

## entry.json

a JSON file including all fields required for this entry

## entry.yaml

A YAML file example. This will need to be converted to JSON for use as the directory only processes JSON entries.

TODO: add conversion script / facility / command

# Data fields:

## Entry

### entry_type

One of:

- software 
- casestudy 
- policy 
- resource

### entry_description

The description element of the entry - plain text

### entry_logoURL

URL for the logo of the entry

### entry_lang

Language of the entry

(EN default)

### entry_sector

The sector categorisation of the entry.

One or many of:
- localgov
- centralgov
- healthcare
- education
- defence

### entry_category

The operational category that the project will be used in.

One or many of:
- e-voting
- website
- housing
- ticketing

entry_category: 'housing'

### entry_license

The license of the code refered to in the entry.

### developer_category

One of:
- public
- ngo
- commercial

### developer_contact

Details of the original develoer

Mandatory
- Organisation_name

Optional
- tel
- email
- website
- address

### maintainers

A list of maintainers for the resource
TODO: Array
