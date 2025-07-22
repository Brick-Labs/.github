# Welcome to Brick Labs


```mermaid
graph TD
    
    subgraph APIs
        Vulkan[<a href="https://vulkan.org">Vulkan</a>]
        BLAPI[<span>BrickLabs Web Api</span>]
    end

    subgraph Third-party Libraries
        GLFW[<a href="https://www.glfw.org">GLFW</a>]
        ImGUI[<a href="https://github.com/ocornut/imgui">ImGUI</a>]
    end

    subgraph Libraries
        Renderer[<a href="https://github.com/Brick-Labs/Renderer">Renderer</a>]
        FileHandler[<a href="https://github.com/Brick-Labs/FileHandler">FileHandler</a>]
        BLGUI
    end

    subgraph Applications
        Viewer[<a href="https://github.com/Brick-Labs/Viewer">Viewer</a>]
        Builder
        Engine
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
    Renderer --> Applications
    GLFW --> Applications
    BLGUI --> Applications 
    FileHandler --> Applications

    %% Applications to Applications
    Engine --> Editor
```


This chart shows the various projects this organization is working on and its external dependencies.
