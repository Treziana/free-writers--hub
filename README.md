# FreeWritters - AI-Powered Creative Writing Platform

## Overview
FreeWritters is a comprehensive platform empowering writers to share creative and non-creative works, receive intelligent AI feedback, connect with communities, and showcase their best pieces in a curated gallery.

## 🎯 How It Works

### 1. Upload Writing
- Writers submit work in text or document form
- Supports multiple genres: poems, plays, novels, articles, scripts
- Easy drag-and-drop interface or text editor

### 2. AI Feedback Engine
- AI reads submission and provides constructive comments
- Tailored feedback:
  - **Creative works**: suggestions for tone, imagery, emotional impact
  - **Articles**: clarity, structure, argument flow
- Choose AI personas: Mentor, Critic, or Supportive Coach
- Real-time feedback with specific line-by-line comments

### 3. Quality Gate → Gallery
- AI determines if work is polished and impactful
- Approved works promoted to public gallery
- Readers can browse, engage, and appreciate works

### 4. Community & Growth
- Peer review circles for collaborative feedback
- Co-authoring capabilities
- AI tracks progress over time:
  - Vocabulary growth
  - Style development
  - Creative improvements
- Gamification: badges, milestones, spotlight author of the week

## ⭐ Unique Features

### Interactive Gallery
- Readers highlight favorite lines
- Leave comments and feedback
- Request more works from authors
- Social sharing integration

### AI Prompt Generator
- Overcome writer's block
- Genre-specific creative prompts
- Daily writing challenges

### Mood Analyzer
- Detect emotional tone of writing
- Suggest adjustments for impact
- Emotional resonance scoring

### Cross-Media Support
- Upload audio (spoken word performances)
- Visual attachments (illustrations, covers, artwork)
- Video readings of works

### Privacy Controls
- Publish anonymously
- Keep feedback private
- Control who can see work
- Selective sharing options

### Multilingual Support
- AI translation of works
- Global reach for writers
- Support multiple languages

## 🏗️ Project Structure

```
free-writers--hub/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── styles/
│   │   └── App.js
│   └── package.json
├── backend/
│   ├── routes/
│   ├── controllers/
│   ├── models/
│   ├── middleware/
│   ├── utils/
│   └── server.js
├── database/
│   └── schema.sql
├── docker-compose.yml
├── .env.example
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js 16+
- PostgreSQL 13+
- Redis 6+
- Docker & Docker Compose (optional)

### Quick Start with Docker
```bash
docker-compose up
```

Access:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000/api
- Database: localhost:5432

### Manual Setup

1. **Backend Setup**
```bash
cd backend
npm install
cp .env.example .env
# Edit .env with your configuration
npm run migrate
npm run dev
```

2. **Frontend Setup**
```bash
cd frontend
npm install
npm start
```

## 📚 Key Features Implementation

### AI Feedback System
- Integrates with OpenAI GPT-4
- Genre-aware analysis
- Multiple AI personas
- Real-time suggestions

### Gallery System
- Smart curation algorithm
- Quality scoring
- Search and filtering
- Trending works

### Community Features
- Peer review system
- Writing circles
- Collaboration tools
- Author profiles

### Analytics Dashboard
- Writing statistics
- Progress tracking
- Reader engagement metrics
- Growth insights

## 🔐 Security
- JWT authentication
- Password hashing (bcrypt)
- Input validation
- CORS protection
- Rate limiting

## 📝 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

### Submissions
- `POST /api/submissions` - Create submission
- `GET /api/submissions` - List user submissions
- `GET /api/submissions/:id` - Get submission details
- `PUT /api/submissions/:id` - Update submission
- `DELETE /api/submissions/:id` - Delete submission

### AI Feedback
- `POST /api/feedback/analyze` - Get AI feedback
- `POST /api/feedback/mood` - Analyze mood/tone
- `POST /api/feedback/prompts` - Generate writing prompts

### Gallery
- `GET /api/gallery` - Browse published works
- `GET /api/gallery/trending` - Trending works
- `GET /api/gallery/search` - Search gallery
- `POST /api/gallery/:id/comment` - Add comment

### Community
- `GET /api/circles` - List writing circles
- `POST /api/circles` - Create circle
- `POST /api/reviews` - Submit peer review
- `GET /api/users/:id/profile` - User profile

## 🎮 Gamification
- **Badges**: First submission, 100 readers, Consistent writer
- **Milestones**: Words written, Works published, Reviews received
- **Leaderboards**: Most read, Most reviewed, Rising star
- **Spotlight**: Author of the week

## 📊 Technology Stack

### Frontend
- React 18
- Tailwind CSS
- Redux Toolkit
- Monaco Editor
- Socket.io-client

### Backend
- Node.js + Express
- PostgreSQL
- Redis
- OpenAI API
- JWT Authentication

### DevOps
- Docker & Docker Compose
- GitHub Actions (CI/CD)
- AWS S3 (file storage)

## 🤝 Contributing
Contributions welcome! Please:
1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Open Pull Request

## 📄 License
MIT License - see LICENSE file

## 📞 Support
For issues or questions, open a GitHub issue or contact support.

---

**Made with ❤️ for writers everywhere**
