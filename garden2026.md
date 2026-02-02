```mermaid

graph TB
    subgraph Garden[Garden Grid]
        direction TB
                
        subgraph Row1[Row 1 - North]
            direction LR
            R1[1] --- A1["Garlic"] --- B1["carrots"] --- C1["bunching onions"] --- D1["x"] --- E1["x"] --- F1["x"] --- G1["Tomato"] --- H1["x"]
        end
        
        subgraph Row2[Row 2]
            direction LR
            R2[2] --- A2["x"] --- B2["x"] --- C2["Chives"] --- D2["x"] --- E2["Marigolds"] --- F2["bunching<br>onions"] --- G2["x"] --- H2["x"]
        end
        
        subgraph Row3[Row 3]
            direction LR
            R3[3] --- A3["Strawberry"] --- B3["Strawberry"] --- C3["x"] --- D3["x"] --- E3["Leek"] --- F3["Marigolds"] --- G3["x"] --- H3["x"]
        end
        
        subgraph Row4[Row 4 - South]
            direction LR
            R4[4] --- A4["x"] --- B4["x"] --- C4["x"] --- D4["x"] --- E4["x"] --- F4["x"] --- G4["x"] --- H4["x"]
        end
        
        %% Connect rows vertically
        Cols --- Row1
        Row1 --- Row2
        Row2 --- Row3
        Row3 --- Row4
    end

    classDef default fill:#1b4d3e,stroke:#333,stroke-width:4px,font-size:28px,font-weight:bold;
    classDef cell text-align:center,width:150px,height:150px;
    classDef header fill:#f9f9f9,stroke:#666;
    class A1,B1,C1,D1,E1,F1,G1,H1,A2,B2,C2,D2,E2,F2,G2,H2,A3,B3,C3,D3,E3,F3,G3,H3,A4,B4,C4,D4,E4,F4,G4,H4 cell;
    class Cols,R1,R2,R3,R4 header;

    ```
