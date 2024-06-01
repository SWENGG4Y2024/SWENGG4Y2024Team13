## Table of Contents

1. [Introduction](#1-introduction)
   1. [Purpose](#11-purpose)
   2. [Scope](#12-scope)
   3. [Definitions, Acronyms, and Abbreviations](#13-definitions-acronyms-and-abbreviations)
2. [Functional Requirements](#2-functional-requirements)
   1. [Onboarding](#21-onboarding)
   2. [Homepage](#22-homepage)
   3. [Chat Room](#23-chat-room)
   4. [Calendar](#24-calendar)
   5. [Journal](#25-journal)
   6. [Insights and Recommendations](#26-insights-and-recommendations)
   7. [Autopilot Farming](#27-autopilot-farming)
3. [Cross Reference Matrix](#3-cross-reference-matrix)
4. [Non-Functional Requirements (NFRs)](#4-non-functional-requirements-nfrs)
   1. [Performance](#41-performance)
   2. [Reliability](#42-reliability)
   3. [Usability](#43-usability)
   4. [Security](#44-security)
   5. [Scalability](#45-scalability)
   6. [Data Quality and Volume](#46-data-quality-and-volume)
5. [Constraints](#5-constraints)
6. [Appendices](#6-appendices)
   1. [Appendix A: Glossary](#appendix-a-glossary)
   2. [Appendix B: References](#appendix-b-references)


# Software Requirements Specification (SRS) Document

## 1. Introduction

The agriculture dashboard application aims to provide farmers with a user-friendly and robust tool to manage their crop cultivation activities efficiently. Considering that farmers may often have dirty hands while using the app and may operate it outdoors, the UI design will prioritize well-placed buttons and a color scheme optimized for outdoor visibility. This document outlines the requirements for the development of the agriculture dashboard application.

### 1.1 Purpose

The purpose of this document is to define the functional and non-functional requirements of the agriculture dashboard application, keeping in mind the unique needs and environments of farmers. It serves as a guide for the development team and stakeholders to understand the scope and objectives of the project.

### 1.2 Scope

The agriculture dashboard application will include the following key features:
- Onboarding with language preferences and crop selection.
- Homepage with weather information, market prices, reminders, and crop-specific developments.
- Chat room for farmers, calendar for task management, journal for data logging, insights and recommendations, and autopilot farming for automation.

### 1.3 Definitions, Acronyms, and Abbreviations

- SRS: Software Requirements Specification
- NFRs: Non-Functional Requirements
- UI: User Interface
- IoT: Internet of Things

## 2. Functional Requirements

### 2.1 Onboarding
1. Farmer must be able to easily navigate the onboarding process, with large and clearly labeled buttons for selecting language preferences and crop types.
2. Input fields for crop size shall be designed with larger touch targets to accommodate farmers with dirty hands.
3. Get immideate information from farmer's locale and set languages straight away based on location.
4. Have a app walk-through for all new farmers to ensure they are able to navigate and use features in the app effectively.
5. Agriculture researches may also use this application for their experiments on different genetically modified crop. 

### 2.2 Homepage
1. The homepage shall feature prominently displayed weather information and market prices, with high contrast color themes for outdoor visibility.
2. Buttons for todos and reminders shall be strategically placed for easy access, even with dirty hands.

### 2.3 Chat Room
1. The chat room interface shall prioritize legibility and ease of use, with well-spaced text and intuitive navigation.
2. The chat room feature shall have minimal loading times to ensure real-time communication among farmers.

### 2.4 Calendar
1. The calendar shall have a clean and uncluttered layout, with color-coded task categories for easy identification outdoors.
2. Task management buttons shall be placed at the bottom of the screen for easy access while holding a mobile device with dirty hands.

### 2.5 Journal
1. The journal interface shall be designed with large input fields and buttons for easy data entry, even with gloves or dirty hands.
2. Data logging shall be seamless and intuitive, allowing farmers to quickly record daily activities such as rainfall and fertilizer amounts.

### 2.6 Insights and Recommendations
1. The insights and recommendations feature shall present information in a visually appealing format, with charts and graphs optimized for outdoor viewing.
2. Recommendations shall be actionable and tailored to the specific needs of each farmer, taking into account crop type and environmental factors.
3. The insights should be easily understandable and translated keeping the context and meaning intact in all languages to ensure effective communication to farmers.

### 2.7 Autopilot Farming
1. The autopilot farming feature shall have a user-friendly setup process, with clear instructions and minimal manual input required.
2. Automation controls shall be easily accessible from the homepage, allowing farmers to monitor and adjust settings on the go.
3. The autopilot farming assistant must inform the farmer the action/decision that it will take via email notification or WhatsApp message. Only after the user
4. responds the assistant can go ahead with the decision to change farming parameters by communicating with the IoT devices

## 3. Cross-Reference Matrix

| Requirement              | Farmers | Agricultural Experts | Regulatory Authorities | Developers |
|--------------------------|---------|----------------------|------------------------|------------|
| 2.1 Onboarding           |    X    |                      |                        |      X     |
| 2.2 Homepage             |    X    |                      |                        |      X     |
| 2.3 Chat Room            |    X    |                      |                        |      X     |
| 2.4 Calendar             |    X    |                      |                        |      X     |
| 2.5 Journal              |    X    |                      |                        |      X     |
| 2.6 Insights and Recommendations |    X    |          X           |                        |      X     |
| 2.7 Autopilot Farming    |    X    |          X           |                        |      X     |
| 3.1 Performance          |    X    |                      |                        |      X     |
| 3.2 Reliability          |    X    |          X           |                        |      X     |
| 3.3 Usability            |    X    |          X           |                        |      X     |
| 3.4 Security             |    X    |          X           |            X           |      X     |
| 3.5 Scalability          |    X    |          X           |                        |      X     |
| 3.6 Data Quality and Volume |    X    |          X           |                        |      X     |


## 4. Non-Functional Requirements (NFRs)

### 4.1 Performance
1. The application shall respond to user interactions within 2 seconds, even under poor network conditions.
2. Chat room messages shall be delivered in real-time with minimal latency, ensuring seamless communication among farmers.

### 4.2 Reliability
1. The application shall have an uptime of at least 99%, with regular maintenance and updates to minimize downtime.
2. Data loss shall be minimized through automatic backups and synchronization with cloud storage.
3. The language must be simple and understandable as the major target audience are farmers and they may not have had access to scientific agricultural education.

### 4.3 Usability
1. The UI must be intuitive and easy to navigate, with clear visual cues and minimal text-based instructions.
2. User interactions shall be optimized for touch screens, with large touch targets and gesture-based controls.
3. Have many tootips to ensure user never feels helpless and can always find out what each feature does.

### 4.4 Security
1. User data shall be encrypted both in transit and at rest, with strict access controls to protect sensitive information.
2. The application shall undergo regular security audits and penetration testing to identify and address potential vulnerabilities.

### 4.5 Scalability
1. The application shall support a growing user base without compromising performance, with scalable infrastructure and load balancing capabilities.
2. Backend systems shall be designed to handle large volumes of data and user requests, with horizontal scaling options for future expansion.

### 4.6 Data Quality and Volume
1. The application shall require good quality and large volumes of data to ensure accuracy and reliability in machine learning models used for autopilot farming and disease detection.
2. Data collection mechanisms shall be designed to capture a wide range of environmental and agronomic variables, ensuring robustness and generalizability of predictive models.

## 5. Constraints

- The application shall be compatible with modern web browsers (Chrome, Firefox, Safari) and mobile devices running iOS and Android operating systems.
- Development shall adhere to budget and time constraints specified by stakeholders.

## 6. Appendices

### Appendix A: Glossary
- Dashboard: The main interface of the application displaying relevant information and features.
- Journal: A section where users log daily activities and observations related to crop cultivation.

### Appendix B: References
- SWEBOK (Software Engineering Body of Knowledge)
- Lab Guides on Software Requirements Specification
