# OpenUK publiccode.directory (PCD) project

After seeking contributions to an OpenUK NHS report project, it became apparent that there is lots of Public Administration Open Source being created but no curated list of applications, meaning that lots of local builds are taking place.

This project delivers a single curated directory index of public code and associated resources with federated entry files to enable the teams who manage the code to take ownership of thier own entry.

Think of it as an internet-based federated and distributed database.

# What problem does this solve?

1. 'Discoverability' of Public Code - find out what has been written, who made it and how to get it
2. Repo owners manage the description via their normal code repo
3. A visitor can discover mature software rather than trawling through thousands of repositories

# Who is behind it?

This is an [OpenUK](https://openuk.uk) initiative in association with the EU Free Software Policy group to provide a practical tool to support the PMPC campaign.

# Web interface

A web interface is provided in a [separte repo](https://github.com/OpenUK/publiccode.directory-web-interface) but as the data and code is open, anyone can create their own initerface on top. However, it would make sense to improve the one that is there and also help improve the database.

# Operations

A repo needs to be registered in the database and have meta data within the repo to be included. The index will build the rest on the fly.
The full details of the database can be found in the database folder and here is a summary.

## Sector categories

Repositories of public code belong to a set of categories, therefore each have a separate index. For example, these may indicate:

- Local administration
- Central government / national
- Healthcare
- Education
- Defence

A repo may exist in multiple categories if it happened to originate in one of these yet be relevant to more than one.
A tag is used to indicate the categories that an entry belongs to.

## Maintainer category

Code is created and maintained by various organisations, either public, NGO or commercial.

# Getting involved

There are a few ways you can get involved.

## Technical Git users:

Here is how to get your entry into this project:

- Get the [Entry-JSON file](https://github.com/OpenUK/publiccode.directory/blob/master/entry-files/entry.json)
- Fill in the file in a JSON structure (most fields take strings as values, some take arrays, the example covers all the possible fields)
- Save it in a publically accessible HTTPS location (maybe your code repo would be the best place?)
- Create a PR for the [Database Index file](https://github.com/OpenUK/publiccode.directory/blob/master/database/database.index.json) and add the link to your entry file
- Create an issue and place the link there
- Once your entry has been checked, it will be entered in to the index and you can manage the entry yourself.

The website will automatically pick up all the changes and refresh the lists on each page reload.

## Non-technical git users

Raise a Github issue with your comments or inclusions

## Non-technical users

Get in touch with OpenUK and share your thoughts: https://openuk.uk

# Supporters

Various public organisations have offered support once the indexes are published. These will be listed in the Supporters page.

# Licence

This software is OpenUK copyright 2018. It is released under the GPLv3 licence. For details see the 'LICENSE' file.

