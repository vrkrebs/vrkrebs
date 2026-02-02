```mermaid

graph TB
    subgraph Garden[Garden Grid]
        direction TB
                
        subgraph Row1[Row 1]
            direction LR
            R1[1] --- A1["Garlic"] --- B1["carrots"] --- C1["bunching<br>onions"] --- D1["Empty"] --- E1["Empty"] --- F1["Empty"] --- G1["Tomato"] --- H1["Empty"]
        end
        
        subgraph Row2[Row 2]
            direction LR
            R2[2] --- A2["Empty"] --- B2["Empty"] --- C2["Chives"] --- D2["Empty"] --- E2["Marigolds"] --- F2["bunching<br>onions"] --- G2["Empty"] --- H2["Empty"]
        end
        
        subgraph Row3[Row 3]
            direction LR
            R3[3] --- A3["Strawberry"] --- B3["Strawberry"] --- C3["Empty"] --- D3["Empty"] --- E3["Leek"] --- F3["Marigolds"] --- G3["Empty"] --- H3["Empty"]
        end
        
        subgraph Row4[Row 4]
            direction LR
            R4[4] --- A4["Empty"] --- B4["Empty"] --- C4["Empty"] --- D4["Empty"] --- E4["Empty"] --- F4["Empty"] --- G4["Empty"] --- H4["Empty"]
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
