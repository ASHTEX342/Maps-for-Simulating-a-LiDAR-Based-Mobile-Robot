# LiDAR Mobile Robot Simulation Maps

Custom 3D test arenas designed in **Autodesk Fusion** for simulating mobile robot navigation, SLAM, obstacle avoidance, and 2D/3D LiDAR raycasting.

## Arena Overview

| Map | Geometry & Obstacle Profile | LiDAR / Navigation Test Focus |
| :--- | :--- | :--- |
| **`map1`** | Enclosed perimeter arena with rectangular and square prism blocks | Orthogonal walls, corridors, right-angle reflections, and baseline path planning |
| **`map2`** | Enclosed perimeter arena with triangular, wedge, and angled prism obstacles | Oblique ray incidence, specular/angled reflections, and non-parallel obstacle avoidance |
| **`map6`** | Enclosed perimeter arena with curved, cylindrical, and multi-profile obstacles | Curved surface contours, narrow/varied clearances, and smooth trajectory tracking |

## Exporting & Using in Simulation

1. **Origin & Units:** Keep the arena floor origin (`0, 0, 0`) consistent across `map1`, `map2`, and `map6`, and convert millimeters (`mm`) to meters (`m`) when importing into ROS / Gazebo / Isaac Sim.
2. **LiDAR Scan Plane:** Ensure obstacle heights exceed your simulated LiDAR mounting plane so scan rays reliably intersect obstacles rather than passing over them.
3. **Recommended Formats:** Export `.step` from Autodesk Fusion for clean CAD exchange, and `.stl` / `.dae` / `.sdf` for physics and sensor simulation engines.

## Credits & Contributors

* **Rakshith S Kumar** — Project contributor / collaborator
* **Anirudh Shridhar** — Project contributor / collaborator

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
