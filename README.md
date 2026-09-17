
# Custodian: Culture on Its Own Terms 🌍✨

> **Culture isn't content. It is community-owned knowledge.**

[![Live Demo](https://img.shields.io/badge/Live-Website-brightgreen?style=for-the-badge&logo=vercel)](https://custodian-chi.vercel.app/)
[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github)](https://github.com/prathvikshettyy/custodian)
[![M# Manipal Hackathon 2026](https://img.shields.io/badge/Manipal-Hackathon_2026-blue?style=for-the-badge)]()
[![Track](https://img.shields.io/badge/Track-Culture_and_Community-orange?style=for-the-badge)]()

---

## 🚀 Overview

Traditional cultural tourism prioritizes visitors, leaving local custodians without control over their stories, access, and financial value. When culture travels without its custodians, meaning and value travel away.

**Custodian** is a custodian-first digital platform designed for discovering, experiencing, and preserving living culture on its own terms. Grounded in the core design principle that **"AI translates culture; it does not invent it,"** the platform ensures that consent, native language preservation, spatial context, and fair value return are embedded directly into every cultural interaction.

---

## 💡 Key Features

* **Custodian-Controlled Consent:** Custodians define what can be seen, shared, or booked. Consent acts as a first-class data layer where scope, audience, reuse rights, and revenue rules travel alongside every story.
* **Native-Language Storytelling:** Custodians record field notes and audio in their native regional dialects, preserving their authentic voice rather than providing a diluted summary.
* **AI-Assisted Multilingual Access:** RAG-grounded translation allows travellers to listen and read in their preferred language without eroding local cultural authority.
* **Place-Led Map Discovery:** Interactive spatial discovery introduces genuine relationships and context rather than extracting content.
* **Direct Participation & Monetization:** Experience bookings, craft commissions, and direct support mechanisms return financial value straight to knowledge holders.

---

## 🛠️ Detailed Architecture & Technical Implementation

The platform is engineered around **provenance over performance**, guaranteeing that every answer provided by the system is grounded strictly in custodial content, permissions, and context.

### 🏗️ End-to-End System Architecture

```text
┌────────────────────────────────────────────────────────────────────────┐
│                           USER INTERFACES                              │
│   [ Cultural Custodian ]     [ Traveller ]     [ Institutions / NGOs ] │
└───────────────┬───────────────────┬───────────────────────┬────────────┘
                │                   │                       │
                ▼                   ▼                       ▼
┌────────────────────────────────────────────────────────────────────────┐
│                   FRONTEND (Next.js / React)                           │
│        Multilingual UI | Interactive Maps | Booking | Storytelling     │
└───────────────────────────────────┬────────────────────────────────────┘
                                    │
                                    ▼
┌────────────────────────────────────────────────────────────────────────┐
│                   BACKEND SERVICES (FastAPI / Node.js)                  │
│ ┌──────────────────────┐ ┌───────────────────┐ ┌─────────────────────┐ │
│ │ User / Identity Mgmt │ │  Content & Rules  │ │ Matching & Recomm.  │ │
│ └──────────────────────┘ └───────────────────┘ └─────────────────────┘ │
│ ┌──────────────────────┐ ┌───────────────────┐                         │
│ │ Booking & Payments   │ │  AI / RAG Service │                         │
│ └──────────────────────┘ └───────────────────┘                         │
└───────────┬───────────────────────┬───────────────────────┬────────────┘
            │                       │                       │
            ▼                       ▼                       ▼
┌──────────────────────┐ ┌────────────────────┐ ┌──────────────────────┐
│ POSTGRESQL + PGVECTOR│ │ CLOUD STORAGE (S3) │ │   OPENAI / LLM RAG   │
│ Structured & Vectors │ │ Audio, Photo, Video│ │ Speech-to-Text, Q&A  │
└──────────────────────┘ └────────────────────┘ └──────────────────────┘
