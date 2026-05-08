# VisionText: High-Performance Offline OCR Framework for Android

VisionText is an advanced Optical Character Recognition (OCR) solution engineered for secure, real-time text extraction on edge devices. By leveraging a hybrid integration of Google ML Kit and optimized recognition engines, the system achieves sub-second latency for text detection and extraction without requiring an active network connection.

---

## Technical Architecture

The framework is built to address the critical requirement for privacy-compliant data processing. VisionText ensures that 100% of image analysis occurs locally on the hardware, eliminating data transit risks and ensuring functionality in remote or restricted environments.

### Core Capabilities

* **On-Device Intelligence:** Zero-latency text extraction using local machine learning models and asynchronous processing.
* **Real-Time Spatial Mapping:** Dynamic coordinate-based mapping of text blocks with immediate visual feedback via high-precision overlays.
* **Granular Data Selection:** Interactive selection logic allowing users to isolate and extract specific data points from complex document layouts.
* **Resource Efficiency:** Optimized for minimal CPU and memory overhead, ensuring stability across a broad spectrum of Android hardware.

---

## Implementation Pipeline

The application manages the OCR lifecycle through a specialized six-stage technical pipeline:

1. **User Interface Layer:** A streamlined interface implemented via `activity_main.xml` designed to minimize user friction during high-frequency data entry.
2. **Asynchronous Image Acquisition:** Integration of the CameraX API for high-resolution bitmap capture with automated permission management.
3. **Neural Text Recognition:** Utilization of the Google ML Kit Text Recognizer for sophisticated segmentation of text blocks, lines, and word-level entities.
4. **Spatial Visualization:** A custom `TextOverlayView.kt` component that renders precision bounding boxes based on engine-provided spatial coordinates.
5. **Interactive Event Handling:** Event-driven touch listeners that facilitate real-time state changes and selection of specific detected text segments.
6. **Data Output Management:** Automated string processing that formats extracted data for immediate export to the system clipboard.

---

## Technical Specifications

* **Development Environment:** Android Studio Ladybug or later
* **Language:** Kotlin 1.9+
* **Minimum SDK:** API Level 24 (Android 7.0)
* **Target SDK:** API Level 34
* **Core Dependencies:** Google ML Kit, CameraX, Kotlin Coroutines

---

## Project Origins

This system was developed as a collaborative initiative by a team of six developers focused on edge-computing and mobile machine learning implementations. The goal was to produce a model that runs efficiently on low-resource hardware without compromising on recognition accuracy.
