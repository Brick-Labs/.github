# Welcome to Brick Labs
Welcome to **Brick Labs** – an organization dedicated to building software that revolves around **bricks**.  
Our projects focus on creativity, construction, and digital tools for everyone who loves to build with bricks – virtually or in real life.  

## Projects
```mermaid
graph TD
    
    subgraph APIs
        Vulkan[<a href="https://vulkan.org">Vulkan</a>]
        SteamAPI[<a href="https://partner.steamgames.com/doc/sdk/api">Steamworks-API</a>]
    end

    subgraph Third-party Libraries
        GLFW[<a href="https://www.glfw.org">GLFW</a>]
        ImGUI[<a href="https://github.com/ocornut/imgui">ImGUI</a>]
        spdlog[<a href="https://github.com/gabime/spdlog">spdlog</a>]
        json[<a href="https://github.com/nlohmann/json">json</a>]
        glm[<a href="https://github.com/g-truc/glm">glm</a>]
    end

    subgraph Libraries
        Renderer[<a href="https://github.com/Brick-Labs/Renderer">Renderer</a>]
        FileHandler[<a href="https://github.com/Brick-Labs/FileHandler">FileHandler</a>]
        Logger[<a href="https://github.com/Brick-Labs/Logger">Logger</a>]
        Interface[<a href="https://github.com/Brick-Labs/Interface">Interface</a>]
    end

    subgraph Applications
        Builder[<a href="https://github.com/Brick-Labs/Builder">Builder</a>]
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
    SteamAPI --> FileHandler

    %% Libraries to Libraries
    ImGUI --> Interface
    spdlog --> Logger
    json --> FileHandler
    glm --> Renderer

    %% Librararies to Applications
    Renderer --> Applications
    GLFW --> Applications
    Interface --> Applications 
    FileHandler --> Applications
    Logger --> Applications

    %% APIs to Applications
    SteamAPI --> Applications

    %% Applications to Applications
    Engine --> Editor
```
*This chart shows the various projects this organization is working on and its external dependencies.*
