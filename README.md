# 🎨 AI Thumbnail Generator

> An AI-powered full-stack platform for creating professional thumbnails for YouTube, social media, and digital content.

<p align="center">

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)

</p>

<p align="center">

![GitHub Stars](https://img.shields.io/github/stars/Codechef555/ai_thumbnail_generator?style=for-the-badge)
![GitHub Forks](https://img.shields.io/github/forks/Codechef555/ai_thumbnail_generator?style=for-the-badge)
![GitHub Issues](https://img.shields.io/github/issues/Codechef555/ai_thumbnail_generator?style=for-the-badge)
![GitHub License](https://img.shields.io/github/license/Codechef555/ai_thumbnail_generator?style=for-the-badge)

</p>

## ✨ Features

- 🤖 **AI-Powered Thumbnail Generation**
  - Generate thumbnails using Google Gemini.
  - Customize generation through structured prompts.

- 🎨 **Multiple Visual Styles**
  - Bold graphics
  - Futuristic designs
  - Minimalist layouts
  - Photorealistic compositions
  - Illustrated styles

- 🌈 **Custom Color Schemes**
  - Select preferred color palettes to influence the generated design.

- 📐 **Custom Aspect Ratios**
  - Generate thumbnails according to different content requirements.

- 🔐 **Secure Authentication**
  - User signup and login.
  - JWT-based authentication.
  - Protected application routes.
  - Secure cookie handling.

- ☁️ **Cloud Image Storage**
  - Generated thumbnails are uploaded and stored using Cloudinary.

- 🔄 **Generation Status Polling**
  - Frontend polling allows users to receive updates while AI-generated thumbnails are being processed.

- 📱 **Responsive Interface**
  - Designed to work across desktop and mobile screen sizes.

- ⚡ **REST API Architecture**
  - Modular backend with controllers, routes, middleware, services, and database models.

---

## 🧠 How It Works

The application follows a simple AI-powered generation pipeline:

```text
User
  │
  ▼
React Frontend
  │
  │  Thumbnail configuration
  ▼
Node.js + Express API
  │
  ├── Authentication
  │
  ├── Prompt Processing
  │
  └── Thumbnail Generation Request
          │
          ▼
     Google Gemini
          │
          ▼
     Generated Image
          │
          ▼
       Cloudinary
          │
          ▼
       MongoDB
          │
          ▼
    React Thumbnail UI
```

---

## 🏗️ System Architecture

### Frontend

The frontend is responsible for:

- User authentication
- Thumbnail configuration
- Prompt submission
- API communication
- Loading and generation states
- Thumbnail preview
- Responsive UI

### Backend

The backend provides:

- REST API endpoints
- Authentication and authorization
- AI generation orchestration
- Database operations
- Image upload handling
- Error handling
- Middleware-based request processing

### External Services

| Service | Purpose |
|---|---|
| **Google Gemini** | AI-powered image generation and prompt processing |
| **MongoDB** | Application and user data persistence |
| **Cloudinary** | Generated image storage and delivery |
| **Vercel** | Frontend deployment |
| **Render / Railway** | Backend deployment |

---

## 🛠️ Tech Stack

### Frontend

- **React**
- **TypeScript**
- **Vite**
- **Tailwind CSS**
- **Axios**
- **React Context API**
- **React Hooks**
- **React Hot Toast**

### Backend

- **Node.js**
- **Express.js**
- **MongoDB**
- **JWT**
- **REST APIs**
- **Middleware Architecture**

### AI & Media

- **Google Gemini API**
- **Prompt Engineering**
- **Cloudinary**

### Deployment

- **Vercel**
- **Render / Railway**

---

## 📂 Project Structure

```text
ai_thumbnail_generator/
│
├── public/
│
├── src/
│   ├── components/
│   ├── context/
│   ├── pages/
│   └── ...
│
├── .gitignore
├── index.html
├── package.json
├── package-lock.json
├── tsconfig.json
├── vite.config.ts
├── eslint.config.js
└── README.md
```

> The repository currently contains the frontend application under `src/`. Backend components can be maintained as a separate server application when deployed as a full-stack setup.

---

# 🚀 Getting Started

## Prerequisites

Make sure you have the following installed:

- **Node.js** 18+
- **npm**
- **MongoDB**
- **Google Gemini API key**
- **Cloudinary account**

---

## 1. Clone the Repository

```bash
git clone https://github.com/Codechef555/ai_thumbnail_generator.git

cd ai_thumbnail_generator
```

---

## 2. Install Dependencies

```bash
npm install
```

---

## 3. Configure Environment Variables

Create a `.env` file in the appropriate application directory.

```env
PORT=5000

MONGODB_URI=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

GEMINI_API_KEY=your_gemini_api_key

CLIENT_URL=http://localhost:5173
```

### ⚠️ Security

Never commit `.env` files or API credentials to GitHub.

Add sensitive environment files to `.gitignore`:

```gitignore
.env
.env.local
.env.production
```

---

## 4. Start the Development Server

```bash
npm run dev
```

The Vite development server will start locally.

Open:

```text
http://localhost:5173
```

---

# 🔌 API Endpoints

The backend exposes RESTful endpoints for authentication and thumbnail generation.

### Authentication

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/auth/signup` | Create a new user account |
| `POST` | `/api/auth/login` | Authenticate a user |
| `POST` | `/api/user/logout` | Logout the current user |

### Thumbnail Generation

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/user/generate-thumbnail` | Generate a new AI thumbnail |
| `GET` | `/api/user/thumbnail/:id` | Retrieve thumbnail generation status/data |

---

# 🎯 Thumbnail Generation Workflow

A typical generation request contains configuration such as:

```text
Title
  ↓
Visual Style
  ↓
Color Scheme
  ↓
Aspect Ratio
  ↓
Additional Prompt
  ↓
AI Generation
  ↓
Cloudinary Upload
  ↓
Thumbnail Result
```

This approach allows creators to control the creative direction while using AI to automate the image-generation process.

---

# 💡 Example Use Cases

### YouTube Creators

Generate attention-grabbing thumbnails for:

- Tech videos
- Tutorials
- Gaming
- Reviews
- Educational content
- AI-related content

### Social Media Creators

Create visual assets for:

- Instagram
- LinkedIn
- X
- Facebook
- Short-form content

### Digital Marketing

Generate promotional graphics and visual concepts for:

- Campaigns
- Product launches
- Advertisements
- Blog content
- Online courses

---

# 🔐 Authentication & Security

The application uses JWT-based authentication to protect user-specific resources.

The authentication architecture includes:

```text
User Login
    ↓
Credentials Validation
    ↓
JWT Generation
    ↓
Secure Cookie
    ↓
Authenticated Request
    ↓
Authentication Middleware
    ↓
Protected API Resource
```

Sensitive configuration such as database credentials, JWT secrets, Gemini API keys, and Cloudinary credentials should always be provided through environment variables.

---

# 📸 Screenshots

Add application screenshots here to showcase the product.

```markdown
![Home Page](./public/screenshots/home.png)

![Thumbnail Generator](./public/screenshots/generator.png)

![Generated Thumbnail](./public/screenshots/result.png)
```

Recommended screenshots:

1. Landing page
2. Thumbnail generation interface
3. Generated thumbnail result
4. Authentication page
5. User dashboard

---

# 🚀 Deployment

## Frontend

The frontend can be deployed using platforms such as:

- Vercel
- Netlify

## Backend

The backend can be deployed using:

- Render
- Railway

Before deployment, configure all required environment variables in the hosting provider.

---

# 🗺️ Roadmap

Future improvements planned for the platform include:

- [ ] AI-assisted title generation
- [ ] Thumbnail generation history
- [ ] User dashboard
- [ ] Template marketplace
- [ ] Drag-and-drop thumbnail editor
- [ ] Multiple export formats
- [ ] Advanced image editing
- [ ] Batch thumbnail generation
- [ ] Brand kit / saved brand styles
- [ ] Team collaboration
- [ ] Usage analytics
- [ ] Subscription and credit-based generation system

---

# 📊 Future Product Vision

The long-term goal is to evolve the project from a simple AI image-generation application into a complete **AI-powered creative workspace for content creators**.

Potential future workflow:

```text
Content Idea
     ↓
AI Title Generation
     ↓
Thumbnail Concept
     ↓
AI Image Generation
     ↓
Thumbnail Editing
     ↓
A/B Variations
     ↓
Export
     ↓
Performance Analytics
```

---

# 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

### Fork the repository

```bash
git fork
```

### Create a feature branch

```bash
git checkout -b feature/your-feature
```

### Commit your changes

```bash
git commit -m "feat: add your feature"
```

### Push the branch

```bash
git push origin feature/your-feature
```

Then open a Pull Request.

---

# 📄 License

This project is licensed under the **MIT License**.

See the [LICENSE](./LICENSE) file for more information.

---

# 👨‍💻 Author

**Md. Karaamathullah Sheriff**

AI & Full-Stack Developer

- GitHub: [@Codechef555](https://github.com/Codechef555)
- Repository: [AI Thumbnail Generator](https://github.com/Codechef555/ai_thumbnail_generator)

---

## ⭐ Support

If you find this project useful or interesting, consider giving the repository a ⭐ on GitHub.

---

> **AI Thumbnail Generator — turning content ideas into visually engaging thumbnails with AI.**
