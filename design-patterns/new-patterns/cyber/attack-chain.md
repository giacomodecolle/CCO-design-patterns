```mermaid

flowchart LR
  %% === CLASSES (TBox) ===
  OffensiveAction[Offensive Action]
  Attacker[Attacker]
  OffensiveTechnique[Offensive Technique]
  DigitalArtifact[Digital Artifact]

  %% === INSTANCES (ABox) ===
  subgraph AttackInstances
    direction LR
    OffensiveAction1{OffensiveAction1}
    Attacker1{Attacker1}
    OffensiveTechnique1{OffensiveTechnique1}
    OffensiveTactic1{OffensiveTactic1}
    OffensiveTactic2{OffensiveTactic2}
    OffensiveTactic3{OffensiveTactic3}
    OffensiveTactic4{OffensiveTactic4}
    OffensiveTactic5{OffensiveTactic5}
    OffensiveTactic6{OffensiveTactic6}
    OffensiveTactic7{OffensiveTactic7}
    OffensiveTactic8{OffensiveTactic8}
    OffensiveTactic9{OffensiveTactic9}
    OffensiveTactic10{OffensiveTactic10}
    OffensiveTactic11{OffensiveTactic11}
    OffensiveTactic12{OffensiveTactic12}
    OffensiveTactic13{OffensiveTactic13}
    OffensiveTactic14{OffensiveTactic14}
    DigitalArtifact1{DigitalArtifact1}

    %% Labels as yellow boxes
    Reconnaissance[[Reconnaissance]]
    ResourceDevelopment[[Resource Development]]
    InitialAccess[[Initial Access]]
    Execution[[Execution]]
    CredentialAccess[[Credential Access]]
    Persistence[[Persistence]]
    PrivilegeEscalation[[Privilege Escalation]]
    LateralMovement[[Lateral Movement]]
    Discovery[[Discovery]]
    Collection[[Collection]]
    CommandAndControl[[Command And Control]]
    Exfiltration[[Exfiltration]]
    Impact[[Impact]]
    DefenseEvasion[[Defense Evasion]]
  end

  %% === rdf:type assertions ===
  OffensiveAction1 -->|rdf type| OffensiveAction
  Attacker1 -->|rdf type| Attacker
  OffensiveTechnique1 -->|rdf type| OffensiveTechnique
  DigitalArtifact1 -->|rdf type| DigitalArtifact

  %% link instances to labels
  OffensiveTactic1 -->|rdf type| Reconnaissance
  OffensiveTactic2 -->|rdf type| ResourceDevelopment
  OffensiveTactic3 -->|rdf type| InitialAccess
  OffensiveTactic4 -->|rdf type| Execution
  OffensiveTactic5 -->|rdf type| CredentialAccess
  OffensiveTactic6 -->|rdf type| Persistence
  OffensiveTactic7 -->|rdf type| PrivilegeEscalation
  OffensiveTactic8 -->|rdf type| LateralMovement
  OffensiveTactic9 -->|rdf type| Discovery
  OffensiveTactic10 -->|rdf type| Collection
  OffensiveTactic11 -->|rdf type| CommandAndControl
  OffensiveTactic12 -->|rdf type| Exfiltration
  OffensiveTactic13 -->|rdf type| Impact
  OffensiveTactic14 -->|rdf type| DefenseEvasion

  %% === Instance level relations ===
  OffensiveAction1 -->|has agent| Attacker1
  OffensiveAction1 -->|implements| OffensiveTechnique1
  OffensiveTechnique1 -->|enables| OffensiveTactic1
  Attacker1 -->|uses| OffensiveTactic1

  %% --- SEQUENCE: full attack chain using "precedes" ---
  OffensiveTactic1 -->|precedes| OffensiveTactic2
  OffensiveTactic2 -->|precedes| OffensiveTactic3
  OffensiveTactic3 -->|precedes| OffensiveTactic4
  OffensiveTactic4 -->|precedes| OffensiveTactic5
  OffensiveTactic5 -->|precedes| OffensiveTactic6
  OffensiveTactic6 -->|precedes| OffensiveTactic7
  OffensiveTactic7 -->|precedes| OffensiveTactic8
  OffensiveTactic8 -->|precedes| OffensiveTactic9
  OffensiveTactic9 -->|precedes| OffensiveTactic10
  OffensiveTactic10 -->|precedes| OffensiveTactic11
  OffensiveTactic11 -->|precedes| OffensiveTactic12
  OffensiveTactic12 -->|precedes| OffensiveTactic13
  OffensiveTactic13 -->|precedes| OffensiveTactic14

  %% link the action to the artifact
  OffensiveAction1 -->|has participant| DigitalArtifact1

  %% === LEGEND ===
  subgraph Legend
    AA{Individual}
    BB[Class]
    CC[data]
    EE[CCO superclass]
    BB --> |relation| CC
    DD[This pattern uses numbered instances but can be reused for other scenarios]
  end

  %% === STYLING ===
  classDef yellow fill:#ffe680,stroke:#333,stroke-width:1px;
  classDef purple fill:#dbc9ef,stroke:#333,stroke-width:1px;
  classDef white fill:#ffffff,stroke:#333,stroke-width:1px;
  classDef grey fill:#d9d9d9,stroke:#333,stroke-width:1px;

  %% Assign colors
  class OffensiveAction,Attacker,OffensiveTechnique,DigitalArtifact yellow
  class OffensiveAction1,Attacker1,OffensiveTechnique1,OffensiveTactic1,OffensiveTactic2,OffensiveTactic3,OffensiveTactic4,OffensiveTactic5,OffensiveTactic6,OffensiveTactic7,OffensiveTactic8,OffensiveTactic9,OffensiveTactic10,OffensiveTactic11,OffensiveTactic12,OffensiveTactic13,OffensiveTactic14,DigitalArtifact1 purple
  class Reconnaissance,ResourceDevelopment,InitialAccess,Execution,CredentialAccess,Persistence,PrivilegeEscalation,LateralMovement,Discovery,Collection,CommandAndControl,Exfiltration,Impact,DefenseEvasion yellow

  %% Color legend items
  class AA purple
  class BB yellow
  class CC white
  class EE grey
  class DD white
