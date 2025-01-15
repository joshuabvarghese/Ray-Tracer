# Ray Tracer

This is a full implementation of Peter Shirley's *Ray Tracing in One Weekend* guide, rewritten in Zig. The project demonstrates how to build a simple ray tracer from scratch, capable of producing stunning images by simulating the behavior of light rays in a 3D environment.

## Features
- **Ray Tracing Core:** Implements fundamental ray tracing concepts, including rays, spheres, and planes.
- **Realistic Lighting:** Simulates diffuse, reflective, and refractive surfaces.
- **Camera System:** Generates perspective views with configurable field of view and aspect ratio.
- **Materials:** Supports Lambertian (diffuse), metal (reflective), and dielectric (refractive) materials.
- **Image Output:** Outputs rendered images in PPM format.
- **Performance Optimization:** Efficiently uses Zig’s safety, performance, and modern tooling.


### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/joshuabvarghese/ray-tracer.git
   cd zig-ray-tracer
   ```
2. Build the project:
   ```bash
   zig build
   ```
3. Run the ray tracer:
   ```bash
   zig build run
   ```

### Rendering an Image
The rendered output will be saved as `output.ppm` in the project directory. You can view the PPM file using tools like GIMP, Photoshop, or any PPM viewer.

## Project Structure
```
zig-ray-tracer/
├── src/
│   ├── main.zig        # Entry point of the application
│   ├── vec3.zig        # Vector math utilities
│   ├── ray.zig         # Ray structure and operations
│   ├── hittable.zig    # Spheres and surface intersection logic
│   ├── material.zig    # Material properties (diffuse, reflective, etc.)
│   ├── camera.zig      # Camera and perspective transformations
│   └── scene.zig       # Scene setup and rendering logic
├── build.zig           # Build system configuration
└── README.md           # Project documentation
```


## Acknowledgments
- **Peter Shirley:** Author of *Ray Tracing in One Weekend*. Original guide: [https://raytracing.github.io/books/RayTracingInOneWeekend.html](https://raytracing.github.io/books/RayTracingInOneWeekend.html).
