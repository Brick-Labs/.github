# Welcome to Brick Labs


```mermaid
graph TD
    %% APIs to Libraries
    Vulkan --> Renderer
    Vulkan --> GLFW

    %% Librararies to Applications
    Renderer --> Viewer
    Renderer --> Builder

    GLFW --> Viewer
    GLFW --> Builder
```


This chart shows the various projects this organization is working on and its external dependencies.
