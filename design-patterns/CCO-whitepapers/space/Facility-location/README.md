# Pattern Name
Facility Location

# Intent

To represent location relationships where material entities (e.g., facilities, equipment, infrastructure) are situated within progressively larger geographic regions or sites (e.g., building → campus → city → state → country), enabling multi-level location queries and reasoning. The specific entity types and site hierarchies shown are examples—this pattern generalizes to any material entity that can be located at sites, and any hierarchical organization of sites.

# Competency Questions

Where is a specific facility located?

what bigger site is this facility located in, and are there smaller sites that the facility is located in that are also located in the bigger site?

what are all the facilities located within a particular site?


# Structure

Represents the location of a site and there approriate relations with a broader area.

Helps with creating transitive realtions between sites. 

Visual model through mermaid and png


Additional Notes:

Geospatial Coordinate Pattern

```mermaid
flowchart BT
    A@{ label: "<font color=\"#000000\">Facility 1</font>" } -- LocatedIn<br>BFO:0000171 --> B@{ label: "<font color=\"#000000\">City 1</font>" }
    B -- LocatedIn<br>BFO:0000171 --> C@{ label: "<font color=\"#000000\">State 1</font>" }
    A -- rdf:type --> D@{ label: "<span style=\"color:black\"><b>Facility<br>ont00000192</b></span><br>" }
    B -- rdf:type --> E@{ label: "<span style=\"color:black\"><b>Site<br>BFO_0000029</b></span><br>" }
    C -- rdf:type --> E
    A -. rdfs:label .-> F["Building 1"]
    B -. rdfs:label .-> G["NY City"]
    C -. rdfs:label .-> H["NY State"]

    subgraph Legend[" "]
    direction LR
    AA{Individual}
    BB[Class]
    CC[data]
    AA --> |relation| CC
    end

    A ~~~ Legend

    A@{ shape: diam}
    B@{ shape: diam}
    C@{ shape: diam}
    D@{ shape: rect}
    E@{ shape: rect}
    F@{ shape: rect}
    G@{ shape: rect}
    H@{ shape: rect}
    A:::purple
    B:::purple
    C:::purple
    D:::yellow
    E:::yellow
    F:::white
    G:::white
    H:::white
    classDef yellow fill:#ffe680
    classDef purple fill:#dbc9ef
    classDef white fill:#FFFFFF
    class BB yellow
    class AA purple
    class CC white

```
