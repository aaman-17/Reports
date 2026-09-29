**SINGLE-PASS DRONE VIDEO TO ACCURATE 3D MODEL GENERATION SYSTEM**

**Smart India Hackathon 2026**\
**Problem Statement ID:** SIH26057\
**Theme:** Robotics and Drones\
**PS Category:** Software\
**Team ID:** SIH26-21\
**Team Name:** Cognexa 2. O

**1. EXECUTIVE SUMMARY**

The proposed system, Single-Pass Drone Video to Accurate 3D Model Generation System, is able to generate an accurate, textured, georeferenced 3D model from a single continuous drone video with associated GPS and flight information.

The system aims to reduce the time and manual work involved in converting drone imagery into some form of a useful 3D representation. It implements computer vision, AI-assisted processing and a native photogrammetry pipeline consisting of COLMAP, OpenMVS and PoissonRecon.

The resulting 3D model can be used for measuring height, depth, distance and area. The system is intended for applications such as disaster assessment, infrastructure inspection, mapping and analysis.

The prototype combines a browser-based interface using React, TypeScript and Three.js with a Node.js and tRPC backend, database-backed reconstruction jobs, object storage and a native reconstruction pipeline.

**2. INTRODUCTION**

Drones offer an efficient way of capturing visual information of large, complex and hard-to-reach areas. However, converting drone video into a detailed and measured 3D model requires several stages of image processing and reconstruction.

The proposed system solves this requirement through a single-pass drone approach. A continuous drone flight captures the required visual information, which is then processed using computer vision and photogrammetry techniques to generate a textured 3D model.

The system uses drone video, GPS and flight metadata combined with AI, computer vision and existing 3D reconstruction frameworks to produce a realistic, measurable representation of the surveyed environment.

**3. PROBLEM SIGNIFICANCE**

Conventional drone-based mapping and inspection methods may involve extensive data capture and manual processing. Multiple passes and image processing can make it difficult to quickly obtain useful spatial information.

The value of this project is that it allows for the generation of a meaningful 3D model from a single pass, reducing the amount of manual processing.

The system offers the following capabilities:

• 3D model generation from a single pass of a drone,

• measuring heights, depths, distances, and areas,

• generating geographically accurate 3D models,

• enhanced situational awareness in 3D,

• safe inspection of dangerous and hard-to-reach places,

• hazard and disaster assessment,

• efficient repeat inspection of the road, structures, and terrain,

• reduced reliance on expensive hardware.

**4. EXISTING GAPS**

The existing approach has several gaps which could impact the speed, quality and usefulness of 3D reconstruction.

  ----------------------------------------------------------------------------------
  **Existing Gap**           **Impact**                 **Proposed Solution**
  -------------------------- -------------------------- ----------------------------
  Slow manual processing     Errors and delays          Automated native pipeline

  Sparse video views         Poor 3D reconstruction     COLMAP + OpenMVS

  Generic inspection model   False or hidden surfaces   Provenance-aware 360° view

  No completion control      Missing completion data    Completion detection

  Unclear data source        Engineering uncertainty    Provenance-based report
  ----------------------------------------------------------------------------------

The proposed system would fill the gaps by combining automated processing, photogrammetry, 3D visualisation and provenance-based information.

**5. PROPOSED SOLUTION**

The proposed solution converts a single continuous drone video and GPS/flight information into an accurate textured and georeferenced 3D model. The system follows an automated reconstruction process that consists of the following steps: image processing, camera pose estimation, dense reconstruction, surface reconstruction and 3D visualisation.

The main components of the proposed solution are:

1\. Single-pass drone video and GPS data acquisition.

2\. Image and video upload.

3\. Image processing and segmentation.

4\. Camera pose estimation using COLMAP.

5\. Dense multi-view stereo using OpenMVS.

6\. Surface and mesh reconstruction using PoissonRecon.

7\. Generation of an accurate textured 3D model.

8\. Georeferenced 3D output.

