<div align="center">

<img src="./assets/backend-profile-banner.svg" alt="Kiarash Delavar - Backend development, APIs and cloud systems" width="100%" />

**Software Engineering Student · Backend Developer**

[Print.com](https://www.print.com/) intern · Saxion University of Applied Sciences · Deventer, Netherlands

<a href="https://www.kiarashdelavar.com/"><img src="https://img.shields.io/badge/Portfolio-0F766E?style=for-the-badge" alt="Portfolio" /></a>
<a href="https://www.linkedin.com/in/kiarash-delavar/"><img src="https://img.shields.io/badge/LinkedIn-1E293B?style=for-the-badge" alt="LinkedIn" /></a>
<a href="mailto:kiarash.delavar@gmail.com"><img src="https://img.shields.io/badge/Email-1E293B?style=for-the-badge" alt="Email Kiarash" /></a>
<a href="https://leetcode.com/u/KiarashDelavar/"><img src="https://img.shields.io/badge/LeetCode-1E293B?style=for-the-badge&logo=leetcode&logoColor=F5B841" alt="LeetCode" /></a>

[Experience](#currently-building) · [Projects](#selected-projects) · [Tech](#tech-i-work-with) · [Languages](#languages) · [Opportunities](#lets-talk)

</div>

---

At Print.com, I'm working on the backend between a customer reviewing a print proof and an order moving into production. That's the kind of problem I enjoy: connecting **APIs, data, and business rules** to make a real workflow work.

I'm a third-year Software Engineering student at Saxion, with expected graduation in **July 2028**. My projects have taken me from print workflows to cycling analysis, robotics, and energy simulation. Across them, I like understanding both the system and the people who will use it.

## Currently building

### Print.com · Digital Proof
**Software Engineering Intern · Bricks backend team**

Developing the workflow for reviewing and approving proof files before print production:

- **APIs and data:** proof files, versions, customer decisions, and approval history.
- **Cloud services:** serverless backend functions and file uploads using S3 presigned URLs.
- **Business logic:** connecting approval decisions to order status and production workflows, including Go rule-engine logic.

`TypeScript` `Node.js` `AWS Lambda` `Amazon S3` `MySQL` `Go`

### Track Cycling Start Analysis · Saxion / NOC*NSF research
**Computer Vision & Software Developer · Sports Biomechanics & Performance Analysis**

Developing a Python desktop application that transforms track-cycling videos into measurable biomechanics and sprint-start performance data. The goal is to give researchers and coaches useful information about rider posture, movement, and acceleration through **pose estimation, cyclist tracking, joint-angle calculations, and synchronized video analysis**.

The project combines computer vision, tracking algorithms, scientific data processing, and cross-platform desktop software.

**Implemented so far**

- **Pose estimation and biomechanics:** Built video-analysis pipelines using MMPose and OpenCV to extract cyclist landmarks, calculate joint angles, and display skeleton overlays.
- **Start-performance metrics:** Developed plots for pelvis movement, velocity, acceleration, joint angles, and measurements aligned with events such as the starting gun.
- **Cyclist tracking:** Implemented rider tracking and investigated multi-person approaches such as BoT-SORT and person re-identification (Re-ID) to address identity switching when cyclists overlap or leave the frame.
- **Desktop application:** Created a PySide6 interface with video playback, pose overlays, interactive Plotly graphs, analysis results, and quality-check views.
- **Persistent research sessions:** Added local SQLite storage with unique session IDs, frame timestamps, tracking states, detected landmarks, confidence data, and save/reopen support.
- **Research exports:** Implemented CSV, XLSX, PDF, dataset-folder, and ZIP exports for further analysis and data sharing.
- **Desktop distribution:** Produced Windows and macOS builds to let researchers use the application without setting up a Python development environment.

**Current engineering improvements**

- Strengthening primary-rider identity locking so pose tracking does not jump to another cyclist when the target exits the camera view.
- Moving toward frame-by-frame analysis across the entire video, with explicit tracking states for frames where no reliable pose is available.
- Evaluating selectable pose-estimation models, balancing fast exploratory processing against higher-accuracy research analysis.
- Improving velocity and acceleration handling, confidence-aware visualizations, and consistency between application charts and exported reports.
- Developing wheel-size and pixel-to-real-world calibration methods for physically meaningful speed estimates.
- Hardening session persistence, export integrity, and reproducible analysis workflows.

**Upcoming camera research and development**

- **Live camera capture:** Explore webcam and USB-camera integration with manual start/stop recording for trackside sessions.
- **Camera placement and feedback:** Work with VU Amsterdam Human Movement Sciences students on practical camera positions, mounting, recording quality, and tripod-camera-to-TV feedback workflows.
- **Pose validation:** Evaluate how camera position, angle, and recording conditions affect detected landmarks and calculated joint angles.
- **Speed validation:** Compare speed inferred from tracked motion and wheel rotation with independent reference measurements; investigate wheel geometry and calibration uncertainty.
- **Recording metadata:** Add structured camera, calibration, and bicycle information to support repeatable sessions and comparisons.
- **Coach-oriented usability:** Refine the capture-to-analysis experience so useful sprint-start metrics and graphs can be reviewed quickly after a run.

**Long-term goal:** build a reliable, validated research and coaching tool that connects video-based measurements with practical feedback for track-cycling sprint starts.

`Python` `MMPose` `OpenCV` `PySide6` `Plotly` `SQLite` `Pose Estimation` `Multi-Object Tracking` `Biomechanics`

Alongside these projects, I'm building **Python/FastAPI services and a React dashboard for Esports Team Twente**, and improving an educational microgrid simulator with **Saxion Sustainable Energy Systems**.

## Selected projects

<table>
<tr>
<td width="50%" valign="top">
<h3>01 · DEMKit Microgrid Simulator</h3>
<p><strong>Making energy simulation easier to use in a classroom.</strong></p>
<p>Building on an existing DEMKit-based touchtable simulator. My focus is setup, startup reliability, and usability so students can explore solar power, batteries, EVs, and grid limits.</p>
<p><code>Python</code> <code>Node.js</code> <code>JavaScript</code></p>
<p><a href="https://github.com/kiarashdelavar/demkit-microgrid-simulator"><strong>Explore the repository →</strong></a></p>
</td>
<td width="50%" valign="top">
<h3>02 · Track Cycling Start Analysis</h3>
<p><strong>Computer vision and biomechanical analysis for sprint-cycling research.</strong></p>
<p>Developing a cross-platform Python desktop application for cyclist tracking, pose estimation, joint-angle measurements, and sprint-start analysis. Built with PySide6, MMPose, OpenCV, Plotly, and SQLite, including saved research sessions and multiple export formats. Current work focuses on tracking reliability and wheel calibration; planned studies include camera positioning, live capture, and speed validation with academic partners.</p>
<p><code>Python</code> <code>MMPose</code> <code>OpenCV</code> <code>PySide6</code> <code>SQLite</code></p>
<p><a href="https://www.linkedin.com/pulse/hard-part-wasnt-computer-vision-building-tool-coaches-kiarash-delavar-sy94e/"><strong>Read the project story →</strong></a></p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<h3>03 · Conference Room Booking</h3>
<p><strong>Coordinating bookings across independent processes.</strong></p>
<p>A Java coursework project where clients, rental agents, and buildings communicate through RabbitMQ queues and exchanges. Supports reservations, confirmations, cancellations, and multiple rental agents.</p>
<p><code>Java</code> <code>RabbitMQ</code> <code>AMQP</code> <code>Maven</code></p>
<p><a href="https://github.com/kiarashdelavar/ConferenceRent-RabbitMQ"><strong>Explore the repository →</strong></a></p>
</td>
<td width="50%" valign="top">
<h3>04 · IoT Telemetry Platform</h3>
<p><strong>Connecting sample sensor data to an API and dashboard.</strong></p>
<p>A prototype that generates simulated telemetry, stores readings in PostgreSQL, and exposes telemetry and history endpoints to a Next.js dashboard. Includes a simple temperature-trend flag and Docker configuration.</p>
<p><code>FastAPI</code> <code>PostgreSQL</code> <code>Next.js</code> <code>Docker</code></p>
<p><a href="https://github.com/kiarashdelavar/iot-telemetry-platform"><strong>Explore the repository →</strong></a></p>
</td>
</tr>
</table>

**Also built with a team:** [Frog Autonomous Navigation System](https://github.com/kiarashdelavar/Frog-Autonomous-Navigation-System) - a Java application that uses radar input to guide a simulated robot around obstacles and records mission data in SQLite.

## Tech I work with

My current work centres on **TypeScript, Python, backend APIs, SQL, and AWS**.

| Area | Technologies |
| :--- | :--- |
| **Programming** | TypeScript · JavaScript · Python · Go · Java · C++ · SQL |
| **Backend & messaging** | Node.js · FastAPI · Spring Boot · REST APIs · TypeORM · RabbitMQ |
| **Databases** | MySQL · PostgreSQL · DynamoDB · SQLite |
| **Cloud & delivery** | AWS Lambda · Amazon S3 · Docker · Git · GitHub Actions |
| **Testing & API tools** | Jest · Postman |
| **Interfaces** | React · Next.js · PySide6 |
| **Research & robotics** | Computer vision · MMPose · OpenCV · MediaPipe · ROS 2 · MoveIt 2 |

## Languages

| Language | Level |
| :--- | :--- |
| **Persian / فارسی** | Native |
| **English** | C1 - Advanced |
| **Dutch / Nederlands** | B1 - Intermediate; still learning Dutch |

## Beyond the code

Registered for the **[ProRail Data Challenge 2026](https://www.prorail.nl/evenementen-overzicht/data-challenge-2026)** · **4 November - 2 December 2026**. The challenge explores sensor and incident data from the Best railway tunnel to identify patterns that could support proactive maintenance.

## Let's talk

I'm interested in **full-time Junior Software Engineer roles, especially backend development**. I'm also open to **part-time student developer positions** and **Software Engineering internships starting in February 2027**.

If your team works on APIs, data, cloud services, or software that supports everyday operations, I'd like to hear about it.

**[View my portfolio](https://www.kiarashdelavar.com/) · [Connect on LinkedIn](https://www.linkedin.com/in/kiarash-delavar/) · [Email me](mailto:kiarash.delavar@gmail.com)**
