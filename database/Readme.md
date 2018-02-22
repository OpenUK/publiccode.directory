# Description of database
## sector_category
One or many of:
- local
- central
- healthcare
- education
- defence

## maintainer_category
One of:
- public
- ngo
- commercial

## base_url
A required base URL for the public code. For example:
- https://github.com/alphagov/signon

Within this it is required that the meta files exist for inclusion in the directory.

## protocol
For now, just git. However, who knows what will come in future. If not specified, the sensible default is just 'git'

One of:
- git

