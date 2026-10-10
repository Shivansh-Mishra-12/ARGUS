# ARGUS 👁️
### Autonomous Real-time Guardian for Unusual Situations

**An AI-powered situational awareness system designed to detect potential safety incidents from CCTV footage and trigger timely alerts for human review.**

> *It doesn't just see. It analyzes what might be happening.*

---

## 📌 Overview

ARGUS is an experimental AI-powered surveillance and incident-detection project that aims to go beyond traditional object detection.

Conventional object detection models can identify people and objects in a video feed, but identifying an object alone does not explain the situation unfolding around it.

ARGUS aims to bridge this gap by combining computer vision, object tracking, temporal analysis, and intelligent decision-making to identify potentially dangerous situations and notify authorized personnel.

The long-term vision is to help improve situational awareness in environments such as retail stores, offices, and other public or commercial spaces.

**ARGUS is currently a work in progress.** Its detection capabilities, reliability, and real-world applicability will be evaluated throughout development.

## 🎯 Objectives

- **Real-time perception:** Analyze CCTV footage using computer vision.
- **Object detection:** Identify people and relevant objects within a scene.
- **Temporal analysis:** Examine sequences of events rather than isolated video frames.
- **Incident recognition:** Investigate methods for identifying predefined safety-related activities.
- **Intelligent decision-making:** Evaluate structured decision models, including JEV, alongside conventional rule-based approaches.
- **Automated notifications:** Generate alerts containing relevant incident information for human review.
- **Privacy-conscious processing:** Explore local video processing and secure handling of recorded footage.

## 🧠 Proposed Architecture

```text
       CCTV / Video Input
               |
               v
      Video Frame Processing
               |
               v
       Object Detection
             (YOLO)
               |
               v
      Object Tracking & Analysis
               |
               v
       Temporal Event Analysis
               |
               v
     Incident Classification
        (JEV / Rules)
               |
               v
       Safety & Verification
               |
               v
      Alert & Review Dashboard
```

The architecture is a proposed development plan. Individual components will be evaluated and integrated incrementally.

### Core Components

| Component | Purpose |
|---|---|
| YOLO | Detect people and supported objects in video frames |
| Object tracking | Associate detections across successive frames |
| Pose estimation / action recognition | Explore body movement and activity analysis |
| Temporal analysis | Interpret patterns across multiple frames |
| JEV / rule-based decision layer | Evaluate structured observations against predefined categories |
| Alert system | Notify designated reviewers about potential incidents |

OpenCV may be used for video capture, frame processing, visualization, and related computer vision utilities. It is a supporting tool, not a replacement for the detection model.

The final architecture will depend on experimental results and performance requirements.

## 🚀 Development Roadmap

- [ ] **Phase 1 — Video Processing:** Load and process prerecorded CCTV footage.
- [ ] **Phase 2 — Object Detection:** Integrate YOLO and visualize supported detections.
- [ ] **Phase 3 — Object Tracking:** Track detected objects across consecutive frames.
- [ ] **Phase 4 — Activity Analysis:** Investigate pose estimation and temporal action recognition.
- [ ] **Phase 5 — Incident Classification:** Develop and evaluate a predefined incident-classification pipeline.
- [ ] **Phase 6 — Decision Layer:** Compare JEV-assisted classification with conventional rules.
- [ ] **Phase 7 — Alert System:** Build an alert dashboard and simulated notification workflow.
- [ ] **Phase 8 — Evaluation:** Measure detection performance, false alarms, processing latency, and resource usage.
- [ ] **Phase 9 — Optimization:** Explore edge deployment, local processing, and privacy safeguards.

## 📊 Evaluation Goals

ARGUS will be evaluated using measurable performance criteria, including:

- **Precision:** How often detected incidents correspond to actual incidents in the test data.
- **Recall:** How many incidents in the test data are successfully detected.
- **False alarm rate:** How frequently harmless activity triggers an alert.
- **Detection latency:** The time required to identify a potential incident.
- **Processing performance:** Frame-processing speed and resource consumption.
- **Robustness:** Performance under different lighting, camera angles, and scene conditions.

These metrics will help determine whether each development stage provides a meaningful improvement.

## 🔐 Safety, Privacy & Responsible Use

ARGUS is an experimental decision-support system, not an autonomous law-enforcement system.

- An AI-generated alert must not be treated as proof that a crime has occurred.
- Human verification is required before escalating a potential incident to emergency services.
- Testing should begin with prerecorded or safely staged footage.
- Video data should be handled securely, with access limited to authorized individuals.
- Privacy, applicable laws, and consent requirements must be considered during development and deployment.
- Detection limitations and false positives must be documented transparently.

## 🛠️ Planned Technology Stack

The technology stack will evolve as development progresses.

- **Language:** Python
- **Computer Vision:** OpenCV
- **Object Detection:** YOLO
- **Machine Learning:** PyTorch and compatible model libraries, as required
- **Decision-Making:** JEV and conventional rule-based approaches under evaluation
- **Interface:** To be determined
- **Deployment:** Local processing initially, with edge deployment explored later

These technologies are planned or under evaluation; their inclusion does not imply that they have already been integrated.

## 🧪 Current Status

**Status: Early-stage development / architecture planning**

The initial focus is to establish a reliable video-processing and object-detection pipeline before attempting higher-level incident recognition.

As development progresses, this section will document completed features, test results, known limitations, and future improvements.

## 🌟 Long-Term Vision

The long-term goal of ARGUS is to explore how AI systems can move from recognizing individual objects to interpreting sequences of events and assisting people in responding to potential safety incidents.

Rather than relying on a single model or prediction, ARGUS aims to investigate a modular, measurable, and privacy-conscious approach to situational awareness.

## 🤝 Contributions & Feedback

Suggestions, research references, and technical feedback are welcome.

Potential areas for exploration include object tracking, action recognition, temporal reasoning, edge AI, and reliable incident-alert systems.

---

**ARGUS — Autonomous Real-time Guardian for Unusual Situations**

*Built to explore a more intelligent approach to situational awareness.*
