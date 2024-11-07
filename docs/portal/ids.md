---
tags: ['identifiers']
icon: material/identifier
---

# Identifiers

There are many different identifiers that records receive on their journey from entry to publication. This page explains each one, and how it can be used to find a record across systems.

## Catalog Number
| | |
| -- | -- |
| Structure | [A-Z]######|
| Arbitrary | No |
| Persistant | Best effort |
| Purpose | Uniquely identify a record within a collection|

The catalog numbers at Beaty all begin with a capital letter followed by 6 digits. They are meant to be easily remembered by humans, and convey information about the collection that a particular specimen is from. The catalog numbers for published datasets are as follows

| Dataset | Catalog Number Structure |
| ------- | ------------------------ |
| Birds | B###### |
| Mammals | M###### |
| Herpetology | H###### |
| Fish | X###### |
| Entomology | E###### |
| Fungi | F###### |
| Lichen | L###### |
| Bryophytes | B###### |
| Vascular Plants | V###### |
| Algae | A###### |

## Use cases

Catalog numbers can be used to easily find a record through the [catalog number search](searching.md) option on the homepage. They are also used when staff or visiting researchers are using specimens.
## GBIF ID

| | |
| -- | -- |
| Structure | Numeric only |
| Arbitrary | Yes |
| Persistant | Yes |
| Purpose | View objects shared with GBIF easily through the GBIF interface |

This is an identifier assigned by GBIF when a record is shared to GBIF systems. It is numeric and arbitrary. The purpose of this identifier is to identify records within all 3 billion (and counting) GBIF records. Since GBIF itself applies this identifier, there is no risk of institutions publishing conflicting identifiers.

### Use cases

The GBIF identifier can be used to navigate to a record by appending it to the end of the following URL

`https://gbif.org/occurrence/{gbif_id}`

For example, the Steller's Jay is <https://gbif.org/occurrence/1291974418>. The Beaty Biodiversity Museum does not have control over these identifiers, as we do not assign them. However, they are persistent.

## Occurrence ID

| | |
| -- | -- |
| Structure | UUID v4 |
| Arbitrary | Yes |
| Persistant | Yes |
| Purpose | Uniquely identify a record at Beaty out of all records in the world |

The occurrence id is generated when a record is cataloged at the Beaty Museum. We use the [UUID 4 Standard](https://www.rfc-editor.org/rfc/rfc9562.html#name-uuid-version-4). 

For example, the occurrence id of the Steller's Jay is `4c906ce8-a2bf-425f-8d50-82197e918028`. 

### Use cases

The occurrence id can be used to easily find an object through [general search](searching.md) since it will be unique not only in the Beaty Museum but everywhere. It can also be used to search for records in various other system (such as GBIF or Symbiota) if a general search option is available in those systems.

!!! tip

    When citing a particular specimen, this is the best identifier to use.

