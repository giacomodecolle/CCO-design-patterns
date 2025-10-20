```mermaid

flowchart TD
  %% === ATTACK SUBGRAPH ===
  subgraph Attack
    direction TB
    %% Classes
    OffensiveAction[Offensive Action]
    Attacker[Agent]
    OffensiveTechnique[Offensive Technique]
    OffensiveTactic[Offensive Tactic]
    DigitalArtifact[Digital Artifact]

    %% Instances
    OffensiveAction1{OffensiveAction1}
    Attacker1{Attacker1}
    OffensiveTechnique1{OffensiveTechnique1}
    OffensiveTactic1{OffensiveTactic1}
    DigitalArtifact1{DigitalArtifact1}
    DigitalEvent1{DigitalEvent1}

    %% Type assertions
    OffensiveAction1 -->|rdf type| OffensiveAction
    Attacker1 -->|rdf type| Attacker
    OffensiveTechnique1 -->|rdf type| OffensiveTechnique
    OffensiveTactic1 -->|rdf type| OffensiveTactic
    DigitalArtifact1 -->|rdf type| DigitalArtifact
    DigitalEvent1 -->|rdf type| DigitalEvent

    %% Relations between instances (attack)
    OffensiveAction1 -->|has agent| Attacker1
    OffensiveAction1 -->|implements| OffensiveTechnique1
    OffensiveTechnique1 -->|enables| OffensiveTactic1
    Attacker1 -->|uses| OffensiveTactic1
    OffensiveAction1 -->|has participant| DigitalArtifact1
  end

  %% === DEFENSE SUBGRAPH ===
  subgraph Defense
    direction TB
    %% Classes
    DefensiveTechnique[Defensive Technique]
    DefensiveAction[Defensive Action]
    DefensiveTactic[Defensive Tactic]

    %% Instances
    DefensiveTechnique1{DefensiveTechnique1}
    DefensiveAction1{DefensiveAction1}
    DefensiveTactic1{DefensiveTactic1}


    %% Type assertions
    DefensiveTechnique1 -->|rdf type| DefensiveTechnique
    DefensiveAction1 -->|rdf type| DefensiveAction
    DefensiveTactic1 -->|rdf type| DefensiveTactic

    %% Relations between instances (defense)
    DefensiveAction1 -->|has participant| DigitalArtifact1
    DefensiveAction1 -->|implements| DefensiveTechnique1
    DefensiveTechnique1 -->|enables| DefensiveTactic1
  end
  OffensiveAction1 -->|causes| DigitalEvent1
  DigitalEvent1 -->|produces| DigitalArtifact1


  %% === CCO SUPERCLASSES ===
  subgraph CCO
    direction TB
    CCOProcess[BFO:Process BFO_0000015]
    CCOPlan[cco:Plan ont00000974]
  end

  %% Subclass relations (D3FEND classes -> CCO classes)
  OffensiveAction -->|rdfs:subClassOf| CCOProcess
  DefensiveAction -->|rdfs:subClassOf| CCOProcess

  OffensiveTechnique -->|rdfs:subClassOf| CCOPlan
  OffensiveTactic -->|rdfs:subClassOf| CCOPlan
  DefensiveTechnique -->|rdfs:subClassOf| CCOPlan
  DefensiveTactic -->|rdfs:subClassOf| CCOPlan
  DigitalEvent -->|rdfs:subClassOf| CCOProcess

  %% === LEGEND ===
  subgraph Legend
    AA{Individual}
    BB[Class]
    CC[data]
    EE[CCO superclass]
    BB --> |relation| CC
    DD[This is a high-level pattern of D3FEND which represents how attacking and defensive techniques are implemented to attack and defend digital artifacts]
  end

  %% === STYLING ===
  classDef yellow fill:#ffe680,stroke:#333,stroke-width:1px;
  classDef purple fill:#dbc9ef,stroke:#333,stroke-width:1px;
  classDef white fill:#ffffff,stroke:#333,stroke-width:1px;
  classDef grey fill:#d9d9d9,stroke:#333,stroke-width:1px;

  %% Assign colors
  class OffensiveAction,Attacker,OffensiveTechnique,OffensiveTactic,DigitalArtifact,DefensiveTechnique,DefensiveAction,DefensiveTactic,DigitalEvent yellow
  class OffensiveAction1,Attacker1,OffensiveTechnique1,OffensiveTactic1,DigitalArtifact1,DefensiveTechnique1,DefensiveAction1,DefensiveTactic1,DigitalEvent1 purple
  class Label1 white
  class CCOProcess,CCOPlan grey

  %% Legend colors
  class AA purple
  class BB yellow
  class CC white
  class EE grey
