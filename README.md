# grapho

## GRAPHO - Graph Databases Course - Prof. Gianmaria Silvello

### University of Padova - A.A. 2024-25

---

## Group Members

GRAPHO Group

| Surname   | Name    | ID      |
| --------- | ------- | ------- |
| Antonutti | Manuel  | 0000000 |
| Volpones  | Simone  | 0000000 |
| Zanon     | Tommaso | 2129677 |

---

## Domain of interest:

We chose to focus on the music industry, combining it with the domains of movies and social media. This decision was based on the large amount of public open data related to these areas and we thought it would be interesting to find links between them.

## Objective

The objective of this repository is to propose an ontology that can handle data about music. The proposed system aims to model:

- General information about MusicEntity (single Artist or Group) and its discography
- Information about user-generated Playlist
- Information about Movies in which an Artist has taken part

## Datasets Overview

## Main statistics

4806 different **Music Entity** (either **Group** or **Artist**) with information about :

- Stage Name
- Number of spotify, youtube and twitter followers
- Genre
- Personal Information (Gender, Birthdate and Nationality)
- Movies that they have worked in
- Awards (Grammy and Oscar) nominations and winnings

236613 **Album** with information about:

- Name of the album
- The Release Date
- Number of songs contained (Albums with one song are inferred to be Singles)

1496098 **Song** with information about:

- Name
- Duration
- The fact if they are explicit or not
- Youtube Statistics (Likes and Views)

5067 **Movie** with information about:

- Title (movieName)
- Release Date
- Duration
- Oscar nominated and won

2694 **Playlist** with information about:

- Name
- Followers
- Song added to the playlist

## Ontology Diagram

<img src="ontology/grapho_ontology.jpeg" alt="Ontology Diagram"/>

The image provided above displays the class diagram for reference.
[`Ontology_without_data.ttl`](https://github.com/tommasozanon/grapho/blob/main/ontology/grapho-music-ontology-base.ttl)

## Organization of the Repository

The project is developed using:

- [draw.io](https://drawio-app.com/) for drawing the ontology model.
- [PROTÉGÉ](https://protege.stanford.edu/) for implementing the ontology model.
- [Python RDFlib](https://rdflib.readthedocs.io/en/stable/) for serializing the data.
- [GraphDB](https://www.ontotext.com/products/graphdb/) for querying the data.
