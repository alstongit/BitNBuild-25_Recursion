# 🎓 GigCampus

**GigCampus** is a hyperlocal, two-sided marketplace designed to connect student freelancers with clients within their university and local community. It provides a complete, end-to-end project lifecycle—from project posting and bidding to secure payments and reputation building—creating a self-sustaining micro-economy for student talent.

---

## 🚀 Backstory

Within any university ecosystem, there exists a wealth of untapped student talent in fields like design, coding, writing, and tutoring. These students are eager for real-world experience and opportunities to earn an income. Simultaneously, there is a constant demand for these skills from other students, campus clubs, and local businesses who need affordable, short-term help. The primary barrier is the lack of a centralized, trusted platform to efficiently connect this supply and demand.

---

## 🏆 Problem Statement

Develop **GigCampus**, a platform that:

- Connects student freelancers with clients (students, clubs, local businesses)
- Provides a trusted, end-to-end project workflow
- Enables secure payments and reputation building
- Fosters a campus micro-economy for student talent

---

## ✨ Key Features

### 1. Project Marketplace & Bidding System
- **Clients** can post detailed project requirements, timelines, and budgets.
- **Student freelancers** can browse projects and place competitive bids, submitting a proposal and price.
- **Bidding UI**: Projects, bids, and proposals are managed via intuitive dashboards.

### 2. Secure Payment Escrow
- **Escrow system**: Client’s payment is held securely when a bid is accepted.
- **Release on approval**: Funds are released to the freelancer only after the client marks the project as complete.
- **Trust**: Ensures both parties are protected throughout the project lifecycle.

### 3. Integrated Real-Time Chat with File Sharing
- **Messaging system**: Built-in chat supports real-time text and file sharing (designs, code, docs).
- **Centralized communication**: All project-related discussions and files are documented on the platform.

### 4. Dynamic Portfolio & Reputation System
- **Automatic portfolio**: Completed work is added to the student’s public portfolio.
- **Ratings & reviews**: Both client and freelancer can rate and review each other.
- **Reputation score**: Transparent, verifiable scores influence future opportunities.

---

## 🛠️ Tech Stack

- **Frontend**: React (Vite), Tailwind CSS
- **Backend**: Supabase (Postgres, Auth, Storage, Realtime)
- **State Management**: React Context API
- **Routing**: React Router
- **Other**: Lucide Icons, Custom Hooks

---

## 📂 Project Structure

```
frontend/
│
├── public/
│   └── vite.svg
├── src/
│   ├── components/
│   │   ├── Bids/                # Bid cards, bid lists, attachments
│   │   ├── Chat/                # Real-time chat UI
│   │   ├── Contracts/           # Contract overview and cards
│   │   ├── Dashboard/           # Dashboards for clients/freelancers
│   │   ├── Deliverables/        # Deliverable cards, list, modal
│   │   ├── Landing/             # Landing page sections
│   │   ├── Milestones/          # Milestone cards, list, creation form
│   │   ├── Profile/             # Profile overview, settings, reviews
│   │   ├── Projects/            # Project posting, details, summary
│   │   ├── Register/            # Registration form components
│   │   └── ui/                  # Shared UI elements (buttons, cards)
│   ├── context/                 # Auth context
│   ├── lib/                     # Supabase client, hooks, utils
│   ├── pages/                   # Main app pages (Login, Register, Dashboard, etc.)
│   ├── App.jsx
│   └── main.jsx
└── ...
```

---

## 🖥️ Main User Flows

### 1. **Client Flow**
- Register/login as a client
- Post a project with requirements and budget
- Review bids from student freelancers
- Accept a bid (escrow funds are held)
- Chat with freelancer, manage milestones and deliverables
- Approve work and release payment
- Leave a review

### 2. **Freelancer Flow**
- Register/login as a student freelancer
- Browse available projects
- Place bids with proposals and pricing
- Chat with clients, view milestones
- Submit deliverables for funded milestones
- Get paid upon approval, build portfolio
- Receive reviews and grow reputation

---

## 📦 Key Components

- **Project Marketplace**: Browse, post, and bid on projects
- **Bidding System**: Submit and manage bids
- **Contracts & Milestones**: Track project progress and payments
- **Deliverables**: Upload and review work for each milestone
- **Escrow Payments**: Secure, conditional fund release
- **Chat**: Real-time messaging and file sharing
- **Portfolio & Reviews**: Showcase work and build trust

---

## 🏛️ Database Overview

- **users / profiles**: Auth, roles, and profile info
- **projects**: Project postings
- **bids**: Bids on projects
- **contracts**: Accepted bids, project agreements
- **milestones**: Project phases, funding, and deliverables
- **deliverables**: Files and notes submitted for milestones
- **reviews**: Ratings and feedback

---

## 📝 How to Run Locally

1. **Clone the repo**
2. **Install dependencies**
   ```bash
   npm install
   ```
3. **Set up your `.env` with Supabase keys**
4. **Start the dev server**
   ```bash
   npm run dev
   ```
5. **Visit** [http://localhost:5173](http://localhost:5173)

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License

MIT

---

## 💡 Inspiration

GigCampus is inspired by the real needs of students and campus communities to unlock talent, build experience, and create new opportunities—right where they are.

---