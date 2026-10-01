# Awesome-Deepfake-Detection

## Top Deepfake Detection Platforms Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Synthetic Media Detection, Content Provenance & Real-Time Verification*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Deepfake Detection**. These tools help organizations detect AI-generated and manipulated media—images, video, audio, and text—protecting identity verification, fraud prevention, and content authenticity workflows.



**Examples** include Reality Defender, Sensity AI, Hive, Truepic, DeepMedia, Attestiv, Resemble Detect, Intel FakeCatcher, GetReal Security, and Reality Guard (the category leaders).



**Open-source emphasis**: Deepfake detection has a **small but emerging open-source ecosystem**. **DeMorph** provides a multimodal detection solution with explainable AI (XAI) insights using Grad-CAM . **DeepScan** is a multi-modal web-based system for detecting AI-generated and manipulated media, achieving **94.8% accuracy** on audio detection with RawNet2 . This section documents these focused solutions honestly—the open-source ecosystem remains significantly behind commercial platforms in detection accuracy and production readiness.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Reality Defender](https://www.realitydefender.com/)**  

  **The most comprehensive deepfake detection platform with multi-language SDK support.** Provides SDKs for TypeScript/JavaScript, Python, Go, Rust, and Java . **RealAPI** enables integration in two lines of code with enterprise-grade detection for images, audio, and video . **Key features**: Score normalization to 0-1 range, heatmaps for image scans showing manipulation regions, event-based or polling integration, batch processing, and user feedback recording . Free tier: 50 scans/month; Business: $399/month for 1,000 scans; Enterprise: custom with on-premises, private cloud, or air-gapped deployment .



- **[Sensity AI](https://sensity.ai/)**  

  **Enterprise deepfake detection focused on KYC and live video call protection.** Detects AI-generated faces and voice manipulation in real time, protecting against injection attacks and impersonation . **SDK monitors user sessions** for anomalies (virtual cameras, mobile emulators); **API performs pixel-level analysis** of images and videos with near real-time binary real/fake response . **Microsoft Teams integration** protects video calls with face swap and voice cloning detection . ISO 27001 certified, GDPR compliant .



- **[Hive](https://thehive.ai/)**  

  **AI-generated content detection with source identification.** Single endpoint runs two models: one for detecting AI-generated images (Midjourney, DALL-E, Firefly) and one for deepfake detection . **Source classification** identifies the specific generator used (Sora, Pika, Runway, etc.) . **C2PA metadata extraction** when present . Confidence scores provided for each classification .



- **[Truepic](https://www.truepic.com/)**  

  **First to support C2PA 2.0 for enterprises.** Founded on the Coalition for Content Provenance and Authenticity specification, Truepic provides **secure key generation, certificate issuance, and combined claim generation and signing** . **Content Credentials Display** shows verified origin and traceable edits . The world's first authenticated deepfake video was produced using Truepic's C2PA transparency tools .



- **[DeepMedia](https://deepmedia.ai/)**  

  **Pentagon-contracted deepfake detection for countering information warfare.** Awarded contract to provide "rapid and accurate deepfake detection to counter Russian and Chinese information warfare" . Uses **generative AI and large language models** to analyze synthetic or modified faces and voices across languages, races, ages, and genders .



- **[Attestiv](https://attestiv.com/)**  

  **Forensic media integrity platform with free tier for journalists.** **DeepScan** analyzes images, video, and documents for deepfake indicators, detecting AI-generated or manipulated content even when repackaged as screenshots . **Free starter tier** for journalists, fact-checkers, and media professionals . Enterprise use cases include insurance claims, underwriting, lending, and compliance .



- **[Resemble Detect](https://www.resemble.ai/)**  

  **Real-time deepfake detection for Microsoft Teams and telecom fraud prevention.** **Teams-native experience** as a pinned app—no separate meeting bot required . **Live audio and video analysis** flags suspicious participants during calls . **Identity matching across calls** recognizes enrolled individuals by face and voice, flagging when name doesn't match . **DETECT-3B-Omni** reports **98.3% overall accuracy** with equivalence across content and demographic splits .



- **[Intel FakeCatcher](https://www.intel.com/)**  

  **Biologically-based deepfake detection using remote photoplethysmography (rPPG).** Analyzes **blood flow signals in facial veins** at 32 points on the face—when the heart pumps blood, veins change color imperceptibly but detectably . **96%+ detection accuracy** with real-time capability . The only detection approach based on biological signals rather than artifacts.



- **[GetReal Security](https://www.getrealsecurity.com/)**  

  **First platform combining deepfake detection with continuous identity verification.** Co-founded by **Dr. Hany Farid**, the foremost expert on deepfakes and manipulated media . **GetReal Protect** offers four integrated capabilities: deepfake detection, impersonation detection, continuous identity verification, and global threat intelligence . Integrates with Microsoft Teams, Cisco Webex, Zoom, and voice systems with **40+ native integrations** including Okta, Microsoft Entra, and CyberArk . SOC 2 Type II, GDPR, CCPA/CPRA, and BIPA compliant .



- **[Reality Guard](https://www.realityguard.ai/)**  

  Deepfake detection platform specializing in **video analysis** where face, facial expressions, and lip sync with voice matter . Performs well on video content but has reduced accuracy on landscapes and images without people .



## Open-Source GitHub Projects



### Multimodal Detection Systems



- **[DeMorph](https://github.com/praevalis/demorph)**  

  **Comprehensive open-source deepfake detection solution using multimodal approach.** Analyzes **facial movements, lip synchronization, and audio-visual consistency** for detection . **Explainable AI (XAI) Insights** provides visual explanations using **Grad-CAM** techniques . **Real-time and batch processing** of videos with downloadable reports including authenticity status, detected abnormalities, and confidence scores . **Social link support** for checking media from Twitter trends and YouTube channels . **Tech stack**: Python, TypeScript, FastAPI, React, PyTorch, OpenCV, GradCAM, PostgreSQL .



- **[DeepScan](https://zenodo.org/records/19953053)**  

  **Multi-modal web-based system for detecting AI-generated and manipulated media.** **Image detection**: TensorFlow 2.16 with **XceptionNet** for deepfake image/video detection . **Audio detection**: PyTorch 2 with **RawNet2** for synthetic speech detection . **Results**: **94.8% accuracy**, 93.9% precision, 95.7% recall, **4.54% EER**, **0.989 AUC** on LibriSeVoc audio dataset . **Tech stack**: FastAPI 0.110, React 18, TypeScript, Vite, Tailwind CSS, OpenCV, MTCNN, Librosa, Prometheus . Rate limiting: 5 req/sec, 10 req/min per IP . **Limitations**: Pre-trained models not fine-tuned for specific AI generation tools; requires large labelled datasets and GPU resources for tool-specific training .



### Additional Strong Open-Source Options



- **Multimodal Detection**: **DeMorph** (Grad-CAM explainability, social link support) , **DeepScan** (94.8% audio accuracy, multi-modal) .

- **Tooling Note**: **Deep-Live-Cam** (72.7k GitHub stars) is a **deepfake generation tool**, not detection—included as context for the threat landscape .



**Frameworks for building custom systems**: Combine **DeMorph** for multimodal detection with Grad-CAM explainability, **DeepScan** for image (XceptionNet) and audio (RawNet2) detection pipelines, and **C2PA** open specifications for content provenance. Add **PostgreSQL** for metadata persistence and **Docker** for deployment. **Note**: Open-source detection accuracy significantly trails commercial platforms—expect higher false positive rates and lower generalization to novel generation techniques.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Deepfake detection platforms handle sensitive media and identity data; ensure compliance with privacy regulations, biometric laws (BIPA), and applicable content authenticity standards.

- **Open-source reality**: The open-source ecosystem for deepfake detection is **emerging but significantly behind commercial platforms**. **DeMorph** and **DeepScan** provide functional multimodal detection with published accuracy metrics, but **generalization to novel AI generation techniques, real-time performance at scale, and integration breadth** remain limited compared to Reality Defender, Sensity AI, Hive, and GetReal. Detection is fundamentally an **adversarial arms race**—open-source models trained on public datasets struggle against proprietary generators and adversarial perturbations. The open-source path is most viable for **research, education, or supplementary verification workflows** rather than production-grade enterprise deployment.



---



**Made for security engineers, fraud prevention teams, media forensics analysts, and content authenticity researchers.**

Let's make deepfake detection more open, transparent, and resilient.
