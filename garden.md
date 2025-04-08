```mermaid
graph TB
    subgraph Garden[Garden Grid]
        direction TB
                
        subgraph Row1[Row 1]
            direction LR
            R1[1] --- A1["Genovese<br/>Basil"] --- B1["Tomato"] --- C1["Empty"] --- D1["Empty"] --- E1["Empty"] --- F1["Empty"] --- G1["Tomato"] --- H1["Strawberry"]
        end
        
        subgraph Row2[Row 2]
            direction LR
            R2[2] --- A2["Empty"] --- B2["Empty"] --- C2["Empty"] --- D2["Empty"] --- E2["Empty"] --- F2["Empty"] --- G2["Empty"] --- H2["Watermelon"]
        end
        
        subgraph Row3[Row 3]
            direction LR
            R3[3] --- A3["Empty"] --- B3["Garlic<br/>Chives"] --- C3["Bunching<br/>Onions"] --- D3["Empty"] --- E3["Leek"] --- F3["Bush<br/>Bean"] --- G3["Empty"] --- H3["Cantaloupe"]
        end
        
        subgraph Row4[Row 4]
            direction LR
            R4[4] --- A4["Dwarf<br/>Marigold"] --- B4["Empty"] --- C4["Baby<br/>Romaine"] --- D4["Baby<br/>Butterhead"] --- E4["Genovese<br/>Basil"] --- F4["Empty"] --- G4["Strawberry"] --- H4["Strawberry"]
        end
        
        %% Connect rows vertically
        Cols --- Row1
        Row1 --- Row2
        Row2 --- Row3
        Row3 --- Row4
    end

    classDef default fill:#fff,stroke:#333,stroke-width:2px;
    classDef cell text-align:center,width:150px,height:150px;
    classDef header fill:#f9f9f9,stroke:#666;
    class A1,B1,C1,D1,E1,F1,G1,H1,A2,B2,C2,D2,E2,F2,G2,H2,A3,B3,C3,D3,E3,F3,G3,H3,A4,B4,C4,D4,E4,F4,G4,H4 cell;
    class Cols,R1,R2,R3,R4 header;

    ```
