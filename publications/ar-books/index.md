---
layout: publication
title: "Augmented Reality Books: An Immersive Approach to Learning"
publication_id: ar-books
---

## Implementation

The system uses a **marker-less image and text based approach** built on the Vuforia SDK integrated with Unity. A 2-tier client-server architecture separates the rendering (client) from the data storage and processing (server), keeping the app lightweight on mobile devices.

### System Architecture

The architecture divides into a **client side layer** (camera GUI, autofocus, content tracking, marker/text detection) and a **server side layer** (image target database, information retrieval, model mapping). The client identifies whether the target is an image or text, forwards it to the server, which returns the corresponding 3D model or video.

![System Architecture](/assets/images/ar-books/paper-architecture.png)

### Key Modules

- **Image Recognition** — Vuforia's image targets are recognized via feature points (no special markers needed). Images are rated by feature density; higher ratings yield faster recognition.
- **Text Recognition** — Vuforia detects printed English words matched against a pre-defined word list, highlighted with a blue bounding box.
- **Model Augmentation** — 3D models (e.g., a ceramic resistor) are rendered over identified text or images in real-time.
- **Video Augmentation** — Explanatory videos with full playback controls are overlaid on recognized image targets.

![Implementation Details — Vuforia Portal, Image Targets, Text Recognition, Model & Video Augmentation](/assets/images/ar-books/paper-implementation.png)

### Deployment & Results

The system is deployed cross-platform via Unity (Android, iOS). Users install the app, hover their smartphone camera over a textbook page, and the system augments 3D models, videos, or explanations over the identified content.

![Deployment and Interactive Learning System](/assets/images/ar-books/paper-results.png)

### Proposed System Flow

![Proposed System Flow](/assets/images/ar-books/paper-proposed-approach.png)
