# EmergencyBD

A full-stack emergency response web application for Bangladesh. Citizens can report emergencies with their live location and photos, request funds, and track status updates. Admins verify and resolve reports through a dedicated portal.

Built as a semester project by a student team across 20 features in 4 sprints.

## Features

**Users**
- Registration and login with JWT authentication
- Submit emergency reports with description and image uploads
- Automatic GPS location capture with reverse geocoding (OpenStreetMap Nominatim)
- Google Maps deep links to report locations
- Submit fund requests
- Gmail-style notification system: bell badge with unread count, `/notifications` page, category sidebar, detail panel, bulk actions, search and sort
- Real-time notification triggers on report/fund submission and on admin status changes

**Admin**
- Admin portal to review reports and fund requests
- Status workflow: `Pending → Verified → Resolved`
- Image lightbox and download

**Maps**
- Interactive map showing emergency locations as pins with report details (Leaflet / react-leaflet)

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 18, react-leaflet / Leaflet |
| Backend | Node.js, Express |
| Database | MongoDB Atlas, Mongoose |
| Authentication | JSON Web Tokens (JWT) |
| File uploads | Multer |
| Geocoding | OpenStreetMap Nominatim |
| Version control | Git, GitHub |

## Design

Dark theme: background `#111111`, accent green `#00ff88`, text `#e0e0e0`.

## Getting Started

### Prerequisites
- Node.js and npm installed
- A MongoDB Atlas cluster and connection string

### Installation

```bash
git clone [https://github.com/NimasNawfas/EmergencyBD.git](https://github.com/NimasNawfas/EmergencyBD.git)
cd EmergencyBD
