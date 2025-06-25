---
title: "Vulkan Raytracer"
excerpt: "<div style='display: flex; align-items: center; justify-content: space-between; font-size: 14px; background: linear-gradient(135deg, #f5f7fa, #c3cfe2); padding: 20px; border-radius: 12px; box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);'>
              <div style='flex: 1; margin-left: 20px;'>
               <img src='/images/raytracer_vk.png' alt='Vulkan Raytracer' style='max-width: 75%; border-radius: 12px; box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2); transition: transform 0.3s ease;'>
             </div>
             <div style='flex: 1; padding-right: 20px;'>
               <h2 style='font-size: 18px; margin: 10px 0; font-weight: bold; color: #2c3e50; text-transform: uppercase; letter-spacing: 1px;'>Overview</h2>
               <p style='margin: 10px 0; line-height: 1.6; color: #34495e; font-size: 14px;'>This project is a Vulkan-based raytracer that utilizes the <code>VK_KHR_ray_tracing_pipeline</code> extension. It implements real-time ray tracing with acceleration structures and features such as temporal anti-aliasing, any-hit shaders for transparency, and sample accumulation directly in the ray generation shader. It was later extended into a recursive path tracer for realistic lighting simulations.</p>

               <h2 style='font-size: 18px; margin: 10px 0; font-weight: bold; color: #2c3e50; text-transform: uppercase; letter-spacing: 1px;'>Key Features</h2>
               <ul style='list-style-type: none; padding-left: 0;'>
                 <li style='margin: 8px 0; color: #34495e; font-size: 14px;'><span style='color: #863ce7; font-weight: bold; margin-right: 8px;'>•</span> <b>Use of Acceleration Structure</b>: Efficient ray-triangle intersections using Vulkan's acceleration structures.</li>
                 <li style='margin: 8px 0; color: #34495e; font-size: 14px;'><span style='color: #863ce7; font-weight: bold; margin-right: 8px;'>•</span> <b>Temporal Anti-Aliasing</b>: Subpixel jitter with per-frame accumulation for smoother edges and better image quality.</li>
                 <li style='margin: 8px 0; color: #34495e; font-size: 14px;'><span style='color: #863ce7; font-weight: bold; margin-right: 8px;'>•</span> <b>Any-Hit Shader</b>: Supports alpha cutout and conditional intersection handling, useful for simulating transparent surfaces.</li>
                 <li style='margin: 8px 0; color: #34495e; font-size: 14px;'><span style='color: #863ce7; font-weight: bold; margin-right: 8px;'>•</span> <b>Recursive Path Tracing</b>: Path tracing implemented in the RayGen shader for optimal sample accumulation without excessive traceRay calls.</li>
               </ul>

               <h3 style='font-size: 16px; margin: 10px 0; font-weight: bold; color: #2c3e50; text-transform: uppercase;'>Performance Optimizations</h3>
               <ul style='list-style-type: none; padding-left: 0;'>
                 <li style='margin: 8px 0; color: #34495e; font-size: 14px;'><span style='color: #863ce7; font-weight: bold; margin-right: 8px;'>•</span> Sample accumulation done inside the RayGen shader loop to avoid performance-heavy multiple trace calls.</li>
                 <li style='margin: 8px 0; color: #34495e; font-size: 14px;'><span style='color: #863ce7; font-weight: bold; margin-right: 8px;'>•</span> Utilizes Vulkan's efficient memory handling and AS compaction to maintain responsiveness.</li>
               </ul>

               <h2 style='font-size: 18px; margin: 10px 0; font-weight: bold; color: #2c3e50; text-transform: uppercase; letter-spacing: 1px;'>Repository</h2>
               <a href='https://github.com/SuvrangshuBarua/vk_raytracer' style='text-decoration: none; color: #3498db; font-weight: bold; font-size: 14px; padding: 8px 16px; background: #ecf0f1; border-radius: 6px; display: inline-block; transition: background 0.3s ease;'>View on GitHub</a>
             </div>
           </div>"
collection: project
---

## Overview

**Vulkan Raytracer** is a graphics rendering project focused on implementing real-time ray tracing using the Vulkan API. The project began as a basic raytracer and evolved into a full-fledged path tracer leveraging Vulkan’s ray tracing extension to achieve realism through recursive light simulation.

## Key Features

- **Acceleration Structures**: Reduces computational overhead by minimizing unnecessary ray-triangle intersection tests.
- **Temporal Anti-Aliasing**: Achieved through subpixel jittering and sample accumulation across frames.
- **Efficient Sampling**: All samples are accumulated inside the RayGen shader, avoiding costly multi-pass ray tracing.
- **Any-Hit Shader**: Discards intersections based on material transparency, enabling support for alpha cutouts.
- **Path Tracing Upgrade**: Implements recursion in the RayGen shader, supporting multiple light bounces per frame.

## Performance Notes

- Uses direct sample accumulation in the RayGen shader for speed.
- Reduces unnecessary shader invocations by handling transparency early.
- Optimized for experimental research and educational rendering projects.

## Repository

You can explore the source code and contributions on the [Vulkan Raytracer GitHub repository](https://github.com/SuvrangshuBarua/vk_raytracer).

