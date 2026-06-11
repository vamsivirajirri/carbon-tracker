# Project Case Study: Engineering CarbonSense with AI Collaboration

## 1. Problem Statement
Many carbon calculators are overly complex, requiring extensive user sign-ups and heavy database configurations that increase latency. The goal was to engineer an intuitive, lightning-fast environmental impact estimator that dynamically surfaces standard EPA calculations right in the client's browser.

## 2. Prompt Engineering Strategy
To construct this production-grade, single-file template, I utilized a structured structural layout prompt methodology:

* **UI/UX Prompting:** Instructed the generation engine to construct a dashboard utilizing Tailwind CSS configured with a dark-theme palette, standard semantic HTML (`<main>`, `<section>`, `<header>`), and embedded SVG graphical indicators.
* **Logic Constraints:** Enforced functional encapsulation where input elements are bidirectionally tied to custom graphical range sliders with native exception-handling wrappers (`validateInput`) to shield computations from invalid data.

## 3. Mathematical Framework & Solution Architecture
The single-file architecture relies on content-delivered engines (Tailwind CSS and Chart.js CDNs) to process environmental math directly via client-side JavaScript:

* **Driving:** Daily Miles × 0.404 kg CO2
* **Electricity:** (Monthly kWh ÷ 30) × 0.371 kg CO2
* **Meat Consumption:** Daily Servings × 2.100 kg CO2

The script converts the cumulative daily data into standard annual metric tons (Daily kg × 365 ÷ 1000). It maps these directly into equivalence indicators (offset trees and international flight segments) while executing real-time data updates on a Chart.js canvas.
