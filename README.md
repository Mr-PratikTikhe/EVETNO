# 🎉 EVENTO - Inter-College Event Management Platform

EVENTO is a next-generation event management platform designed for **inter-college events**. Organizers can create events, manage registrations, and provide internship opportunities, while students can explore events, purchase tickets, and apply for internships — all in one seamless experience. 🚀

---

## 🌟 Key Features
✅ **Role-Based Authentication** (Organizers & Students)  
✅ **Event Creation & Management** (by Organizers)  
✅ **Event Registration & Ticket Purchase** (by Students)  
✅ **Internship Enrollments & Management**  
✅ **Firebase Firestore for Real-Time Database**  
✅ **Firebase Storage for Secure Media Uploads**  
✅ **Deployed on Vercel for Scalability**  

---

## 🏗️ Tech Stack
| **Technology** | **Usage** |
|--------------|------------|
| **React.js** | Frontend UI |
| **Node.js & Express.js** | Backend API |
| **Firebase Firestore** | NoSQL Database |
| **Firebase Storage** | Media Hosting |
| **RazorPay** | Payment Gateway |
| **Vercel** | Deployment |

---

## 🎭 User Roles & Flow
### 👩‍🎓 Student Role
- 🔑 Registers/logs in via Firebase Authentication.
- 📌 Redirected to the student dashboard.
- 🎫 Views available events & internships.
- 📝 Registers for events by filling out a form.
- 💳 Purchases event tickets.
- 💼 Enrolls in internships.

### 🎤 Organizer Role
- 🔑 Registers/logs in via Firebase Authentication.
- 📌 Redirected to the organizer dashboard.
- 📅 Creates new events (title, description, date, venue, etc.).
- 📊 Manages event registrations.
- 💼 Manages internship applications.

---

## 📂 Database Structure (Firestore)
```plaintext
/Users
  /{userId}
    - name: string
    - email: string
    - role: "student" | "organizer"

/Events
  /{eventId}
    - title: string
    - description: string
    - date: timestamp
    - venue: string
    - organizerId: string

/Registrations
  /{registrationId}
    - userId: string
    - eventId: string
    - ticketPurchased: boolean

/Internships
  /{internshipId}
    - title: string
    - company: string
    - description: string
    - appliedUsers: array
```

---

## 🛠️ Setup & Installation
### 🔹 Open Project in VS Code
1. Open the project folder in VS Code.
2. Navigate to the backend folder.

### 🔹 Backend Setup
```sh
 cd backend
 npm install
 node server.js
```

### 🔹 Frontend Setup
```sh
 cd frontend
 npm install
 npm start
```

### 🔹 Configure Firebase
1. Create a Firebase project.
2. Enable Firestore, Authentication, and Storage.
3. Add Firebase config to `.env.local`.


---

## 🚀 Deployment
### **Deploying on Vercel**
```sh
 vercel deploy
```

---

## 🔮 Future Enhancements  
📊 **AI-Based Event Recommendations**  
⭐ **Event Feedback & Rating System**  

---

## 📜 License
📄 **MIT License**  

Developed with ❤️ by **EVENTO Team**.

---

## 👨‍💻 Creators
🎨 **Lead Developer:** Pratik Tikhe  
🎨 **UI Designer:** Ansh Nikhare  
🎨 **role:** Priyant Nikhare  
🎨 **role:**Sujal Bhimgade  
🎨 **role:** Ayush Bokde  
