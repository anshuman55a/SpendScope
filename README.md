# SpendScope - Personal Finance Tracker

SpendScope is a modern web application designed to help users track their personal finances effectively. With SpendScope, you can easily monitor your income and expenses, categorize transactions, and gain insights into your spending habits through an intuitive dashboard.

## Features

- Interactive Dashboard
- Income and Expense Tracking
- Transaction History
- Responsive Design
- Secure User Authentication
- Financial Analytics

## Tech Stack

- **Frontend**: React.js, Tailwind CSS, Framer Motion
- **Backend**: Flask (Python)
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens)

## Project Structure

```
SpendScope/
├── backend/
│   ├── app.py              # Main Flask application
│   ├── requirements.txt    # Python dependencies
│   └── .env               # Environment variables
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── App.js        # Main React component
│   │   └── index.js      # React entry point
│   ├── package.json      # Node.js dependencies
│   └── tailwind.config.js # Tailwind CSS configuration
└── docker-compose.yml    # Docker configuration
```

## Prerequisites

- Python 3.8+
- Node.js 14+
- MongoDB 4.4+
- Git

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/SpendScope.git
cd SpendScope
```

### 2. Backend Setup

```bash
cd backend

# Create virtual environment
python -m venv .venv

# Activate virtual environment
# On Windows:
.venv\Scripts\activate
# On Unix or MacOS:
source .venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Start the backend server
python app.py
```

### 3. MongoDB Setup

1. Install MongoDB from [MongoDB Download Center](https://www.mongodb.com/try/download/community)
2. Start MongoDB service:
   - Windows: MongoDB should run as a service automatically
   - Unix/MacOS: `sudo systemctl start mongod`
3. The backend will connect to MongoDB at `mongodb://localhost:27017/`
4. Database name: `personal_finance_tracker`
5. Collections: 
   - `financial_entries`
   - `users`

### 4. Frontend Setup

```bash
cd frontend

# Install dependencies
npm install

# Start the development server
npm start
```

## Running the Application

1. Ensure MongoDB is running
2. Start the backend server (runs on http://localhost:5000)
3. Start the frontend development server (runs on http://localhost:3000)
4. Open your browser and navigate to http://localhost:3000

## Environment Variables

Create a `.env` file in the backend directory with the following variables:

```env
JWT_SECRET_KEY=your_secret_key_here
MONGODB_URI=mongodb://localhost:27017/
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


