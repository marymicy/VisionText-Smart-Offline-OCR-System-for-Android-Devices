# VisionText: High-Performance Offline OCR Framework for Android

VisionText is an advanced Optical Character Recognition (OCR) solution engineered for secure, real-time text extraction on edge devices. By leveraging a hybrid integration of Google ML Kit and optimized recognition engines, the system achieves sub-second latency for text detection and extraction without requiring an active network connection.

---

## Technical Architecture

The framework is built to address the critical requirement for privacy-compliant data processing. VisionText ensures that 100% of image analysis occurs locally on the hardware, eliminating data transit risks.

### Core Capabilities

* **On-Device Intelligence:** Zero-latency text extraction using local machine learning models.
* **Real-Time Spatial Mapping:** Dynamic coordinate-based mapping of text blocks with immediate visual feedback via high-precision overlays.
* **Granular Data Selection:** Interactive selection logic allowing users to isolate and extract specific data points.
* **Resource Efficiency:** Optimized for minimal CPU and memory overhead.

---

## Performance & Output Analysis

The following data represents the system's accuracy in spatial mapping and hardware resource management.

### System Visualization & Extraction
| Detection Phase | Extraction Result | Selection UI |
| :--- | :--- | :--- |
| ![Mapping](assets/output-1) | ![Extraction](assets/output-2) | ![UI](assets/output-3) |

### Advanced Processing
| Multi-Line Handling | Document Segmentation | Logic Verification |
| :--- | :--- | :--- |
| ![Lines](assets/output-4) | ![Segments](assets/output-5) | ![Logic](assets/output-6) |

### Resource Management
The system is optimized for edge computing. Below is the recorded CPU utilization during a high-density text scan:
![CPU Utilization](assets/cpu%20usage)

---

## Implementation Pipeline

The application manages the OCR lifecycle through a specialized six-stage technical pipeline:

1. **User Interface Layer:** Streamlined interface implemented via `activity_main.xml`.
2. **Asynchronous Image Acquisition:** Integration of the CameraX API for high-resolution capture.
3. **Neural Text Recognition:** Utilization of the Google ML Kit Text Recognizer.
4. **Spatial Visualization:** Custom `TextOverlayView.kt` for real-time rendering.
5. **Interactive Event Handling:** Event-driven touch listeners for text selection.
6. **Data Output Management:** Automated string processing for clipboard export.

---

## Technical Specifications

* **Language:** Kotlin 1.9+
* **Minimum SDK:** API Level 24 (Android 7.0)
* **Target SDK:** API Level 34
* **Core Dependencies:** Google ML Kit, CameraX, Kotlin Coroutines

---

## Project Origins

This system was developed as a collaborative initiative by a team of six developers focused on edge-computing and mobile machine learning implementations.
