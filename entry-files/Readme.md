# Federated YAML meta-files

The directory index records locations of YAML files that hold the contents of each record.

## Sample file

A sample file 'entry.yaml' is supplied here https://github.com/OpenUK/publiccode.directory/blob/master/entry-files/entry.yaml. This file includes the data fields and example usage.

## publiccode.directory.entry.yaml

A YAML directory entry configurration file to be hosted and maintained by the owner of the project.

The directory contains the following types of entry:

- Software
- Case study
- Policy
- resource

# Data fields:

## Entry

### entry_type

One of:

- software 
- casestudy 
- policy 
- resource

### entry_descripton

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

One or many of:
- 
# the category the project is meant to be implemented - (evoting, website, housing, ticketing etc)

entry_category: 'housing'

### entry_license

The license of the entry

## Maintainer information

### developer_category

One of:
- public
- ngo
- commercial





