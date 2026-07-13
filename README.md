# CredShield

An institutional, enterprise-grade fintech user interface designed for high-performance portfolio risk management and loan underwriting diagnostics. This interactive mockup implements a clean, data-dense layout using **Tailwind CSS** and **Lucide Vector Icons**.

---

## 📈 Features Included in this Prototype

*   **Premium Fintech Layout:** A high-contrast, minimal color palette featuring deep charcoal backgrounds for navigation elements and vivid emerald green identifiers, inspired by modern software from Stripe, CRED, and top-tier financial institutions.
*   **Live Metrics Display Matrix:** Clean KPI components tracking critical indicators including Active Capital Books, Average Bureau Variance, and System Delinquencies.
*   **Reactive AI Inference Console:** A fully functional client-side form that calculates and presents algorithmic outputs (Probability of Default, Exposure Classifications, and Underwriting Directives) based on dynamic user adjustments.
*   **Real-time Risk Queue:** A robust table showcasing priority accounts with varying severity tiers (`CRITICAL`, `ELEVATED`, `STABLE_WARN`).

---

## 🚀 Quick Start Guide

This frontend mockup is built as a single, decoupled file containing all structure, styling framework components, and interactivity scripts. No build systems or terminal configurations are required to run it.

1. **Save the File:** Copy the provided code asset block and save it to your local environment as `index.html`.
2. **Execute Interactive View:** Double-click the file or right-click and open it inside any modern web browser (Chrome, Edge, Safari, Firefox).

---

## 🕹️ Testing the Interface Interactivity

To observe how the interface handles data rendering state changes without an active Python API connection:
1. Locate the **AI Risk Prediction Console** panel on the left side of the screen.
2. Alter the values in the **Bureau FICO Score** and **Delinquent EMIs** input elements (e.g., lower the score to `580` or increase the delinquencies to `4`).
3. Press **Execute Diagnostic Evaluation**.
4. The dashboard will instantly update its right column workspace view using a simulated mathematical risk weighting formula, shifting color spaces and directives dynamically based on your inputs.

---

## 📂 Production Core Upgrades Roadmap

When you are ready to transition this static prototype to the production-ready Next.js 15 app router architecture:
* **Component Splitting:** Refactor the sidebar navigation and layout tracking bars into standalone React layouts (`/app/layout.tsx`).
* **State Integration:** Swap out the plain JavaScript event handling functions for React hooks (`useState`, `useActionState`).
* **API Hookups:** Update the form submission event to trigger an asynchronous `fetch()` query pointing directly at your Dockerized FastAPI server endpoint (`/api/v1/predict`).
