```mermaid
graph LR
    WD[Working Directory<br>Carpeta Local]
    SA[Staging Area<br>El Escenario]
    RE[Local Repository<br>La Caja Fuerte]
    GH((GitHub<br>Nube))

    WD -->|git add .| SA
    SA -->|git commit -m| RE
    RE -->|git push| GH

    SA -.->|git reset HEAD| WD
    RE -.->|git checkout --| WD

    style WD fill:#e1f5fe,stroke:#03a9f4,stroke-width:2px,color:#000000
    style SA fill:#e1f5fe,stroke:#03a9f4,stroke-width:2px,color:#000000
    style RE fill:#e1f5fe,stroke:#03a9f4,stroke-width:2px,color:#000000
    style GH fill:#efebe9,stroke:#795548,stroke-width:2px,color:#000000