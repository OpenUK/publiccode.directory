# Federated database 'entry' meta-files of resources

A main centralised index file links to federated entry files which contain the information of a particular resource. These 'entry' files can then be managed by the software maintainer or a 3rd party, therefore sharing the upkeep of the records.

An entry represents software, policies, resources and case studies.

## Sample entries

Sample entry files are available in this repo. Details of the fields processed in the file are listed below.

### entry.json

a JSON file including all fields required for this entry

### entry.yaml

A YAML file example. This will need to be converted to JSON for use as the directory only processes JSON entries.

TODO: add conversion script / facility / command ?

## Data fields

### Entry

#### entry_type (mandatory)

One of:

- software
- casestudy
- policy
- resource

```bash
"entry_type": ["policy"]
```

#### description (mandatory)

The description element of the entry - plain text

```bash
"description": "Vestibulum lectus mauris ultrices eros in cursus turpis. Lorem ipsum dolor sit amet consectetur adipiscing elit ut. In arcu cursus euismod quis viverra. Augue lacus viverra vitae congue eu consequat ac. Praesent semper feugiat nibh sed pulvinar proin gravida hendrerit. Ipsum dolor sit amet consectetur adipiscing elit pellentesque habitant. Eu volutpat odio facilisis mauris sit."
```

#### repository (mandatory)

The repository where the entry project lives at (for development, maintainance, etc)

```bash
    "repository": "https://project.repository"
```

#### official_url (not mandatory)

The official website that represents the entry being used (software)

```bash
  "official_url": "https://project.website.if.it.has.any"
```

#### logo_url (not mandatory)

URL for the logo of the entry

```bash
  "logo_url": "https://project.logo"
```

#### origin_country (mandatory)

The initial country where the entry has been developed

```bash
 "origin_country": "UK"
```

#### language (mandatory)

Language of the entry. It can be one languge or multiple languages

```bash
 "language": ["EN", "DE"]
```

#### sector (mandatory)

The sector categorisation of the entry.

One or many of:

- localgov
- centralgov
- healthcare
- education
- defence
- etc...

```bash
  "sector": ["localgov", "council"]
```

#### category (mandatory)

The operational category that the project will be used in.

One or many of:

- e-voting
- website
- housing
- ticketing
- etc...

```bash
entry_category: ['housing']
```

#### license (mandatory)

The license of the code refered to in the entry.
One or many of:

- MIT
- GNU-3
- etc...

```bash
  "license": ["MIT", "GNU-3" ]
```

### developers (mandatory)

The initial developers of the project.
Each developer that participated in the development of the project can have their details included thus creating exposure. For each developer we have the following fields that can be filled in

#### developer_name (mandatory)

```bash
    "developer_name": "developer name"
```

#### developer_logo_url (not mandatory)

```bash
    "developer_logo_url": "https://developer.logo"
```

#### developer_url (not mandatory)

```bash
    "developer_url": "https://developer.domain"
```

#### developer_category (not mandatory)

```bash
    "developer_category": "Public"
```

### maintainers

The current maintainers of the project.
Each maintainer that sustains of the project can have their details included thus creating exposure. We have the following fields that can be filled in

#### maintainer_name (mandatory)

```bash
    "maintainer_name": "maintainer name"
```

#### maintainer_url (not mandatory)

```bash
    "maintainer_url": "https://maintainer_url"
```

#### maintainer_logo_url (not mandatory)

```bash
    "maintainer_logo_url": "https://maintainer_logo_url"
```

#### maintainer_repository (not mandatory)

```bash
    "maintainer_repository": "https://git.repository"
```

### users

The current organisations / private implementations of the project.
Each user can have their details included thus creating exposure. We have the following fields that can be filled in

#### user_name (mandatory)

```bash
    "user_name": "user name"
```

#### user_location (not mandatory)

```bash
    "user_location": "London, UK"
```

#### user_logo_url (not mandatory)

```bash
    "user_logo_url": "https://user_logo_url"
```

#### user_url (not mandatory)

```bash
    "user_url": "https://user_url"
```

#### user_geolocation (not mandatory)

User graphical location used for map markers of where the project is currently used. It will be used as a sepparate layer that end-users of the Federated Database can filter projects by

```bash
   "user_geolocation": {
        "lat": 53.371376,
        "long": -1.23398
      }
```
