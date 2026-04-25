# 📰 News Magazine App

A modern **News Magazine Web App** built using **React** that fetches and displays the latest news articles from an API.

This project helps in understanding API integration, component-based architecture, and dynamic UI rendering in React.

---

# 🚀 Features

* 📰 Latest news articles display
* 🔍 Category-based news (Technology, Sports, Business, etc.)
* ⚡ Fast and responsive UI
* 🌐 API integration
* 🔄 Dynamic data rendering

---

# 🛠️ Tech Stack

* React (Vite)
* JavaScript (ES6)
* News API
* Tailwind CSS (optional styling)

---

# ⚙️ Installation & Setup

```bash
# Clone the repository
git clone https://github.com/guptamayank9/News-Magzine.git

# Go to project folder
cd News-Magzine

# Install dependencies
npm install

# Start the project
npm run dev
```

---

# 🌐 API Integration

The app fetches news using an external API.

Example:

```js
useEffect(() => {
  fetch("https://newsapi.org/v2/top-headlines?country=in&apiKey=YOUR_API_KEY")
    .then(res => res.json())
    .then(data => console.log(data));
}, []);
```

---

# 🧠 How It Works

### 🔹 useState

```js
const [articles, setArticles] = useState([]);
```

👉 Stores fetched news data

---

### 🔹 useEffect

```js
useEffect(() => {
  fetchNews();
}, []);
```

👉 Runs when component loads

---

### 🔹 Rendering Data

```jsx
{articles.map((news, index) => (
  <div key={index}>
    <h2>{news.title}</h2>
  </div>
))}
```

👉 Loops through news and displays it

---

# 🎨 UI

* Clean layout
* Responsive design
* Cards for news articles

---

# 📚 What I Learned

* API fetching using useEffect
* Handling JSON data
* React component structure
* Dynamic rendering using map()
* State management

---

# 🔮 Future Improvements

* Add search functionality
* Add pagination
* Add loading spinner
* Add dark mode

---

# 👨‍💻 Author

**Mayank Gupta**

---

# ⭐ Notes

This project is built for learning React and API integration.
