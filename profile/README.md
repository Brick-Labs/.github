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
        spdlog[<a href="https://github.com/gabime/spdlog">spdlog</a>]
    end

    subgraph Libraries
        Renderer[<a href="https://github.com/Brick-Labs/Renderer">Renderer</a>]
        FileHandler[<a href="https://github.com/Brick-Labs/FileHandler">FileHandler</a>]
        Logger[<a href="https://github.com/Brick-Labs/Logger">Logger</a>]
        BLGUI
    end

    subgraph Applications
        Viewer[<a href="https://github.com/Brick-Labs/Viewer">Viewer</a>]
        Builder
        Engine
        Editor
        FilmMaker
    end

    subgraph Websites
        BrickLabsWeb[<a href="https://github.com/Brick-Labs/Website">BrickLabs</a>]
    end

    %% APIs to Libraries
    Vulkan --> Renderer
    Vulkan --> GLFW
    Vulkan --> ImGUI

    %% APIs to Websites
    BLAPI --> BrickLabsWeb

    %% Libraries to Libraries
    ImGUI --> BLGUI
    spdlog --> Logger
    Logger --> Renderer

    %% Librararies to Applications
    Renderer --> Applications
    GLFW --> Applications
    BLGUI --> Applications 
    FileHandler --> Applications
    Logger --> Applications 

    %% Applications to Applications
    Engine --> Editor
```


This chart shows the various projects this organization is working on and its external dependencies.
