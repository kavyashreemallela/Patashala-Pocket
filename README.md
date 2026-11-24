# Pathshala Pocket

**Track:** Mystery Track — UnlockED: Low-Bandwidth Adaptive Learning for Rural Schools  
**Project stage:** Round 1 blueprint only  
**Team:** Add your team name here

## Project summary

Pathshala Pocket is a proposed offline-first learning companion for rural and remote classrooms. Teachers prepare a short lesson pack for a grade, topic, and language. Students download it while connected, study and practice offline, and sync their progress for the teacher when connectivity returns.

## Problem

Students and teachers in rural and remote schools may not be able to rely on continuous internet access for digital learning. Multi-grade classrooms can also require teachers to support students working at different levels.

## Proposed solution

Pathshala Pocket combines downloadable, low-data lesson packs, short practice activities that respond to learner answers using simple rules, local progress storage, and a teacher view of completed work and topics to revisit.

## Planned hack-day MVP

- One grade, one topic, and one regional language
- One downloadable lesson pack
- A short, rule-based adaptive quiz
- Progress saved on the device while offline
- A basic teacher dashboard showing completion and topics to revisit

This is a proposed hack-day scope. No code or prototype has been developed for this submission phase.

## Proposed technical architecture

- **Frontend:** React + TypeScript progressive web app
- **Offline use:** Service Worker and Cache API for app resources; IndexedDB for lesson packs and unsynced progress
- **Cloud services:** AWS Amplify Hosting, Amazon Cognito for teacher sign-in, AWS AppSync for the data API, Amazon DynamoDB for class and progress records, and Amazon S3 for lesson packs and optional audio
- **Adaptive practice:** Simple on-device rules for the MVP; no AI model is required for basic offline practice

Offline storage and cloud synchronization are proposed behaviors. Sync logic would need to be implemented during the hack day.

## Impact measures to validate in a pilot

- Lesson and quiz completion
- Topic-level quiz progress
- Whether offline work syncs successfully when connectivity returns
- Whether teachers find the progress view useful for identifying topics to revisit

These are proposed pilot measures, not achieved results.

## Business model hypothesis

A proposed B2B2C social-impact model: students and teachers use the service, while schools, education departments, NGOs, or CSR programs fund pilots or institutional access. Basic student access would remain free. The payer, price, and ongoing costs need validation.

## Concept visuals

- `diagrams/process-flow.svg` — lesson preparation, offline learning, and progress sync
- `diagrams/architecture.svg` — proposed device and AWS architecture
- `diagrams/teacher-dashboard-concept.svg` — static dashboard mockup; all displayed sample figures are illustrative
- `diagrams/impact-measure-scale.svg` — proposed pilot, measurement, and expansion path
- `diagrams/solution-flow.svg` — download, practice, adapt, and sync sequence

## Phase note

This repository contains planning documents and static concept visuals only. It intentionally contains no source code, working prototype, real student data, credentials, or API keys. The presentation is submitted separately through the team's Google Drive link.
