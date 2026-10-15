# 🚀 QUICK START GUIDE

## **Get HireWizard Running in 2 Minutes!**

### **Step 1: Install Python Dependencies**
```bash
cd backend
pip install -r requirements.txt
```

### **Step 2: Run the Server**
```bash
python app.py
```

### **Step 3: Open Browser**
```
http://localhost:5000
```

### **That's it! The app is running! 🎉**

---

## **First Time Using?**

### **Create an Account:**
1. Click "Get Started"
2. Enter name, email, password
3. Click "Create Account"

### **Complete Profile (Choose One):**

**Option A - Upload Resume:**
- Drag-drop your resume
- Wait for analysis
- Done!

**Option B - Fill Manually:**
- Phone, location, experience
- Expected salary, skills
- Education, LinkedIn
- Submit!

### **Browse Jobs:**
- Use search bar
- Apply filters
- Click "Apply Now"
- Save for later

---

## **Sample Login (For Testing)**

If you don't want to create account:

**Email:** `demo@hirewizard.com`  
**Password:** `demo123`

(Create this account first OR signup normally)

---

## **Need Help?**

- Check README.md for full documentation
- Backend not starting? Check if port 5000 is free
- Can't see jobs? Make sure backend is running
- Resume upload not working? Check file size < 16MB

---

## **Common Issues**

**"Port 5000 already in use"**
```python
# Edit backend/app.py, change last line to:
app.run(debug=True, host='0.0.0.0', port=5001)
```

**"Module not found"**
```bash
pip install Flask Flask-CORS Werkzeug
```

**"Can't connect to server"**
- Make sure you access via `http://localhost:5000`
- NOT `file:///path/to/index.html`

---

**Enjoy HireWizard! 🎯**