# 🎫 Event Management System
A minimalist, high-contrast event registration system featuring a Flask backend, MySQL persistence, and a modern "Glassmorphism" frontend. This system generates unique QR-coded digital passes and provides an administrative dashboard for real-time participant tracking.

## ✨ Features
- Encrypted UI: Sleek, dark-themed interface with gold accents and CSS backdrop filters.

- Dynamic QR Generation: Automatically generates a Base64-encoded QR code upon registration.

- PDF Pass Issuance: Server-side PDF generation (via FPDF) for downloadable entry tickets.

- Admin Dashboard: A protected management view to monitor total entries and participant details.

- Relational Storage: Robust data handling using PyMySQL.

---

## 🛠️ Tech Stack
- Frontend: HTML5, CSS3 (Custom Variables), Vanilla JavaScript (Fetch API).

- Backend: Python 3, Flask, Flask-CORS.

- Database: MySQL.

- Libraries: qrcode (Image generation), fpdf (PDF generation), PyMySQL (DB Driver).

---
## 📥 Installation & Setup
### 1. Database Configuration

- Ensure you have MySQL installed. The system will automatically create the database college_events and the required table on the first run.

- Update the db_config in app.py with your credentials:

  db_config = {
  
      'host': 'localhost',
  
      'user': 'root',       # Your MySQL username
  
      'password': '1302',   # Your MySQL password
  
      'cursorclass': pymysql.cursors.DictCursor
  
  }

### 2. Backend Setup
   #### 1. Navigate to the project folder:

      cd project-directory

   #### 2. Install dependencies:

       pip install flask flask-cors pymysql qrcode fpdf pillow
			 
The server will start at http://127.0.0.1:5000.

   #### 3. Frontend Setup
	 
				Simply open index.html in any modern web browser. No compilation is required.

---

## ⚙️ System Usage

### User Registration (index.html)

- Enter Full Name, Email, and Phone.

- Select an event (e.g., Innovation Hack).

- Click Request Access.

- Once granted, view your unique QR code and click Download PDF Pass to save your entry ticket.

### Admin Dashboard (admin.html)

- Click System Admin Login at the bottom of the registration page.

- Enter the System Key: admin123.

- View live statistics, total registration counts, and the full participant roster.

---

## 📑 API Endpoints

<img width="896" height="352" alt="image" src="https://github.com/user-attachments/assets/0817c944-3b79-438e-9d7a-501b408293dd" />


## 🛡️ Security Note

- The admin password is currently hardcoded as admin123 for demonstration purposes.

- The system uses CORS to allow the frontend to communicate with the Flask API locally.

---

## 📄 License

- This project is open-source and available under the MIT License.

---

## 👤 Author

- **Name:** Dhrumi Shah, Debankita Biswas

- **Role:** Lead Developer / System Architect

- **GitHub:** [@yourusername](https://github.com/yourusername)
