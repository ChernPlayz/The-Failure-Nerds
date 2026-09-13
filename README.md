# Travel Planner by The Failure Nerds
Team: Lee Fu Chern, Lee Guan Hong, Law Jin Tao, Joshua Chin Wai Kit  
Problem Statement: Travel Planner  
Video Presentation:  [Unlisted Youtube Link]  
Presentation Slides: [Public Link]  

## 1. Project Overview
**The Problem:**  
Planning a trip currently requires juggling multiple fragmented applications. For example, one for accommodation, another for navigation, separate apps for splitting group expenses, and checking weather forecasts manually. This context-switching leads to decision fatigue, poor budget tracking, and rigid itineraries that break when unexpected events occur such as sudden rain or heavy traffic. 
   
The stakeholders are travelers and group leaders who struggle to coordinate itineraries, track shared funds, and adapt to live changes, budget travelers who need information on affordable stays, public transport, and cheap local dining, and also local merchants and transit operators who benefit from increased discovery of last-minute surplus food, parking lots, and public transit options.  

One of the apps that already exists is Google Maps. It is great point-to-point navigation, but fails as an all-in-one trip planner that manages accommodation booking, group budgets, and interactive travel missions.

**Our Solution:**  
Our app will solve the issue of having to switch between apps and make it into an all-in-one travel hub. It will include real-time weather and traffic rerouting and a shared group expense and bill splitter function.  

## 2. Ideation & Process
### 2.1 Ideas We Considered
|   **Idea**    |  **Why it was dropped / kept** |
| :- | :- |
| All-in-One Search Hub (Hotels, Transport, Budget, Food) | Kept: Solves the core issue of app fragmentation by bringing essential trip tools under one roof. |
| Real-Time Weather Rerouting ("Avoid the Rain") | Kept: Provides the core "Wow" utility by dynamically adjusting itineraries based on sudden weather changes. |
| Shared Group Expense Tracker & Bill Splitter | Kept: Essential for group trips to remove awkward fund tracking and streamline shared balances. |
| Parking Lot Finder | Kept: Addresses real-world micro-frustrations while traveling in unfamiliar locations. |
| Travel Bingo (RPG Mission System) | Dropped: No real planning behind it and we were unsure whether we were going succeed making this through |
| AI Travel Journal / Automatic Vlog Generator | Dropped: High technical complexity and API cost; shifted focus toward real-time utility and core user experience instead. |
| AR Navigation for Historical Landmarks | Dropped: Exceeded building scope and increased mobile battery drain significantly during full-day travel. |

### 2.2 Ideation Boards
a

### 2.3 Mentor Consultation
| Date | Mentor | Feedback Received | What Was Changed|
| :- | :- | :- | :- |
| 7/9/2026 | Teh Ming En | - | How to start our project |
| 11/9/2026 | Daniel Koh Yu  Hang | 1. Stick with the current API if it reliably covers walking, driving, and public transit, as minimizing integration risk takes priority over chasing the "best" API.<br>2. **Prototyping Strategy:** Live routing isn't required for every screen.<br>3. Defer non-essential features that don't address the core travel-planning problem.<br>4. **Backend Requirements:** A backend is unnecessary at this stage. | 1. We stuck to reliable api instead of chasing the best API<br>2. We made representative mock route data is sufficient to demonstrate the concept<br>3. We prioritized polishing the main user experience<br>4. We used mock data to prove the concept, ensuring the mock details accurately reflect the intended core product vision |

## 3. Design & Prototype
**UI Prototype:** 
https://www.figma.com/design/zXgn3436jU2KUtdDpn6tFl/Travel-Planner?node-id=1-2&t=hmOs5VZoQLfiX61W-1

## 4. What Makes It Different

Traditional travel tools are highly fragmented: travelers use **TripAdvisor** to research attractions, **Google Maps** for navigation, **Splitwise** to track expenses, and **WhatsApp/Telegram** to debate itineraries. Our application is a unified, intelligent command center designed for the modern traveler. 

Here are the novel twists that set our platform apart:

*   **Real-Time Weather Optimization (The Rerouting Engine):** Instead of manually replanning when rain or unexpected weather ruins outdoor plans, our application actively monitors forecasts from the **Weather API** and triggers an automatic itinerary adjustment. If there is predicted rain, it instantly swaps outdoor attractions (e.g., temples or parks) with indoor alternatives (e.g., museums, galleries, or indoor dining) within your path.
*   **Intelligent Proximity-Based Discovery (Context-Aware Map):** Rather than cluttering the screen with thousands of points, our map leverages the **Google Maps API** to filter destinations smartly by range: locating and highlighting key **tourist attractions within a 2km radius** and top-rated **local dining spots within a 1km radius** of your active location. 
*   **Integrated Multi-Modal Transit comparison:** While normal navigation tools only show one route at a time, selecting any location on our map instantly overlay-compares walking paths, driving, and live public transit schedules via a commercial public transit API in a single, glanceable card.

### Feature Comparison Matrix

The table below demonstrates how our solution bridges the gaps left by existing fragmented platforms:

| Feature | Traditional Planners (e.g., Wanderlog) | Navigation Apps (e.g., Google Maps) | Budget Trackers (e.g., Splitwise) | Our Smart Travel Planner |
|:---|:---|:---|:---|:---|
| **All-in-One Dashboard** | ❌ (No budgeting/nav) | ❌ (No budgeting/planning) | ❌ (Expense tracking only)| **✅ Yes (Unified)** |
| **Real-Time Weather Rerouting**| ❌ No | ❌ No | ❌ No | **✅ Yes (Automated)** |
| **Dual Proximity Filtering** | ❌ No | ❌ (No range limits) | ❌ No | **✅ Yes (2km Attractions / 1km Dining)** |
| **Unified Multi-Modal Transit**| ❌ No | ⚠️ Partial | ❌ No | **✅ Yes (Multi-transit overlay)** |
| **Group Travel Gamification** | ❌ No | ❌ No | ❌ No | **✅ Yes (Travel Bingo)** |


## 5. Technical Architecture & Feasibility
### Tech Stack
Frontend - React Native, because it supports both Android & iOS mobile development  
Backend - X  
Database - MongoDB, because it is easy to use  
APIs - Google maps API becuase
Hosting server - Render because

### System architecture diagram 

### Build plan & scope

For this hackathon, our goal is to build a reliable and working prototype. Instead of trying to build everything poorly, we focus on a clean, working demo for **one city (Tokyo)** that proves our core ideas work.

#### What We Will :

We will build a mobile-responsive web app with 3 core screens:

*   **Screen 1: Trip Setup (Landing Screen)**
    *   Users can enter a destination, travel dates, group size, and total budget.
    *   A clean, modern design with a glass-card interface.

*   **Screen 2: Smart Dashboard & Weather Alert**
    *   Displays the selected trip summary and group budget per person.
    *   Shows hostel recommendations based on the user's budget.
    *   **The Weather Twist:** A live alert card that detects rain on trip dates and suggests indoor activities nearby.

*   **Screen 3: Interactive Map & Route Finder**
    *   A map screen with clear filters: places to eat within 1 km and tourist attractions within 2 km.
    *   A route card showing travel time and options for **walking, public transit, or car**.

*   **Fixed Navigation Bar:**
    *   Allows smooth switching between the Home, Budget, and Map screens.

---

### 2. What Is Out of Scope (Future Work)

To make sure our project works smoothly during the judging presentation, we will not build:

*   **Real booking & payments:** We display hostel recommendations and estimated prices, but we will not process real bank payments.
*   **Worldwide data:** We focus our demo data on Tokyo so the app runs fast and without API errors during judging.

