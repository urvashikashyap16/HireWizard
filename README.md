<div align="center">

# 🧙 HireWizard

### *Get Hired, Get Inspired!*

**An engineering job aggregator that scrapes Naukri, LinkedIn and Indeed into one searchable dashboard.**

![Python](https://img.shields.io/badge/Python-3-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-REST_API-000000?style=for-the-badge&logo=flask&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-Scraping-028090?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

</div>

---

## 💡 Why it exists

Engineering job hunting means checking three or four portals every day. HireWizard pulls listings from all of them, removes duplicates, and lets you filter by location, salary and experience in one place. It cuts manual search time by roughly 80%.

---

## ✨ **FEATURES**

### 🎨 **Ultra-Modern Frontend**
- **Glassmorphism Design** - Frosted glass effect with blur
- **Animated Particle Background** - Interactive particle system
- **Smooth Animations** - Fade-ins, slide-ups, hover effects
- **Responsive Layout** - Works on desktop, tablet, mobile
- **Modern Typography** - Poppins font for clean look
- **Gradient Overlays** - Beautiful purple/blue gradients

### 🔐 **Complete Authentication System**
- **Sign Up** - Create new account with validation
- **Login** - Secure login with password hashing
- **Logout** - Clean session management
- **Profile Management** - Complete user profiles
- **LocalStorage** - Persistent login sessions
- **Password Security** - Hashed passwords (Werkzeug)

### 📄 **Profile Setup (Both Options)**
1. **Resume Upload**
   - Drag & drop interface
   - File preview before upload
   - Supports PDF, DOC, DOCX
   - Automatic profile completion

2. **Manual Form**
   - Phone number
   - Location (dropdown)
   - Experience level
   - Expected salary
   - Skills (comma-separated)
   - Education
   - LinkedIn profile (optional)

### 💼 **Job Features**
- **450+ Sample Jobs** - From TCS, Infosys, Wipro, Amazon, etc.
- **Advanced Filters** - Location, salary, experience, source
- **Smart Search** - Search by title, company, skills
- **Job Cards** - Beautiful glassmorphism cards
- **Apply & Save** - Quick actions
- **Load More** - Pagination
- **Source Badges** - Naukri, LinkedIn, Indeed

### 🗄️ **Backend & Storage**
- **Flask REST API** - Clean, modular endpoints
- **JSON Database** - Simple file-based storage
- **File Upload** - Resume handling with secure storage
- **CORS Enabled** - Frontend-backend communication
- **Error Handling** - Proper HTTP status codes
- **LocalStorage** - Browser-side session persistence

---

## 📁 **PROJECT STRUCTURE**

```
hirewizard-complete/
├── frontend/
│   ├── index.html          # Main HTML (complete UI)
│   ├── styles.css          # Glassmorphism CSS (1457 lines)
│   └── app.js              # JavaScript with particles & auth
├── backend/
│   ├── app.py              # Flask API server
│   └── requirements.txt    # Python dependencies
├── data/
│   ├── users.json          # User database
│   ├── jobs.json           # Jobs database
│   └── applications.json   # Applications database
├── uploads/                # Resume uploads folder
└── README.md              # This file
```

---

## 🚀 **HOW TO RUN**

### **Prerequisites**
- Python 3.8 or higher
- Modern web browser (Chrome, Firefox, Safari)
- Terminal/Command Prompt

### **Step 1: Setup Backend**

```bash
# Navigate to backend folder
cd backend

# Install Python dependencies
pip install -r requirements.txt

# Run Flask server
python app.py
```

**Backend will start on:** `http://localhost:5000`

### **Step 2: Open Frontend**

The Flask server automatically serves the frontend!

**Open in browser:** `http://localhost:5000`

That's it! Everything runs together! 🎉

---

## 📖 **HOW TO USE**

### **1. Landing Page**
- See beautiful animated particle background
- View hero section with stats
- Click "Get Started" or "Login"

### **2. Sign Up**
1. Click "Get Started" button
2. Fill in:
   - Full Name
   - Email
   - Password
   - Confirm Password
3. Agree to Terms & Conditions
4. Click "Create Account"

### **3. Profile Setup (Choose One)**

**Option A: Upload Resume**
1. Click "Upload Resume"
2. Drag & drop your resume OR click Browse
3. Preview file
4. Click "Analyze Resume"
5. Wait for processing

**Option B: Fill Manually**
1. Click "Fill Manually"
2. Enter all details:
   - Phone number
   - Location
   - Experience level
   - Expected salary
   - Skills
   - Education
   - LinkedIn (optional)
3. Click "Complete Profile"

### **4. Dashboard**
- Browse 450+ jobs
- Use filters:
  - Search bar
  - Location dropdown
  - Salary range
  - Experience level
  - Job source
- Click "Apply Now" on any job
- Save jobs for later
- Click profile avatar → Settings/Logout

### **5. Logout**
1. Click profile avatar (top right)
2. Click "Logout"
3. Return to landing page

---

## 🎯 **API ENDPOINTS**

### **Authentication**
- `POST /api/auth/signup` - Register new user
- `POST /api/auth/login` - Login user

### **Profile**
- `POST /api/profile/update` - Update profile
- `POST /api/profile/upload-resume` - Upload resume file

### **Jobs**
- `GET /api/jobs` - Get all jobs
- `POST /api/jobs/filter` - Filter jobs
- `GET /api/jobs/<id>` - Get single job

### **Applications**
- `POST /api/applications/apply` - Apply to job
- `GET /api/applications/user/<id>` - Get user applications

### **Analytics**
- `GET /api/analytics/stats` - Get platform stats

---

## 💾 **DATA STORAGE**

### **LocalStorage (Browser)**
- `currentUser` - Active session data
- Persists across page refreshes
- Cleared on logout

### **JSON Files (Backend)**
1. **users.json** - All user accounts
   ```json
   {
     "id": "uuid",
     "name": "John Doe",
     "email": "john@example.com",
     "password": "hashed_password",
     "profileComplete": true,
     "phone": "+91 9876543210",
     "skills": ["React", "Node.js"]
   }
   ```

2. **jobs.json** - All job listings
3. **applications.json** - All applications

### **File System**
- `uploads/` folder stores resume files
- Filename format: `{userId}_{originalname}`

---

## 🎨 **DESIGN SYSTEM**

### **Colors**
- **Primary:** Purple (#7c3aed)
- **Secondary:** Blue (#3b82f6)
- **Background:** Dark (#0f0f1e)
- **Glass:** rgba(255, 255, 255, 0.05)

### **Fonts**
- **Primary:** Poppins (Google Fonts)
- **Weights:** 300, 400, 500, 600, 700, 800

### **Effects**
- Glassmorphism (backdrop-filter: blur)
- Particle animations (Canvas API)
- Smooth transitions (0.3s cubic-bezier)
- Hover lift effects (translateY)

---

## 🔒 **SECURITY FEATURES**

1. **Password Hashing** - Werkzeug security
2. **Input Validation** - Frontend & backend
3. **File Type Checking** - Only PDF, DOC, DOCX
4. **File Size Limit** - 16MB maximum
5. **Secure Filenames** - Werkzeug secure_filename
6. **CORS Protection** - Flask-CORS configured

---

## 📱 **RESPONSIVE BREAKPOINTS**

- **Desktop:** 1024px+
- **Tablet:** 768px - 1023px
- **Mobile:** < 768px

All features work on all devices!

---

## 🐛 **TROUBLESHOOTING**

### **Backend won't start**
```bash
# Make sure you're in backend folder
cd backend

# Install dependencies again
pip install -r requirements.txt

# Try different port
python app.py  # Change port in app.py if 5000 is busy
```

### **Frontend not loading**
- Make sure backend is running first
- Open `http://localhost:5000` (not file://)
- Check browser console for errors

### **Can't upload resume**
- Check file size (< 16MB)
- Use PDF, DOC, or DOCX format
- Make sure `uploads/` folder exists

### **Login not working**
- Check browser localStorage is enabled
- Clear localStorage: `localStorage.clear()`
- Try signup with new email

---

<div align="center">Built by <a href="https://github.com/urvashikashyap16">Urvashi Kashyap</a> 💜</div>
