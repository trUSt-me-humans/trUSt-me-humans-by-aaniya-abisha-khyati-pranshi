# trUSt-me-humans-by-aaniya-abisha-khyati-pranshi

### Transparent, Accountable & Community-Verified Civic Governance

TrUSt me humans is a civic technology platform designed to make local issue reporting more **transparent, verifiable, and accountable**.

Citizens can report civic problems such as potholes, water leaks, sanitation issues, streetlight failures, drainage problems, and safety concerns. Each report receives a unique civic ID and is tracked through a transparent timeline from reporting to resolution.

The platform combines **community verification, AI-assisted classification, evidence-based resolution, and tamper-evident audit trails** to build trust between citizens and civic stakeholders.

## 🚀 Key Features

### 1. Civic Heatmap

* Interactive map of civic issues across India.
* Displays issue hotspots and severity levels.
* Supports categories such as roads, water, sanitation, lighting, drainage, and safety.
* Helps identify areas with recurring civic problems.

### 2. Civic Issue Reporting

Citizens can submit:

* Issue title
* Category
* Description
* Location
* Priority
* Supporting evidence

Each report receives a unique **Civic ID**.

### 3. Trust Score

The platform provides a trust-oriented view based on factors such as:

* Verified reports
* Completed audits
* Resolution transparency
* Community confirmations
* Evidence quality

This helps users understand how reliable and transparent a civic record is.

### 4. Immutable Audit Trail

Every important action is recorded in a chronological timeline.

Examples:

* Citizen report submitted
* AI classification completed
* Department assigned
* Action initiated
* Evidence uploaded
* Community verification

Timeline events are linked using cryptographic hashes, making unauthorized modification easier to detect.

### 5. Proof-of-Resolution

A resolution is supported with evidence rather than simply changing the status to "Resolved."

The system can record:

* Before evidence
* After evidence
* Evidence hash
* Evidence quality score
* Location verification
* Timestamp verification
* Citizen verification

### 6. Community Verification

Nearby citizens can verify civic reports and resolutions.

Community verification increases confidence in the authenticity of an issue and its resolution.

### 7. Resolution Challenges

Citizens can challenge a resolution if they believe an issue has not actually been solved.

A challenge is appended to the civic timeline rather than replacing previous records.

### 8. Ghost Resolution Detection

The system identifies potentially suspicious resolution patterns, such as repeated resolutions and reopenings.

These records can be flagged for further review.

### 9. Network Status

The dashboard provides visibility into:

* Core network
* API status
* Database status
* Map service

This demonstrates system health and operational transparency.

## 🏗️ Technology Stack

### Frontend

* React
* TypeScript
* Vite
* Tailwind CSS
* Radix UI / shadcn-style components
* Lucide React
* Recharts
* Framer Motion

### Backend

* Node.js
* Express
* TypeScript
* tRPC
* Zod

### Database

* MySQL
* Drizzle ORM
* Drizzle Kit

### Mapping

* Google Maps JavaScript API
* Google Maps Marker
* Places
* Geocoding
* Geometry

### Security & Integrity

* OAuth authentication
* JWT/session management
* Secure cookies
* SHA-256 hashing
* Chained timeline hashes
* Pseudonymous citizen identifiers

## 🔄 System Architecture

```text
Citizen
   │
   ▼
React + TypeScript Frontend
   │
   ▼
tRPC API
   │
   ▼
Express + Node.js Backend
   │
   ├── Issue Management
   ├── Verification
   ├── Resolution Challenges
   ├── Proof-of-Resolution
   └── Audit Timeline
   │
   ▼
MySQL + Drizzle ORM
   │
   ▼
Tamper-Evident Civic Records
```

Google Maps provides the interactive geographic visualization layer.

## 🔐 Data Integrity

TrUSt me humans uses cryptographic hashing to create tamper-evident records.

Each timeline event contains:

* Event information
* Current event hash
* Previous event hash
* Timestamp
* Actor information

This creates a chain of events where modifying an earlier record would affect the integrity of subsequent hashes.

Personal information is kept separate from the public-facing civic record wherever possible.

## 📊 Civic Issue Lifecycle

```text
Report Issue
     ↓
Generate Civic ID
     ↓
AI / Category Classification
     ↓
Priority Assessment
     ↓
Department Assignment
     ↓
Action Initiated
     ↓
Proof of Resolution
     ↓
Community Verification
     ↓
Resolved / Disputed / Reopened
```

## 🎯 Problem We Address

Civic complaints often suffer from:

* Lack of transparency
* Limited visibility into complaint progress
* Unclear responsibility
* Weak verification of resolutions
* Repeated or unresolved issues
* Difficulty identifying recurring local problems

TrUSt me humans addresses these gaps by creating a transparent digital trail for civic issues.

## 🌍 Vision

Our vision is to create a civic ecosystem where:

**Every report is traceable.
Every action is accountable.
Every resolution has evidence.
Every citizen can verify.**

The goal is not simply to collect complaints, but to create **trust between communities, institutions, and civic stakeholders**.

## 🧪 Project Status

This project is a working prototype developed for hackathon/demo purposes.

Some dashboard metrics and civic heatmap entries are currently demonstration data, while the core reporting, timeline, verification, challenge, and proof-of-resolution workflows are implemented through the application backend.

## 🛠️ Getting Started

### Prerequisites

* Node.js
* pnpm
* MySQL database

### Installation

```bash
git clone <repository-url>
cd civic-ledger
pnpm install
```

Configure the required environment variables, including the database connection and application/API configuration.

### Development

```bash
pnpm dev
```

### Production Build

```bash
pnpm build
pnpm start
```

### Type Checking

```bash
pnpm check
```

### Tests

```bash
pnpm test
```

### Database Migration

```bash
pnpm db:push
```

## 📁 Project Structure

```text
client/
 └── src/
     ├── components/
     ├── pages/
     ├── hooks/
     ├── contexts/
     └── lib/

server/
 ├── _core/
 ├── db.ts
 ├── routers.ts
 └── storage.ts

drizzle/
 ├── schema.ts
 └── migrations/

shared/
 ├── const.ts
 └── types.ts
```

## 🤝 Core Concept

TrUSt me humans brings together:

**Citizens + Evidence + Verification + Transparency + Technology**

to create a more accountable civic issue-resolution ecosystem.

## 📜 License

This project is licensed under the MIT License.
