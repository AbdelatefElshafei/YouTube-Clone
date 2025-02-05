# YouTube Clone using Ruby on Rails
![image](https://github.com/user-attachments/assets/f4f8a613-e7da-4c26-b053-e5746c088c39)

This is a YouTube clone built using Ruby on Rails. The application mimics the core functionality of YouTube, including video uploads, playback, user authentication, and a responsive video grid layout. The project is designed to demonstrate how to build a modern web application with Rails, Active Storage, and responsive design.

---

## Features

- **User Authentication**:
  - Sign up, log in, and log out functionality.
  - User profiles with uploaded videos.

- **Video Upload and Playback**:
  - Users can upload videos with titles and descriptions.
  - Videos are stored using Active Storage (local or cloud storage).
  - Video playback using HTML5 `<video>` tag.

- **Responsive Video Grid**:
  - A YouTube-like video grid layout with thumbnails, titles, and metadata.
  - Responsive design for desktop, tablet, and mobile devices.

- **Video Details Page**:
  - Dedicated page for each video with a larger player, title, description, and uploader information.

- **Search Functionality**:
  - Search for videos by title or description.

- **Pagination**:
  - Paginated video listings for better performance and user experience.

---

## Technologies Used

- **Ruby on Rails**: Backend framework for handling requests, database interactions, and business logic.
- **Active Storage**: For handling video uploads and storage.
- **PostgreSQL**: Database for storing users, videos, and metadata.
- **HTML/CSS/JavaScript**: Frontend for rendering the user interface.
- **Tailwind CSS (optional)**: For styling the application (if preferred over custom CSS).
- **Stimulus JS (optional)**: For adding interactivity to the frontend.

---

## Getting Started

### Prerequisites

- Ruby 3.x
- Rails 7.x
- PostgreSQL
- Node.js (for JavaScript dependencies)
- Yarn (for managing frontend dependencies)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/youtube-clone-rails.git
   cd youtube-clone-rails
   ```

2. **Install dependencies**:
   ```bash
   bundle install
   yarn install
   ```

3. **Set up the database**:
   - Update `config/database.yml` with your PostgreSQL credentials.
   - Run the following commands to create and migrate the database:
     ```bash
     rails db:create
     rails db:migrate
     ```

4. **Set up Active Storage**:
   - Run the following command to set up Active Storage:
     ```bash
     rails active_storage:install
     rails db:migrate
     ```
   - Configure storage in `config/storage.yml` (e.g., local disk or cloud services like AWS S3).

5. **Run the application**:
   ```bash
   rails server
   ```
   Visit `http://localhost:3000` in your browser.

---

## Folder Structure

```
youtube-clone-rails/
├── app/
│   ├── assets/
│   ├── controllers/
│   ├── models/
│   ├── views/
│   └── helpers/
├── config/
│   ├── environments/
│   ├── initializers/
│   └── routes.rb
├── db/
│   ├── migrate/
│   └── schema.rb
├── public/
├── test/
├── Gemfile
├── Gemfile.lock
├── README.md
└── ...
```

---

## Usage

### User Authentication

- Sign up for a new account or log in with an existing one.
- Authenticated users can upload videos and view their profile.

### Uploading Videos

1. Log in to your account.
2. Click on the "Upload" button.
3. Fill in the video title, description, and select a video file.
4. Click "Submit" to upload the video.

### Watching Videos

- Browse videos on the homepage.
- Click on a video thumbnail to watch it on the video details page.
---
