---
layout: publication
title: "Augmented Reality Books: An Immersive Approach to Learning"
publication_id: ar-books
---

## Overview

This paper presents an augmented reality system that transforms traditional textbooks into interactive learning experiences. Students hover their smartphone camera over a page and the system overlays related 3D models, videos, or explanations directly on the identified content — no typing or searching required.

The system supports both **image recognition** (marker-less, using Vuforia feature points) and **text recognition** (printed English words matched against a word list), making it work with a wide range of textbook content.

## System Architecture

A 2-tier client-server architecture keeps the mobile app lightweight. The client handles camera input, autofocus, and content tracking, while the server stores image targets and maps them to corresponding 3D models or videos.

![System Architecture](/assets/images/ar-books/fig-system-architecture.png)

## Results

The system demonstrates three core augmentation capabilities:

**3D Model Augmentation** — When the camera identifies a keyword like "Ceramic Resistors", a 3D model of the component is rendered directly over the text.

![3D Model Augmented on Identified Text](/assets/images/ar-books/fig-model-augmentation.png)

**Video Augmentation** — Hovering over an image target plays an explanatory video with full playback controls.

![Video Augmentation on an Image Target](/assets/images/ar-books/fig-video-augmentation.png)

**Interactive Learning** — The fully deployed system running on a smartphone, augmenting a 3D resistor model on identified text in a real textbook.

![An Interactive Learning System](/assets/images/ar-books/fig-interactive-system.png)
