# 📚 Flashcard Learning App (Leitner System)

A **MERN Stack** application implementing the **Leitner System** for effective spaced repetition learning. Users can create, review, and progress through flashcards based on scientifically proven memory retention techniques.

## 🚀 Features

- **Create & Manage Flashcards**: Add, update, and delete flashcards with ease.
- **Spaced Repetition**: Flashcards move through levels based on correct/incorrect responses.
- **Intelligent Scheduling**: Reviews are dynamically scheduled based on the user’s progress.
- **Progress Tracking**: Displays flashcards due for review each day.
- **Minimal & User-Friendly UI**: Clean interface for a distraction-free learning experience.

## 🛠️ Tech Stack

### Backend (Node.js, Express, MongoDB, Mongoose)
- **API Endpoints:**  
  - `POST /flashcards` → Add a new flashcard  
  - `GET /flashcards` → Retrieve all flashcards  
  - `PUT /flashcards/:id` → Update a flashcard’s level  
  - `DELETE /flashcards/:id` → Remove a flashcard  
- **Leitner System Logic:**  
  - Flashcards start in **Box 1**.  
  - Correct answers move them to the next box.  
  - Incorrect answers send them back to **Box 1**.  
  - Higher boxes have longer review intervals.  

### Frontend (React, Tailwind CSS)
- **Flashcard Display**: Flip cards to reveal answers.  
- **User Interaction**: Mark cards as correct or incorrect.  
- **Scheduled Reviews**: Fetches due flashcards based on next review date.  

## 📌 Installation & Setup

1️⃣ **Clone the Repository**  
```bash
git clone https://github.com/your-repo/flashcard-app.git
cd flashcard-app
```

2️⃣ **Backend Setup**  
```bash
cd backend
npm install
```
- Create a `.env` file in the `backend` directory and add:  
  ```
  PORT=5000
  MONGO_URI=your_mongodb_connection_string
  JWT_SECRET=your_secret_key
  ```
- Run the backend server:  
  ```bash
  npm run dev
  ```

3️⃣ **Frontend Setup**  
```bash
cd frontend
npm install
npm start
```

## 🧠 Thought Process

- **User-Centered Design**: Focused on an intuitive UI to enhance learning efficiency.
- **Performance Optimization**: Implemented efficient database queries and state management.
- **Scalability**: Designed a structured API and database model for future expansions.
- **Spaced Repetition Accuracy**: Ensured the Leitner System logic is accurately followed.

## 📧 Contact
For any inquiries, feel free to reach out: **kasaudhananand2003@gmail.com**

