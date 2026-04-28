**SMART EMERGENCY RESPONSE SYSTEM (SERS)**

A real-time, offline-capable emergency response platform designed for large environments like hotels, campuses, and hospitals.

The system enables instant SOS-based crisis reporting, coordinated staff response, and AI-assisted decision support—while continuing to function even during network failures.

**Problem:**

In large, decentralized environments:

Emergency reporting is often delayed
Communication between guests and staff is fragmented
Systems fail during connectivity loss

This leads to slow response and increased risk during critical situations.

**Solution**

SERS provides a human-triggered, real-time emergency reporting and coordination system with offline resilience.

⚡ Instant SOS-based alert triggering
🔄 Real-time coordination across staff dashboards
🧠 AI-based classification of emergencies
🔌 Offline-first functionality with background sync

**Key Screens**
# Dashboard – Real-time emergency monitoring and alerts
# SOS / Report – Instant emergency reporting interface
# History – Track past and resolved emergencies
# Staff Panel – Manage responses and update status
# Admin Controls – System overview and role management

**Key Features**

# Emergency Handling
# One-Tap SOS Button for instant reporting
# AI Classification (type + severity using Gemini AI)
# Multi-Level Severity System (Level 1–3 Critical)
#Live Status Tracking (Active → Resolved)

**Real-Time Coordination**
Instant alert broadcasting using Socket.IO
Centralized dashboard for all staff
Role-based access (Admin / Staff / Guest)
Shared visibility of ongoing emergencies

**Offline-First Capability (Core Highlight)**
Works even without internet connectivity
Uses LocalStorage for emergency handling
Staff can:
View alerts
Update status
Continue operations offline
Automatic sync to server when connection returns

**AI Integration**
Powered by Gemini AI
Classifies:
Emergency type (Medical, Fire, Security)
Severity level (1–3)
Assists in faster decision-making

**Centralized Dashboard**
Real-time monitoring of all emergencies
Status-based filtering
Critical alert highlighting
Unified command view for admins

🧑‍💼 **User Roles**
*Guest
Trigger SOS alerts
View personal emergency status

*Staff
Receive real-time alerts
Respond and update status

*Admin
Manage system
Monitor all emergencies
Control access and roles

🔐 **Authentication Model (Prototype)**
Initial system setup requires internet
Users join via campus/system access code
First login must be online
After login:
Users can access system offline
If a user has never logged in online:
They are treated as Guest in offline mode

⚠️ **QR-Based Reporting (In Progress)**
QR system is generated from dashboard
Intended for guest entry without app install
Full scanning + routing integration is under development

🛠️ **Tech Stack**
Frontend: React, TypeScript, Tailwind CSS,Tanstack query
Backend: Node.js, Express
Database: MongoDB Atlas
Real-Time: Socket.IO
AI Integration: Gemini AI
Offline Support: LocalStorage + Sync Engine

🔄 **System Flow**
**Online Mode**

User → Frontend → Backend → DB
        ↓
     Socket.IO → Staff Dashboards
        ↓
     AI → Classification

**Offline Mode**

User → Frontend → LocalStorage
      ↓
  Local Dashboard Updates

Reconnect → Sync → Backend → DB

📱 Responsive Design
Mobile-first UI
Optimized for quick emergency actions
Works across desktop, tablet, and mobile devices
🔒 Security Note

This is a prototype system.

**For production use:**

Implement secure authentication (JWT/OAuth)
Encrypt sensitive data
Enforce strict RBAC
Ensure compliance with data protection standards
🚧 Future Improvements
Full authentication system
Complete QR-based reporting flow
Push notifications
Advanced staff auto-assignment
Analytics dashboard
Mobile app support
## 🎯 Future Enhancements

### Potential Features
- []JWT Authentication support
- []Complete QR-based reporting flow
- []Push notifications
- [ ] Voice-based SOS input
- [ ] AI panic detection and severity upgrade
- [ ] Indoor location tracking (GPS/Bluetooth beacons)
- [ ] Integration with building management systems
- [ ] Mobile app (iOS/Android)
- [ ] Wearable device support
- [ ] Video call integration for remote assistance
- [ ] Analytics and reporting dashboard
- [ ] Multi-language support

