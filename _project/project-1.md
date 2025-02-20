---
title: "Pathtracer"
excerpt: "<div style='display: flex; align-items: center; justify-content: space-between; font-size: 14px;'>
             <div style='flex: 1;'>
               <h2 style='font-size: 16px; margin: 5px 0; font-weight: bold; color: #2c3e50;'>Description</h2>
               <p style='margin: 5px 0; line-height: 1.5; color: #34495e;'>A pathtracer capable of rendering photorealistic images, developed for the Computer Graphics course at Chalmers. This project showcases advanced rendering techniques, including global illumination, material modeling, and importance sampling.</p>

               <h2 style='font-size: 16px; margin: 5px 0; font-weight: bold; color: #2c3e50;'>Libraries</h2>
               <ul style='list-style-type: none; padding-left: 0;'>
                 <li style='margin: 2px 0; color: #34495e;'><span style='color: #e74c3c;'>•</span> OpenGL graphics API</li>
                 <li style='margin: 2px 0; color: #34495e;'><span style='color: #e74c3c;'>•</span> SDL2</li>
                 <li style='margin: 2px 0; color: #34495e;'><span style='color: #e74c3c;'>•</span> CMake</li>
               </ul>

               <h2 style='font-size: 16px; margin: 5px 0; font-weight: bold; color: #2c3e50;'>Link</h2>
               <a href='https://github.com/SuvrangshuBarua/Computer-Graphics-Project' style='text-decoration: none; color: #3498db; font-weight: bold;'>Github Link</a>
             </div>
             <div style='flex: 1; margin-left: 20px;'>
               <img src='/images/pathtracer-1.png' alt='Pathtracer' style='max-width: 100%; border-radius: 8px; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);'>
             </div>
           </div>"
collection: project
---
### **Project: Path Tracer Implementation**

#### **Overview**
A **path tracer** developed from scratch as part of computer graphics course at Chalmers University of Technology. This physically-based rendering engine simulates light behavior in 3D scenes to generate realistic images, demonstrating my understanding of ray tracing, material modeling, and advanced rendering techniques.

#### **Key Features**
- **Ray Tracing Core**: Implemented ray generation, intersection testing, and recursive shading for global illumination.
- **Material Models**: Developed **diffuse**, **metal**, and **dielectric** materials using **BSDFs**, including **Fresnel reflections** for glass-like surfaces.
- **Lighting**: Calculated direct illumination from point lights and indirect illumination through path tracing. Integrated **environment maps** for realistic lighting.
- **Importance Sampling**: Improved efficiency with **cosine-weighted sampling** (diffuse) and **microfacet sampling** (glossy/metals).
- **Optimizations**: Used **Russian Roulette** for path termination and **epsilon offsets** to avoid numerical instability.

#### **Technologies**
- **Languages**: C++
- **Libraries**: GLM for vector/matrix math.
- **Algorithms**: Custom ray tracing, path tracing, and importance sampling.

#### **Results**
- Produced realistic images with accurate lighting, reflections, and refractions.
- Achieved efficient rendering through advanced sampling techniques.

#### **Relevance**
This project showcases my ability to implement complex rendering algorithms and my understanding of computer graphics principles. It highlights my skills in C++, mathematics, and problem-solving, making it a strong addition to my portfolio.

