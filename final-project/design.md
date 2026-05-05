# Design System

## Typography

| Role | Font |
|------|------|
| Heading 1 | Source Sans Pro Bold |
| Heading 2 | Source Sans Pro Regular |
| Body | Instrument Sans Regular |

---

## Colors

| Token | Hex | Usage |
|-------|-----|-------|
| Background | `#F2F0EF` | Off-white page background |
| Text | `#373838` | Primary text gray |
| Teacher Comments | `#61A5AB` | Teal — annotation pop-ups |
| High Credibility | `#D8F3DC` | Green — high credibility indicator |
| Mixed Credibility | `#FFB922` | Yellow — mixed credibility indicator |
| Low Credibility | — | Red — low credibility indicator |

---

## Components

### Navigation
- Class Feed
- Submissions
- Analytics
- Notifications

> Navigation is fixed to the top of the screen.

---

### Content Blocks
- **Posts** — student-submitted sources shown on the class feed
- **Comments** — student discussion on posts
- **Bulletin Board** — feed layout for displaying all approved posts

---

### Inputs
- Text fields
- Drop-down menus
- Sliders

---

### Actions

| Actor | Actions |
|-------|---------|
| Student | Submit posts, add comments |
| Teacher | Annotate posts, remove/flag posts, assign credibility scores, make notes public or private |

---

### Feedback States
- **URL validation** — validates links before submission
- **Loading screen** — shown while articles are being uploaded
- **Confirmation screen (student)** — prompts student to verify before submitting
- **Confirmation screen (teacher)** — final review before post goes live on the feed

---

## System Rules

### Roles
- **Students** post sources, discuss with each other, and view teacher notes/annotations.
- **Teachers** observe interactions, add notes/annotations, and approve or reject posts — teachers do not post sources themselves.

### Submission Flow
1. Student submits a post → sees a confirmation screen before sending.
2. Teacher reviews the submission → sees a final confirmation screen before approving to the feed.
3. Approved post appears on the class feed.

### Teacher Annotations
- Notes appear both in the **notification box** and **on the post itself**.
- Teachers can mark notes as **public** (visible to all) or **private** (visible only to the submitting student).
- Teacher notes render as a **teal pop-up box** (`#61A5AB`).
