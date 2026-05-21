```mermaid
gitGraph
    commit id: "Base del proyecto"
    commit id: "Estructura HTML/CSS"
    branch feature-login
    checkout feature-login
    commit id: "Formulario de login"
    commit id: "Validación de contraseña"
    checkout main
    commit id: "Arreglo bug en portada"
    merge feature-login id: "Unión de rama login a main"
    commit id: "Versión final estable"