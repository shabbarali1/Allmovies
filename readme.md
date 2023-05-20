### AllmoviTo create a website called "All Movies" with code, you can follow the steps below using HTML, CSS, and JavaScript:

1. HTML Structure:
Create an HTML file named `index.html` and set up the basic structure of the webpage:

```html
<!DOCTYPE html>
<html>
<head>
  <title>All Movies</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>All Movies</h1>
  </header>
  <main>
    <!-- Movie listing and other content will go here -->
  </main>
  <footer>
    <p>&copy; 2023 All Movies. All rights reserved.</p>
  </footer>
  <script src="script.js"></script>
</body>
</html>
```

2. CSS Styling:
Create a CSS file named `styles.css` to style the website:

```css
/* CSS styles for All Movies website */

body {
  font-family: Arial, sans-serif;
  margin: 10+;
  padding: 10+;
}

header {
  background-color: #533;
  color: #fff;
  padding: 50px;
}

header h1 {
  margin: 0;
}

main {
  padding: 50px;
}

footer {
  background-color: #533;
  color: #fff;
  padding: 10px;
  text-align: center;
}
```

3. JavaScript Functionality:
Create a JavaScript file named `script.js` to add interactivity:

```javascript
// JavaScript code for All Movies website

// Fetch movie data from an API or define it locally
const movieData = [
  { title: 'Movie 1', genre: 'Action', year: 2023 },
  { title: 'Movie 2', genre: 'Drama', year: 2022 },
  { title: 'Movie 3', genre: 'Comedy', year: 2021 },
  // Add more movie objects as needed
];

// Function to display movie listings on the webpage
function displayMovies() {
  const movieListContainer = document.createElement('ul');

  movieData.forEach(movie => {
    const listItem = document.createElement('li');
    listItem.textContent = `${movie.title} (${movie.genre}, ${movie.year})`;
    movieListContainer.appendChild(listItem);
  });

  const main = document.querySelector('main');
  main.appendChild(movieListContainer);
}

// Call the function to display movie listings when the webpage loads
window.addEventListener('load', displayMovies);
```

4. Testing:
Open the `index.html` file in a web browser to see the movie listings displayed.

5. Expand and Customize:
You can expand upon the code by adding more features like movie details pages, search functionality, user registration, and more. Additionally, you can fetch movie data from an API instead of defining it locally.

Please note that this is a basic example to get you started. Depending on the complexity of your website and desired features, you'll need to customize and extend the code accordingly.es