9\. Interactive 3D visualisation.

10\. Export of reconstructed models in GLB, OBJ, PLY and LAS formats.

The system also provides features such as surface and depth preview, 360° building mode, orbit controls, zoom and pan, mesh-resolution controls and source-image inspection.

**6. SYSTEM WORKFLOW**

Stage 1: Single-Pass Drone Data Capture

A continuous drone flight captures the desired visual data of the target area. Drone video, GPS and flight metadata are used as primary inputs.

Stage 2: Image and Video Upload

The captured images or videos are uploaded via a browser application interface. The prototype supports uploading images or videos.

Stage 3: Image Processing and Segmentation

The uploaded data is processed before reconstruction. Segmentation is included in the reconstruction worker as a preparatory process for further processing.

Stage 4: Camera Pose Estimation

COLMAP is used for camera pose estimation and Structure-from-Motion. This step determines camera positions and relationships between the captured views.

Stage 5: Dense Reconstruction

OpenMVS performs Dense Multi-View Stereo and point-cloud densification, which generates a denser representation of the reconstructed environment.

Stage 6: Surface and Mesh Reconstruction

PoissonRecon is used for surface and mesh reconstruction. The processed 3D information is then reconstructed to form a surface.

Stage 7: 3D Model Generation

The system produces an accurate textured 3D model representing the captured environment. The model is realistic and measurable.

Stage 8: 3D Visualisation and Inspection

The generated model can be viewed within the browser interface using Three.js. The prototype supports orbit, zoom and pan controls, surface and depth preview, 360° building mode and mesh-resolution controls.

Stage 9: Measurement and Analysis

The generated 3D model can be used to derive height, depth, distance and area measurements. It can also be used for inspection, planning and spatial analysis.

Stage 10: Output and Export

The reconstructed data can be exported in formats such as GLB, OBJ, PLY and LAS.

**OVERALL WORKFLOW**

![](drone_drone_media/media/drone_media/media/image1.png){width="3.816666666666667in" height="5.365574146981627in"}

**7. TECHNICAL ARCHITECTURE**

The proposed system consists of a frontend, backend, database and storage layer, and a native reconstruction pipeline.

**7.1 Frontend Technologies**

-   **React 19:** User interface and application components.

-   **TypeScript:** Type-safe frontend and backend code.

-   **Vite:** Development server and production frontend build.

-   **Three.js:** Interactive 3D preview, orbit controls and mesh visualisation.

-   **React Query / tRPC React:** Typed API communication and server-state management.

-   **Tailwind CSS 4:** Styling and responsive layout.

-   **Lucide React:** Interface icons.

-   **Wouter:** Lightweight client-side routing.

-   **Transformers.js:** Browser-side AI and depth-processing support.

-   **WebGL:** Hardware-accelerated 3D rendering in the browser.

**7.2 Backend Technologies**

-   **Node.js:** Server runtime.

-   **Express:** HTTP server.

-   **tRPC 11:** Type-safe API procedures.

-   **Zod:** Input validation.

-   **Drizzle ORM:** Database schema and queries.

-   **MySQL/TiDB-compatible Database:** Storage of users and reconstruction job records.

-   **S3-Compatible Storage:** Storage of uploaded image and video files.

-   **Manus OAuth:** User authentication.

**7.3 Reconstruction Pipeline**

The native reconstruction pipeline uses:

-   **COLMAP:** Camera pose estimation and Structure-from-Motion.

-   **OpenMVS:** Dense Multi-View Stereo and point-cloud densification.

-   **PoissonRecon:** Surface and mesh reconstruction.

-   **OpenCV:** Image processing and computer vision.

-   **Python:** Reconstruction worker and pipeline orchestration.

-   **CUDA/NVIDIA GPU:** Optional acceleration for native reconstruction.

-   **vcpkg:** C++ dependency management for OpenMVS.

-   **7.4 System Architecture**

