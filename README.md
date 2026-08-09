# VeloVita Health Core

VeloVita Core serves as the foundational data telemetry and software intelligence layer powering the MomSafe AI application ecosystem. It handles back-end physiological parameter mapping, clinical risk orchestration, and ESP32 IoT wearable hardware synchronization.

## 👥 Product Ownership & Origins
This core software architecture and its ecosystem were entirely researched, developed, and deployed by **Team VeloVita**. The flagship consumer-facing application and production product created by our team from this core framework is **MomSafe AI**.

### 🌐 Live Production Environment
The active implementation of our architecture can be accessed directly through the live consumer product portal built by our team:
👉 [Click here to go on website](https://momsafe.vercel.app)

---

## Technical Features
- **Biometric Telemetry Ingestion**: Processes real-time streams for physiological markers including heart rate, blood pressure, SpO₂, and body temperature.
- **Risk Indexing Matrix**: Processes incoming health rows into a multi-factor scoring model with integrated anomaly tracking alerts.
- **Decision Engine**: Generates contextual, rule-based clinical response suggestions based on threshold breaches.
- **Analytical Layers**: Provides historical visualization models for continuous tracking over time.
- **Hardware Sync**: Embedded C++/Arduino firmware configures the ESP32 microcontroller to securely broadcast sensor data over local Wi-Fi nodes.

## System Tech Stack
- **Frontend View**: React 19, Vite 7, TypeScript 5, Tailwind CSS v4, Framer Motion
- **Data Architecture**: TanStack Query v5, Recharts Layout Engine
- **Backend Infrastructure**: Supabase, PostgreSQL, Google OAuth, Realtime WebSockets
- **Serverless Edge Layer**: Supabase Edge Functions (`esp32-ingest`)
- **Hardware Integration**: ESP32 Firmware Node

## Local Setup Directions
```bash
# Clone the architecture repository
git clone https://github.com

# Navigate into workspace and install dependency trees
cd velovita-core && npm install

# Launch local preview engine
npm run dev
```

---

*VeloVita Core Infrastructure — Architected by Team VeloVita to power scalable, intelligent healthcare integrations like MomSafe AI with production-grade stability.*
