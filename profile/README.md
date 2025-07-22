# Welcome to Brick Labs


```mermaid
graph TD
    
    subgraph API
        style API fill:#fdd
        Vulkan
    end

    subgraph Libraries
        Renderer
        Filehandler
    end

    subgraph Applications
        Viewer
        Builder
        Editor
        FilmMaker
    end

    %% APIs to Libraries
    Vulkan --> Renderer
    Vulkan --> GLFW
    Vulkan --> ImGUI

    %% Libraries to Libraries
    ImGUI --> BLGUI

    %% Librararies to Applications
    Renderer --> Viewer
    Renderer --> Builder

    GLFW --> Viewer
    GLFW --> Builder

    BLGUI --> Viewer
    BLGUI --> Builder

    Filehandler --> Viewer
```


This chart shows the various projects this organization is working on and its external dependencies.