![](drone_drone_media/media/drone_media/media/image2.png){width="4.511905074365704in" height="6.528915135608049in"}

**8. INNOVATION**

The suggested system involves several key innovations:

8.1 Measure Anything

The suggested system allows measuring the height, width, distance and building dimensions from the created 3D model.

8.2 AI Damage Scan

The system can identify structural damage, debris, flooding, road blockage or deformation.

8.3 3D Geo-Mapping

The system allows obtaining a precise and georeferenced 3D model from a single pass.

8.4 Risk Zones

The system allows defining the severely damaged or high-priority regions for responders.

8.5 Single-Pass Reconstruction

The system allows using a single continuous flight of a drone to build a 3D model, rather than multiple passes.

8.6 Automated Processing

The system reduces the need for manual processing and allows automatic reconstruction of the 3D model from images.

**9. FEASIBILITY AND VIABILITY**

9.1 Technical Feasibility

Drone video, GPS and flight metadata can be acquired from existing drone platforms and datasets.

The system uses AI, computer vision and existing 3D reconstruction frameworks to support single-pass reconstruction. Python-based modules can be used for video processing, depth estimation, 3D reconstruction and the incorporation of geospatial data.

The reconstruction pipeline uses established tools such as COLMAP, OpenMVS and PoissonRecon.

9.2 Economic Feasibility

The system uses existing drones and does not require custom hardware. The prototype can run using available GPU or cloud infrastructure.

The software-based approach reduces the requirement for additional specialised hardware for individual missions.

9.3 Viability

The proposed system is likely to be:

• Platform independent.

• Adaptable to different environments.

• Scalable for different applications.

• Reusable for different missions.

• Upgradable with improved AI models.

**10. IMPACT AND BENEFITS**

The benefits of the proposed system include:

**Single-Pass Reconstruction**

Generates a useful 3D model from a single continuous drone flight

Enables

**Actionable measurements**

Heights, depths, distances, and areas can be found using the 3D model

offers

**High cost and hardware savings**

Uses existing drone images and requires no specialised hardware

and

**Has a wide range of potential applications**

Can be used for disaster assessment, infrastructure inspection, and more.

Additionally,

it enables rapid 3D situational awareness by converting a single drone pass into a 3D model for faster understanding of the environment.

Also,

estimates heights and depths of buildings, terrain, and objects in the scene, as well as distances.

Moreover,

it allows safer and more distant inspections of dangerous or inaccessible locations without requiring multiple surveys.

It also facilitates improved spatial and environmental awareness and supports informed decision-making with a measurable 3D environment for inspection and planning. Finally, it reduces the time between flight and 3D scene reconstruction to allow faster survey turnaround and enables better infrastructure monitoring, including roads, buildings, and other objects of interest.

**11. IMPLEMENTATION PLAN**

The implementation of the proposed system can be divided into the following stages:

  -------------------------------------------------------------------------
  **Phase**   **Activity**
  ----------- -------------------------------------------------------------
  Phase 1     Develop the React and TypeScript frontend.

  Phase 2     Implement image and video upload.

  Phase 3     Develop a Node.js, Express and tRPC backend.

  Phase 4     Integrate database and S3-compatible storage.

  Phase 5     Develop the reconstruction worker.

  Phase 6     Integrate image processing and segmentation.

  Phase 7     Integrate COLMAP for camera pose estimation.

  Phase 8     Integrate OpenMVS for dense reconstruction.

  Phase 9     Integrate PoissonRecon for surface and mesh reconstruction.

  Phase 10    Generate textured 3D models.

  Phase 11    Implement Three. js-based 3D visualisation and inspection

  Phase 12    Implement model export and test the complete workflow.
  -------------------------------------------------------------------------

The browser prototype is recommended to run in a Windows environment, while the native reconstruction tools such as COLMAP, OpenMVS and PoissonRecon are recommended to run using Linux or WSL2.

**12. EVALUATION METHODOLOGY**

The system can be assessed based on several criteria:

