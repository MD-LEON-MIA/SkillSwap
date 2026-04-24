# SkillSwap Project PRD

[](https://trello.com/invite/b/69acf2bf71c2ad8a3d4fec82/ATTIad73ab814464c92ec7682a9d9042857fB160E792/skillswap)

> **Version: 1.0**
> 

> **Status: In Development**
> 

> **Lead: MD.LEON MIA**
> 

**Objective:** **To create a decentralized peer-to-peer platform where users can exchange skills without monetary involvement, using a skill-matching engine.**

---

<aside>
🎯

# 1.Problem Statement & Goals

- **Problem:** Many students want to learn new skills, but face two major hurdles: finding affordable, high-quality tutors and discovering a platform to showcase their own expertise. While they are often experts in certain subjects (e.g., Programming), they lack a medium to share that knowledge. SkillSwap bridges this gap by creating a collaborative community where learning becomes a mutual exchange.
- **Goal:** To build a platform that connects users based on mutual skill needs ("Offer" vs "Wanted"), promoting a community of learning.
</aside>

---

<aside>
📋

# 2. Functional Requirements (Features)

| Feature | Priority | Description |
| --- | --- | --- |
| **User Auth** | Critical | Secure Registration & Login with Password Hashing. |
| **Skill Matrix** | Critical | Users can list skills they "Offer" and "Want". |
| **Matching Engine** | Critical | Backend logic to match reciprocal skill needs. |
| **Request Cycle** | High | Send request -> Accept/Reject -> Reveal Contact. |
| **Rating System** | Medium | Users rate each other based on exchange quality. |
</aside>

---

<aside>
⚙️

# 3. Non-Functional Requirements

- **Security:** Use SHA-256 for password hashing.
- **Usability:** Modern, responsive UI using Guna UI2.
- **Performance:** Matching algorithm must execute in under 2 seconds.
- **Scalability:** Database should handle concurrent users.
</aside>

---

<aside>
👤

# 4. User Stories

- **As a user,** I want to create a profile with my skills so that others can find me.
- **As a user,** I want to search for people who can teach me "Piano" while I teach them "Python."
- **As a user,** I want to see a rating of the other person before accepting a swap request to ensure trust.
- **As a user,** I want to mark the task as "Completed" after the exchange to update my rating.
</aside>

---

<aside>
🛠️

# 5. Technical Stack

**Frontend & UI Design:**

- **Framework/Library:** React.js (or Modern JavaScript)
- **Styling:** CSS3 / Tailwind CSS (for the Glassmorphism, Dark Mode, and Gradient effects)
- **Design Aesthetic:** Dark Glassmorphism, Frosted Glass Cards, Gradient Borders

**Platform & Version Control:**

- **Development Platform:**
- **Version Control:** Git & GitHub

**Project Management:**

- **Dashboard:** Custom Web Dashboard (`/dashboard`)
- **UI Components:** Custom glass-morphism cards, responsive navbar
</aside>

---

<aside>
🧠

# 6. Logic Workflow (Matching Engine)

The system follows a **Two-Way Mutual Matching** logic:

1. **Query:** `WHERE MyWantedSkill = TargetOfferSkill AND MyOfferSkill = TargetWantedSkill`.
2. **Filter:** Sort by User Rating (Highest first).
3. **Result:** Display as a profile card on the Dashboard.
</aside>

---

<aside>
🚀

# 7. Future Scope / Roadmap (v2.0)

- **AI-Powered Skill Suggestion:** Intelligent algorithms to recommend skills based on market trends and user interest.
- **Real-time Chat Integration:** Instead of just contact disclosure, implement an in-app chat system for safer communication.
</aside>

---