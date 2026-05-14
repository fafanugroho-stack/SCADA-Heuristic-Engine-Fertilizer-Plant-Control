# SCADA-Heuristic-Engine-Fertilizer-Plant-Control
Practical, straight to the code, showing an understanding of software development lifecycle and AI evolution.
Overview
A lightweight, serverless SCADA (Supervisory Control And Data Acquisition) web app built to solve a critical operational bottleneck in a fertilizer granulation plant: a 2-hour data latency between physical processing and quality control.

This project bridges the gap between manufacturing constraints and digital system architecture, providing a real-time digital Poka-Yoke for shop-floor operators.
<img width="1366" height="720" alt="image" src="https://github.com/user-attachments/assets/20e77bf9-1277-42cd-a718-93fb12316e37" />
🏗️ System Architecture
Backend: Serverless API via Google Apps Script (V8 Engine).

Database: Google Sheets configured as a lightweight RDBMS.

Frontend UI: Bootstrap 5.3, HTML5, custom CSS for dynamic alerting.

Data Visualization: Chart.js for real-time thermodynamic correlation tracking.

🧠 Core Logic: Rule-Based Heuristic Engine
To provide immediate operational value, the core warning engine utilizes a Rule-Based Heuristic approach.

How it works: The logic parses real-time telemetry (e.g., Ambient Humidity, Feeding Speed, Rotary Dryer Temp) and evaluates them against strict, heuristically determined thresholds derived from historical data (2023-2025).

Actionable Alerts: If boundaries are breached, the frontend dynamically manipulates the DOM (e.g., toggling .blink-danger CSS classes) and outputs explicit adjustment commands for the operators.

🚀 Future Roadmap: Statistical Predictive Modeling
The current heuristic engine is highly modular by design. The architectural roadmap involves scaling this logic layer by integrating advanced Statistical Analysis and Machine Learning algorithms to refine the predictive accuracy of product moisture and hardness based on continuous, real-time data ingestion.