12.1 **3D Reconstruction**

-   Ability to create a 3D model from a single drone pass

-   Quality of the resulting geometry

-   Generation of a textured 3D model

12.2 **Measurement**

Extraction of:

-   Height

-   Depth

-   Distance

-   Area

12.3 **Geospatial Output**

generation of a geospatial 3D output by tying the reconstructed information to a coordinate system

12.4 **Processing**

can be assessed upon:

-   Reduction in manual labour

-   Time needed to process the drone images into a 3d scene

-   Successful completion of the reconstruction pipeline

12.5 **Prototype Functionality**

can be assessed based on:

-   Image and video upload

-   Creation of reconstruction jobs

-   Preview of surface and depth

-   360° building mode

-   Orbit, zoom and pan controls

-   Mesh-resolution controls

-   Source image inspection

-   Reconstruction pipeline status

-   3D model export

**13. RISKS AND LIMITATIONS**

The proposed system has the following technical limitations:

1\. High-accuracy native reconstruction requires Linux or WSL2 together with COLMAP, OpenMVS, PoissonRecon and the configured reconstruction worker.

2\. An NVIDIA GPU is optional, but can accelerate native processing when CUDA and WSL2 GPU access are configured correctly.

3\. The browser prototype and native reconstruction pipeline operate in different recommended environments.

4\. The reconstruction process depends on multiple native components, including COLMAP, OpenMVS and PoissonRecon.

5\. The current browser prototype provides upload, preview, inspection and reconstruction-job capabilities, while the native reconstruction pipeline provides the complete processing capability.

6\. Processing requirements may vary depending on the input imagery and reconstruction configuration.

**14. BUSINESS AND ADOPTION MODEL**

The offered system may be applied in the following spheres, which require drone-based surveying, inspection, and 3D analysis:

• Disaster assessment.

• Infrastructure inspection.

• City mapping.

• Terrain mapping.

• Road monitoring.

• Building inspection.

• Hazardous-area assessment.

• Monitoring of repeatable infrastructure.

The software may be used in multiple missions and does not require specific hardware for each task. The given documents do not include any information concerning the pricing policy, subscription, or revenue policy; thus, it is impossible to offer any specific commercial proposition.

**15. CONCLUSION**

A single-pass drone video to accurate textured and georeferenced 3D model generation system works on the concept of a software system that makes it possible to obtain an accurate 3D model from a video captured by a single drone during one continuous flight.

The developed architecture is integrated with a React and Three.js interface, a Node.js and tRPC-backed, database-driven job system, object storage, and a photogrammetry pipeline written in COLMAP, OpenMVS, PoissonRecon, and other tools.

The proposed system would enable measurement, mapping, disaster response assessment, infrastructure inspections, and 3D situational awareness while reducing the amount of manual labour and multiple data collection passes needed.

**16. REFERENCES**

1.  **3D Gaussian Splatting for Real-Time Radiance Field Rendering.** DOI: 10.1145/3592433.

2.  **Drone-NeRF: NeRF-Based 3D Scene Reconstruction for Large-Scale Drone Survey.** DOI: 10.1016/j.imavis.2024.104920.

3.  **DROID-SLAM: Deep Visual SLAM for Monocular, Stereo, and RGB-D Cameras.** arXiv:2108.10869.

4.  **Structure-from-Motion Revisited.** DOI: 10.1109/CVPR.2016.445.

5.  **COLMAP.** 3D reconstruction using Structure-from-Motion and Multi-View Stereo.

6.  **AliceVision.** Open-source photogrammetry framework.

7.  **OpenDroneMap.** Drone imagery processing and mapping.

8.  **OpenMVS.** Dense 3D reconstruction and mesh generation.

9.  **3DF Zephyr.** Automated photogrammetry and 3D modelling.

10. **Aerotrace Technology Stack.** Technical documentation for the frontend, backend, reconstruction pipeline, architecture and runtime requirements.
