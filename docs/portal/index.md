---
tags:
  - GBIF
---

# Overview

<div class="grid cards" markdown>
- <https://collections.beatymuseum.ubc.ca>
</div>

The data portal allows anyone, anywhere in the world to access information about specimens at the Beaty Biodiversity Museum. Data can be searched on a per dataset basis, or across the whole museum.

<figure markdown>
  ![Image](../assets/screenshots/GBIF_Overview_Image1.png)
  <figcaption>Homepage of the BBM GBIF Data Portal</figcaption>
</figure>

## Data Source

All data is automatically synced between GBIF and the website through GBIF's API. This means that if the data has been published to GBIF it will be accessible through the portal. Data is published at different frequencies for each collection, depending on the size and frequency of updates.

### Images

Images are not hosted by GBIF, rather they are served by a CDN. You may access any image directly from your browser if you know the `catalogNumber` of a specimen. For example, to access the image of the Steller's Jay (B000003), you may use <https://beaty.b-cdn.net/B000003.jpg>. All files are in `jpg` format and will therefore end in `.jpg`. If there are multiple images for the same specimen, the first time will contain no suffix, and the rest will end in `a`, `b`, `c` etc.

!!! example

    Pick a catalog number and try it out! The link will always follow the form `https://beaty.b-cdn.net/` + `catalogNumber` + `.jpg`. The presence of leading zeros in catalogNumbers varies by dataset, but we are actively working to standardize this.

## Identifiers for Collections and Datasets

The Beaty Biodiversity Museum consists of 6 collections (4 with data currently published) and 10 datasets. The identifiers and codes for each are listed below. Datasets exist as a _subset_ of collections. There can be many datasets under one collection. The tree for those collections with data is outlined below:

```mermaid
graph TD
    A[Beaty Biodiversity Museum] ---> CTC[Cowan Tetrapod Collection];
    A[Beaty Biodiversity Museum] ---> SEC[Spencer Entomological Collection];
    A[Beaty Biodiversity Museum] ---> UBC[UBC Herbarium]
    A[Beaty Biodiversity Museum] ---> ICH[Fish Collection]
    CTC[Cowan Tetrapod Collection] ---> B(Birds);
    CTC[Cowan Tetrapod Collection] ---> M(Mammals);
    CTC[Cowan Tetrapod Collection] ---> D(Herpetology);
    SEC[Spencer Entomological Collection] ---> E(Entomology);
    UBC[UBC Herbarium] ---> V(Vascular Plants);
    UBC[UBC Herbarium] ---> Al(Algae);
    UBC[UBC Herbarium] ---> Br(Bryophytes);
    UBC[UBC Herbarium] ---> F(Fungi);
    UBC[UBC Herbarium] ---> L(Lichen);
    ICH[Fish Collection] ---> Fi(Fish);
```

### Collections

Any particular collection can be accessed through `https://collections.beatymuseum.ubc.ca/collection/{identifier}`

| Collection Name | Code | Identifier |
| --------------- | ---- | ---------- |
| Cowan Tetrapod Collection | CTC | `3b2ad644-b3e4-4ac9-a57f-23be3f86ed0e` |
| Beaty Biodiversity Fish Collection | ICH | `5aee131f-91dd-4b78-bfee-296f86801b7f` |
| Beaty Biodiversity Fossil Collection | PAL | `1fcf0cb0-aa26-40d0-8311-fb4b6f2050f7` |
| Beaty Biodiversity Museum Marine Invertebrate Collection | MIC | `403e3c1f-086f-461b-9718-60537ee4ce3c` |
| Spencer Entomological Collection | SEC | `8f5f5b6f-28c6-44b4-8f21-98c55eaae203` |
| UBC Herbarium | UBC | `b44fcb7f-1227-4fa3-8ed2-de27aabb06e0` |

### Datasets

Any particular dataset can be accessed through `https://collections.beatymuseum.ubc.ca/dataset/{identifier}`

| Dataset Name | Identifier |
| ------------ | ---------- |
| Birds | ba0c046d-52bb-4262-a495-652988c9f3f7 |
| Mammals | 3ad882bb-cd21-4201-8b83-3684bfc6d830 |
| Herpetology | df9c8b86-9d36-4e29-91b3-4274dff053e5 |
| Entomology | 9c45867f-f77d-42f3-9751-ae16bb7c9bc8 |
| Fish | 4caf2040-83ad-4fa7-ba13-005bced721eb |
| Fungi | ca1bcd7e-7387-42f9-81ba-1470db55e3e8 |
| Lichen | 628abbe5-dc8d-41e9-a0c7-f05efe282649 |
| Bryophytes | 4edd9396-59df-4b01-9e29-dc21a59f9963 |
| Algae | 90302970-1bc6-4865-be76-9aef1dd707f9 |
| Vascular Plants | 07fd0d79-4883-435f-bba1-58fef110cd13 |


*[API]: Application Programming Interface
*[CDN]: Content Delivery Network