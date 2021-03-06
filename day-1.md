Lightning Talks
==============

Spotlight
--------------

1. Configurable Blacklight
  - Uses an admin interface.
  - Quite pretty.
2. Ingest items from outside.
3. Image cropping capability.
  - Lets you crop out a specific part of an image and then use it in the
    exhibit.
4. Contact
  - http://github.com/sul-dlss/spotlight
  - exhibits-team@lists.stanford.edu
  - Jessie Keck - @jessiekeck

Mirador
--------------

1. IIIF viewer.
2. Zoom/Pan using OpenSeaDragon.
3. Used in windowed environment.
4. Can display objects cross-repositories. 
5. Structural navigation using IIIF presentation API.
6. Annotations using OpenAnnotate/IIIF Presentation API.
7. Can readjust layout - open two items side-by-side for instance.
8. Saves mirador configuration between refreshes.
9. Bookmark current state and send it to someone else.

Sipity - Jeremy Friesen
------------------------

1. TODO oriented self deposit.
2. Great mediated deposit processes.
3. Later discussions on how this is configurable.
4. Opinion is walk people up to deposit in Fedora, THEN deposit.

Arclight
---------

1. Extend core features of blacklight to enable discovery of archival content.
2. Intended to provide for discovery of both physical and digital objects.
  - Digital Objects
    - Enable discovery
3. Not replacement for ArchivesSpace.
4. It's a discovery environment, NOT a finding aid editing environment.
5. Developed/maintained by Blacklight community.
6. Initiated at Stanford because they need it.
7. Want to involve interested institutions in process of development as early as
   possible.
8. Wiki pages on Duraspace of plans.
9. arclight-design@lists.stanford.edu - For collaborating on design.
10. Design collaborators can use Box + Google Drive.
11. Design Process
  - Discovery
  - Information Architecture
  - Interaction & Visual Design
12. Current Status
  - Put out a call for collaborators - a dozen institutions said they had some
    interest in collaboration.
  - Worked on phase 1 of discovery process.
  - Received goals/objectives from 8 institutions.
  - Finished first phase of discovery.
  - Beginning interviews with archivists. They've started, done two interviews
    last week.
  - Some other institutions are interested in doing interviews as well.
13. Wiki: https://wiki.duraspace.org/display/hydra/ArcLight

Session Pitches
================

Geoblacklight
--------------

Session to talk about geoblacklight
1. Deployment
2. Talk to anyone who's interested in contributing/deploying.

Linked Data Platform
----------------------

W3C spec, recently accepted - 2 weeks ago. There's a lot to learn, and it powers
Fedora 4 right now.

1. Would include what's a resource vs what's a container.

IIIF - What's coming up
------------------------
Three bits of work
1. Authentication
  - Reasonably well understood
2. Search within an object
3. Discovery of an object.

Get feedback on how people want to do authorization/make them
discoverable/search within an object depicted by images.

Portland Common Data Model
---------------------------

Next steps, what do we need to do to implement this? How does this fit with our
use cases.

2 sessions - what is this? And WORK.

ArcLight
-----------

Understanding all of the different initiatives for archival development over the
next 18 months. What's going to happen with ArcLight and what's going to follow
ArcLight?

Spotlight
------------

A lot of people interested in spotlight have been waiting and watching. The team
feels like they're ready.

1. Do a deeper dive into the features and what they've accomplished. Go through
   installation process.
2. Improve documentation to encourage adoptability.
3. How do we implement this with our local repository?
4. Future work-plans with how spotlight relates with things like IIIF.

Sipity
-------------

1. How it was architected
2. Plans
3. Different patterns used in Sipity to make it more extensible.
4. Reporting out on what the plans are.

Maybe we need a "rails patterns" session

JSON-LD
-------------

1. Discussion about contexts.
2. How JSON-LD can make RDF, especially from Fedora 4, available to actual use
   rather than "academic handwaving."

Newspapers
------------

1. What can we do to better use newspaper collections with IIIF?

Hydra/Fedora/LDP Resolution of Big Thread
------------------------------------------

There's been an ongoing, morphing, changing slippery discussion of the
intersection of Fedora as a product and LDP as a spec. How much does Fedora
embrace LDP and how much does it keep it at arms length?

Can we agree on what we want that relationship to be?

Ben Armintor will be doing this virtually.

Owning the Application
----------------------

Trying to get in front of the decay that happens with an application. How do you
stay in front of ownership of the application code.

Are we doing a good job making sure our stuff doesn't fall apart?

Video Encoding Services
------------------------

1. Avalon does lots of video encoding.
2. Want to change their infrastructure to allow multiple backends.
3. Wants to hear experiences and make a space for talking about it.
4. Look at some kind of common API to access video encoding services.

Fedora 3 Users Anonymous
-------------------------

1. Northwestern has stated they don't see switching over to F4 for a while out.
2. Find out where people are at in the transition.
3. How do they continue to support Hydra on Fedora 3?

Blacklight Abstraction
-----------------------

1. Been efforts in Blacklight to get it to be more abstract.
2. Blacklight is very coupled to Solr. There's desire for it to work on
   ElasticSearch.
3. DPLA/Europeana are interested in getting Blacklight to work natively with
   their APIs.
