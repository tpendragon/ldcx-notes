Day 2
=======

New Session Proposal
--------------------

### Geocombine

an open source toolkit for geospatial metadata work.

### Spotlight

Goal to try and make Spotlight feed in a IIIF manifest to ingest an item.

Lightning Talks
-----------------

### Put GIS Data in Repository

Did some demos to go from CD-Rom with data on it to a map interface using
CartoDB.

### Triannon

1. Currently a searchworks branch.
2. Can add a tag to a file.
  - A staff member can add things like "about science." 
3. Tags are stored separately from metadata in Triannon (Fedora) store. If metadata
   changes, tags are still there.
4. You can search by tags.
5. Interoperate tags between institutions

### Linked Data for Libraries & VIVO: Researcher Profiling

1. December 13, got a grant
2. Assembling an ontology and linked data sources to provide relationships,
   metadata, and broad context for scholarly information resources.
3. Create a standard to exchange resources.
4. Go beyond bibliographic data.
5. Connect with faculty profiling information
6. Why Linked Data
  - Flexible/extensible
  - Growing ecosystem
  - Wide range of tools/ontologies
  - Linked data cloud image.
7. Convert from "Strings to Things"
  - Go to URIs
8. Get concrete - stories as the basis of use cases.
  - 42 raw use cases.
  - 12 refined use cases in 6 clusters.
    - Bib + Curation Data
    - Bib + person data
    - Leverage external data including authorities
    - Leveraging the deeper graph
    - Leverage usage data
    - Three-site services e.g Cross-site search
9. LD4L data sources
10. How do we connect to LOD web?
  - Map bibliographic data to BIBFRAME
  - Use ontologies commonly found in linked data.
  - Connect research profile info
  - Create persistent, stable local URI IDs
  - Link local IDs to global IDs (ORCID/VIAF/ISNI)
11. VIVO
  - Open search semantic-web based researcher and research discovery tool.
  - Standard ontology that interconnects researchers, communities, and campuses
    using Linked Open Data
  - Broad community
  - Connects scientists and scholars through their research and scholarship
  - Semantic web application
    - Provides RDF/HTML
    - Self-describing data
    - Provides search & query augmented by relationships
    - Underlying Vitro code supports generic edit/display of ontology and
      instances

### What is LibraryCloud

1. Service that provides granular, open access to a large and growing
   aggregation of Harvard library metadata through APIs - a metadata hub.
2. http//library.harvard.edu/librarycloud
3. https://github.com/harvard-library
4. Harvard's Instance
  - Contains records from ILS (12.7M bib records), VIA (4M images), OASIS (2M
    finding aid components)
  - Amazon Queues does Ingest -> Normalize (MADS) -> Enhance -> Distribute APIs
    (OAI/PM/Download/etc)
5. Authentication/Authorization
6. Collection API.
7. Technology Stack
  - Uses Amazon - spins up 10 instances for ingest.
  - Scripted - deploying LibraryCloud builds up all these servers.

### Implementing Ontologies as a Ruby Gem

1. Implementing ORE
  - ORE can do sets or ordered lists.
  - In simplest form it's just aggregating a bunch of resources
  - ORE:Aggregation
2. Gem provides business logic end of how all the predicates go together.

### Blacklight Folders

1. Indiana had a lot of users using the bookmarks functionality.
2. There's a dropdown to add to folder when selecting items
3. Can look at folders
4. Creating Folders
  - Name them
  - Can set visibility to "anyone" or "only me"
5. If you share it publically you can pass it on to others.
6. Only the owner has edit rights
7. You can rearrange the order of the items in the folder
8. Cite/Email/Export to Endnote/Refworks
9. If you have bookmarks already there's a rake task to move everything over.

### Mirador Annotations

1. Students go through and mark chapters as doing transcription work.
2. Taking all the annotations, putting them into solr, and providing facet
   search through Blacklight.
3. Blacklight can view the IIIF image, IIIF metadata, and display them in a
   basic blacklight view which can link back to Mirador.
