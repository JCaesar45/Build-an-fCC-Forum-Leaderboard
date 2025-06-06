````markdown
# freeCodeCamp Forum Leaderboard

A responsive web app that displays the latest topics, users, and replies from the freeCodeCamp forum. Built with vanilla JavaScript, HTML, and CSS, this project fetches real-time forum data and presents it in a user-friendly leaderboard format.

---

## Features

- Shows latest forum topics with post titles and categories
- Displays avatars of users who contributed to each topic
- Shows number of replies and views per topic
- Displays relative time since last activity (e.g., "15m ago", "2h ago", "3d ago")
- Category links styled dynamically based on category type
- Responsive layout for desktop and mobile

---

## User Stories

- Calculate and display relative time elapsed for each post's last activity
- Format view counts, abbreviating values above 1000 with “k”
- Dynamically generate category links with appropriate styling and URLs
- Render avatar images of users who posted on each topic
- Fetch forum data asynchronously from the freeCodeCamp forum API
- Display all information in a structured table format

---

## Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/fcc-forum-leaderboard.git
```

2. Navigate to the project directory:

   ```bash
   cd fcc-forum-leaderboard
   ```
3. Open `index.html` in your browser.

---

## Usage

* The app automatically fetches the latest forum posts and populates the leaderboard on page load.
* Click on post titles or category names to navigate to the respective freeCodeCamp forum pages.
* Avatars display the contributors for each topic.

---

## File Structure

```
fcc-forum-leaderboard/
│
├── index.html         # Main HTML structure
├── styles.css         # Styling for the leaderboard
├── script.js          # JavaScript logic and API fetching
└── README.md          # Project documentation
```

---

## Technical Details

* **API Endpoint:**
  `https://cdn.freecodecamp.org/curriculum/forum-latest/latest.json`

* **Main Functions:**

  * `timeAgo(timestamp)`: Converts ISO 8601 timestamp to relative time string.
  * `viewCount(views)`: Formats views, abbreviating over 1000 as “k”.
  * `forumCategory(id)`: Returns styled category anchor element string.
  * `avatars(posters, users)`: Generates avatar images string for posters.
  * `showLatestPosts(data)`: Populates the leaderboard table with fetched data.
  * `fetchData()`: Asynchronously fetches the forum data and triggers display.

---

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/yourusername/fcc-forum-leaderboard/issues) if you want to contribute.

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

## Acknowledgments

* Thanks to [freeCodeCamp](https://www.freecodecamp.org) for the forum API and inspiration.
* Built as part of a learning lab to practice JavaScript and API integration.

---

**Happy coding! 🚀**

```
