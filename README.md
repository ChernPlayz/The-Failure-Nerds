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


## 5. Technical Architecture & Feasibility
### Tech Stack
Frontend - React Native, because it supports both Android & iOS mobile development  
Backend - X  
Database - MongoDB, because it is easy to use  
APIs - Google maps API becuase
Hosting server - Render because

### System architecture diagram

### Build plan & scope