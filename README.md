# Overview

AI Thumbnail Generator is a full-stack web application that allows users to create visually appealing thumbnails using AI. Users can customize title text, style presets, color schemes, aspect ratios, and additional prompts to generate unique thumbnails optimized for social media and YouTube content.

The application integrates AI image generation APIs with a modern React frontend and a scalable Node.js backend architecture.

---

# Features

* 🔐 User Authentication System
* 🎨 AI-powered thumbnail generation
* 🖼️ Multiple thumbnail styles
* 🌈 Dynamic color schemes
* 📐 Custom aspect ratio selection
* ☁️ Cloudinary image storage integration
* 🔄 Real-time thumbnail polling and updates
* 📱 Responsive modern UI
* ⚡ Fast API-based image generation
* 🧩 Reusable React Context architecture
* 🔒 Secure backend authentication with cookies/JWT
* 🚀 Production-ready deployment setup

---

# AI Integrations

### Google Gemini API

Used for:

* AI image generation
* Prompt enhancement
* Thumbnail styling customization

### Prompt Engineering

Custom prompt templates are used for:

* Thumbnail styles
* Color schemes
* Artistic variations
* Image enhancement

### AI Features Included

* Bold Graphic thumbnails
* Futuristic tech designs
* Minimalist layouts
* Photorealistic outputs
* Illustrated thumbnail styles

---

# Frontend Stack

## Technologies Used

* React
* TypeScript
* Vite
* Axios
* React Context API
* React Hooks
* Tailwind CSS
* React Hot Toast

## Frontend Features

* Authentication Context Management
* API Integration using Axios
* Protected Routes
* Dynamic Thumbnail Preview
* Loading State Handling
* Polling for AI-generated image updates
* Responsive User Interface

---

# Backend API Integrations

## Technologies Used

* Node.js
* Express
* MongoDB
* Cloudinary
* JWT Authentication
* Middleware Architecture

## Backend Features

* REST API architecture
* Authentication middleware
* Secure cookie handling
* AI thumbnail generation pipeline
* Cloudinary image uploads
* MongoDB data persistence
* Error handling middleware
* Route-based modular backend structure

## Example API Endpoints

```bash
POST /api/auth/signup
POST /api/auth/login
POST /api/user/generate-thumbnail
GET /api/user/thumbnail/:id
POST /api/user/logout
```

---

# Deployment

## Frontend Deployment

Frontend is deployed using:

* Vercel

## Backend Deployment

Backend can be deployed using:

* Render
* Railway
* Render

## Environment Variables

```env
PORT=
MONGODB_URI=
JWT_SECRET=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
GEMINI_API_KEY=
CLIENT_URL=
```

---

# Project Structure

```bash
client/
 ├── src/
 ├── components/
 ├── context/
 ├── pages/

server/
 ├── controllers/
 ├── middleware/
 ├── routes/
 ├── models/
 ├── services/
```

---

# Installation

## Clone Repository

```bash
git clone https://github.com/Codechef555/ai_thumbnail_generator.git
```

## Install Dependencies

### Frontend

```bash
cd client
npm install
npm run dev
```

### Backend

```bash
cd server
npm install
npm run dev
```

---

# Future Improvements

* AI text generation for titles
* Template marketplace
* Thumbnail history dashboard
* Drag-and-drop editor
* Multiple export formats
* Team collaboration features

---

# Author

Developed by Md.Karaamathullah sheriff - Full Stack AI developer

GitHub:(https://github.com/Codechef555/ai_thumbnail_generator.git)
