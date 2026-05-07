

# Blood Bank App
Libyan Blood Bank 
Minimum Viable Product (MVP) Documentation
NOUR MOHAMED ALMASHAEK

Mission Statement: To provide a decentralized, privacy-first mobile platform that bridges the critical gap between
emergency blood shortages in Libyan medical facilities and willing, eligible local donors.


1. Executive Summary
The application is a dual-interface mobile platform designed to connect medical clinics with blood donors in real-time. By
utilizing localized alerts and automated eligibility screening, the platform dramatically reduces the time it takes to source
specific blood types during emergencies.
The system is designed with a strict "Zero Patient Data" architecture, ensuring
complete privacy and compliance by only broadcasting the required blood type and urgency, rather than patient details.

3. Platform Architecture & User Roles
The application routes users into two distinct portals upon launch:
● Blood Donor Portal: For individuals registering to donate blood, tracking their eligibility, and responding to localized
emergencies.
● Medical Clinic Portal: A restricted-access dashboard for verified medical centers and blood banks to broadcast urgent
needs to the donor network.

4. Core Features: Blood Donor Flow

3.1. Registration & Automated Screening

● Profile Creation: Captures essential contact logistics (Phone, Email), Location (Tripoli, Benghazi, Misrata, Zawia), and
precise Blood Type.

● Dynamic Health Check: An automated, in-app questionnaire verifying age requirements (18-65) and screening for
disqualifying conditions (e.g., Hepatitis, active cancer, recent malaria).

● Instant Eligibility Status: Automatically calculates and displays the user's eligibility to donate. If ineligible, the system
gracefully advises the user and prevents donation scheduling.

3.2. Donor Dashboard & Logistics

● Real-Time Emergency Feed: A filterable feed of active blood requests, displaying the requesting clinic, exact location,
urgency level (Critical, Urgent, Moderate), and units needed.

● "I Can Donate" Action: One-tap response that provides the donor with the clinic's direct contact number and map
routing.

● Facilities Directory: A searchable index of active Blood Centers across Libya, displaying their operating hours and
current blood inventory status.

● Donation History: Automatically logs past donations and calculates the safe waiting period before the next eligible
donation.


5. Core Features: Medical Clinic Flow

4.1. Verified Onboarding

● Licensing Verification: Clinics must provide their Ministry of Health (MOH) License Number and official address during
registration, ensuring only legitimate facilities can broadcast alerts.

4.2. Clinic Management Portal

● Analytics Dashboard: Displays real-time metrics on Active, Fulfilled, and Total blood requests to help clinics manage
their supply chain.

● Emergency Broadcast System: A streamlined form allowing staff to instantly alert local donors. Inputs include required
Blood Type, Urgency Level, Number of Units, and specific logistical notes.

● Targeted Push Notifications: The system automatically routes the broadcast only to registered donors in the exact city
who possess the matching blood type, preventing alert fatigue.


6. Technical & Security Posture

●Framework: Built on React Native (optimized for cross-platform iOS and Android deployment via Expo).

● Privacy-First Design: Does not collect, store, or transmit any Protected Health Information (PHI) regarding the blood
recipients. The connection relies solely on logistical routing and blood type matching.

7. Demonstration & Deployment Strategy
The MVP is currently stabilized in a staging environment. It can be immediately demonstrated to stakeholders at the
Central Blood Bank using Expo Go, allowing them to test both the Clinic broadcast trigger and the resulting Donor push
notification in real-time without requiring app store installation.

Watch a demo video of the app:

<div align="center">
  <a href="https://www.youtube.com/shorts/wLcxh0_ZQn4">
    <img src="https://img.youtube.com/vi/wLcxh0_ZQn4/0.jpg" alt="Libyan Blood Bank App Demo" />
  </a>
</div>
