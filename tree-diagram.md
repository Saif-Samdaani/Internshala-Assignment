# Tree Diagram — Daily Reflection Tree

Visual representation of all branching paths. Rendered as Mermaid.

```mermaid
flowchart TD
    START([START\nGood evening...]) --> A1_OPEN

    A1_OPEN{A1_OPEN\nOne word for today?}
    A1_OPEN -->|Productive / Mixed| A1_Q1_HIGH
    A1_OPEN -->|Draining / Frustrating| A1_Q1_LOW

    A1_Q1_HIGH{A1_Q1_HIGH\nWhat made a good moment happen?}
    A1_Q1_HIGH -->|Prepared / Quick call| A1_REF_INT
    A1_Q1_HIGH -->|Right people / Lucky| A1_REF_MIXED

    A1_Q1_LOW{A1_Q1_LOW\nFirst move when things went sideways?}
    A1_Q1_LOW -->|Looked for control / Vented then problem-solved| A1_REF_MIXED
    A1_Q1_LOW -->|Waited / Felt stuck| A1_REF_EXT

    A1_REF_INT([A1_REF_INT\nYou stayed in the driver's seat...]) --> BRIDGE_1_2
    A1_REF_MIXED([A1_REF_MIXED\nPulled in different directions...]) --> BRIDGE_1_2
    A1_REF_EXT([A1_REF_EXT\nHard days pull attention outward...]) --> BRIDGE_1_2

    BRIDGE_1_2([BRIDGE\nNow let's shift to what you gave]) --> A2_OPEN

    A2_OPEN{A2_OPEN\nFeeling going into memorable interaction?}
    A2_OPEN -->|Help / add value| A2_Q1_CONTRIB
    A2_OPEN -->|Be heard / recognized| A2_Q1_ENTITLE
    A2_OPEN -->|Get through it / Unsure| A2_Q1_NEUTRAL

    A2_Q1_CONTRIB{A2_Q1_CONTRIB\nDid you follow through?}
    A2_Q1_CONTRIB -->|Helped as intended / Helped differently| A2_REF_CONTRIB
    A2_Q1_CONTRIB -->|Not sure it landed / Something got in way| A2_REF_MIXED

    A2_Q1_ENTITLE{A2_Q1_ENTITLE\nDid you get what you hoped for?}
    A2_Q1_ENTITLE -->|Acknowledged / Overlooked| A2_Q2_ENTITLE
    A2_Q1_ENTITLE -->|Didn't need it / Shifted to them| A2_REF_CONTRIB

    A2_Q1_NEUTRAL{A2_Q1_NEUTRAL\nWhat actually happened?}
    A2_Q1_NEUTRAL -->|Helped more than expected| A2_Q2_CONTRIB
    A2_Q1_NEUTRAL -->|Received / Transactional / Nothing| A2_Q2_ENTITLE

    A2_Q2_CONTRIB{A2_Q2_CONTRIB\nDid something beyond your job?}
    A2_Q2_CONTRIB -->|Helped colleague / Pointed something out| A2_REF_CONTRIB
    A2_Q2_CONTRIB -->|Stuck to plate / Too stretched| A2_REF_MIXED

    A2_Q2_ENTITLE{A2_Q2_ENTITLE\nWorld owe you, or you owe world?}
    A2_Q2_ENTITLE -->|Felt a bit owed| A2_REF_ENTITLE
    A2_Q2_ENTITLE -->|Even / Hadn't thought| A2_REF_MIXED
    A2_Q2_ENTITLE -->|Still had things to give| A2_REF_CONTRIB

    A2_REF_CONTRIB([A2_REF_CONTRIB\nYou showed up for someone else...]) --> BRIDGE_2_3
    A2_REF_MIXED([A2_REF_MIXED\nBoth giving and receiving...]) --> BRIDGE_2_3
    A2_REF_ENTITLE([A2_REF_ENTITLE\nFeeling owed is a signal...]) --> BRIDGE_2_3

    BRIDGE_2_3([BRIDGE\nLet's zoom out to the wider world]) --> A3_OPEN

    A3_OPEN{A3_OPEN\nWho came to mind during biggest challenge?}
    A3_OPEN -->|Just me| A3_Q1_SELF
    A3_OPEN -->|My team| A3_Q1_TEAM
    A3_OPEN -->|Specific person / Customer| A3_Q1_OTHER

    A3_Q1_SELF{A3_Q1_SELF\nDid anyone else cross your mind?}
    A3_Q1_SELF -->|Colleague struggling / Work affects others| A3_REF_MID
    A3_Q1_SELF -->|Heads-down / Overwhelmed| A3_REF_SELF

    A3_Q1_TEAM{A3_Q1_TEAM\nSpecific person you were tracking?}
    A3_Q1_TEAM -->|Noticed + checked in / Adjusted for them| A3_REF_ALTO
    A3_Q1_TEAM -->|Team in background / Didn't act| A3_REF_MID

    A3_Q1_OTHER{A3_Q1_OTHER\nDid it change how you acted?}
    A3_Q1_OTHER -->|Decided differently / Reached out / Felt smaller| A3_REF_ALTO
    A3_Q1_OTHER -->|Noticed but didn't change| A3_REF_MID

    A3_REF_ALTO([A3_REF_ALTO\nYou held more than yourself...]) --> SUMMARY
    A3_REF_MID([A3_REF_MID\nA glimpse of a wider frame...]) --> SUMMARY
    A3_REF_SELF([A3_REF_SELF\nSome days you need all of yourself...]) --> SUMMARY

    SUMMARY([SUMMARY\nPersonalized axis summary]) --> END([END\nSee you tomorrow.])
```

## Axis Color Key
- 🔵 **Axis 1 (Locus):** A1_* nodes — Internal vs External
- 🟡 **Axis 2 (Orientation):** A2_* nodes — Contribution vs Entitlement  
- 🟣 **Axis 3 (Radius):** A3_* nodes — Altrocentric vs Self

## Possible Paths
The tree has **18 distinct terminal states** (3 axis outcomes × 3 axis outcomes × 2 axis outcomes = 18 summary combinations), accessible through dozens of unique traversal paths.