4. There's a rough timeline for the work.
5. Wants to coordinate more of the work.

Federal Data Mandates - What should we do?
------------------------------------------

1. Is there anything we can do as a reference implementation or baked in APIs
   that come pre-approved?
2. What is our responsibility?
3. If people want a run-through of NSF report they can share it.


Sign Posting Text & Data Mining Efforts
----------------------------------------

Want to describe content for things like data mining. We haven't done much as
common standards/APIs/infrastructure in this space.

Is there anything we can do across platforms/repositories to facilitate these
kinds of uses.

Media with Synchronized Transcripts
------------------------------------

1. Any backend principles?
2. Coding?
3. UIs they've used.
4. If anybody's had any experience in getting synchronized transcripts to work?
5. Having an open-standard in IIIF for time relations.

DAM Needs for Museums
-----------------------------

1. Specific needs of object-based museums for DAM.
2. How does it relate to Fedora?

Mirador
--------

1. Discussion for future plans.
2. What is the next great book viewer going to be?

Tagging/Virtual Collections in Blacklight
------------------------------------------

1. Using LDP/Fedora 4
2. Different implementation that has a lot of points of interoperability.
3. Cornell uses tags.

Controlled Vocabularies
------------------------

How do we do them.

SESSIONS
============

LDP Introduction
-----------------

1. W3C Technical Recommendation
2. Same status as HTML/CSS/SVG/etc.
3. Layer that sits on top of REST best practices, but focused on link data.
4. Main goal is to have a REST API that follows best practices and works for
   linked data.
4. Fundamentals:
  - Resources ( R in Rest)
    - POST to create
    - PUT to update
    - DELETE
    - PATCH (only the changes on resource)
    - PUT (Replace the entire resource)
    - Two types
      - LDP-RS
        - RDF Resources.
        - RDF in some serialization.
        - Should be able to give back at least TTL or JSON-LD
      - LDP-NRS
        - LDP Non-Rdf
        - This is "anything"
        - Server MAY create an LDP-RS when this is created.
          - It creates a LINK header (describedBy) which points from LDP-NR to
            LDP-RS
  - Containers
    - The question LDP tries to answer is what are the semantics of WHERE you do
      these operations.
    - Three types
      - BasicContainer
        - /images/
        - If you request this it returns a list of its properties AND its
          contents.
        - There's a prefer header for "I only want properties" or "I only want
          contents"
      - DirectContainer
        - Has a way to say "when you post a resource to me, you should also
          manage another triple."
        - Ex When I post a resource to /annotations/anno1/bodies/ it creates a 
          triple <anno1: <hasBody> <x>
        - Done via a property on the container that says membershipResource
          /Anno1/ and memberRelation hasBody
        - Can only have one membership relation.
        - When you create the container you have to say what kind of container
          it is.
      - IndirectContainer
        - Indirect containers let you automatically set a triple on another
          resource to be <subject> <predicateDefinedInContainer> <objectFoundAsObjectInAnotherPredicateInResourceYouCreated>
  - LD Paging
    - Not in official spec - consensus was not reached.
    - Will be published as a working group note.
    - "I want to get N links back and page through"
    - Server has control over where it breaks things up
    - Client has PREFERENCES over how many items to return, but it's up to the
      server.

SPOTLIGHT
---------------

1. One of the big promises of spotlight was to build a self-service platform for
   curators. NO developer access.
2. Wants to be able to do this with content not in the repository.
  - Let them upload items.
3. Improve the look/feel/experience.
4. Where we are
  - What does it mean to install Spotlight?
5. Request an Exhibit
  - Form to fill out that provides a vanilla exhibit.
6. Features
  - Theme pages.
  - Customizable text.
  - Widgets
  - iFrame Widget
    - Recently did a 3D scan of their space.
  - Browse Categories
    - Saved searches provided with context

Installation
===
1. Home page where you can edit front page text while logged in.
2. Permissions to display/edit certain things in the admin dashboard.
3. There's a base behavior with basic roles that you can change if you'd like.
  - Application concern.
4. Edit title/subtitle/description.
5. Contact emails.
6. Published - can hide the entire site.
7. Import/Export. Can export JSON to get all the content to save it.
8. Delete Exhibit
  - If you don't have any exhibits it creates a blank barebones exhibit for you.
9. Administer appearance
  - Searchable
    - Disable search for visitors.
    - Disables facets
  - Create site masthead
    - Add an image for the top banner and scale it to give it more "pop"
  - Site Thumbnail
    - If someone tweets out the exhibit, the thumbnail goes in the twitter card.
  - Configure tabs
    - Change labels/reorder
10. Tag documents and create searches from them.
11. Configure sort dropdown.
12. Modify which metadata fields show up where.
  - Add fields that are only for items in your exhibit
13. Admin interfaces for about/feature pages
14. Create feature pages
15. Can do searches and save it with an alias.
  - You can then use these to browse.
  - Browse categories let you change the look and feel of the site.
  - Clicking an item within a browse category keeps the URL in there and changes
    prev/next appropriately.
16. Add repository item
  - You implement so that it indexes things from your repository.
17. Add non-repository item
  - Lets you ingest items from outside of your repository.
  - There's an edit mode
18. ONE spotlight instance PER exhibit
