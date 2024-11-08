---
title: 'GBIF API'
icon: 'material/api'
---

# GBIF API

When doing analysis for a research study or project, it can be helpful to fetch data directly through code. As all data on the data portal is sourced from GBIF, this means that the GBIF API is the best way to access data from the Beaty Biodiversity Museum programmatically. You do not need an API key to access the data.

!!! example

    Let's say that you wanted to retrieve all Vulpes vulpes records within the at the BBM. You could use the following endpoint:

    ```
    https://api.gbif.org/v1/occurrence/search?institutionKey=c7d5c4da-9590-49c2-b87c-f0e7932611a6&q="Vulpes vulpes"
    ```

## Key Reference

When accessing specimen data, there are a couple of key parameters that you will need to know, depending on the scope you wish to search under. All of the keys relevant to the museum can be found on the [key reference page](../../reference/key-reference.md)
