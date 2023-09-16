<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Netflix Clone</title>
</head>
<body>
    <header>
        <nav>
            <div class="logo">
                <img src="https://wallpaperaccess.com/full/2772922.png" alt="Netflix Logo">
            </div>
            <div class="nav-links">
                <a href="#">Home</a>
                <a href="#">Movies</a>
                <a href="#">TV Shows</a>
                <a href="#">My List</a>
            </div>
        </nav>
    </header>

    <main>
        <!-- Movie/TV show cards go here -->
        <div class="movie-card">
            <img src="https://www.tollywood.net/wp-content/uploads/2020/12/Salaar-First-look-from-Prashanth-Neel-film-The-most-violent-Prabhas.jpg" alt="Movie Title">
            <h2>salaar 2023</h2>
            <p>Genre: Action</p>
            <div class="buttons">
                <button class="watch-now">Watch Now</button>
                <button class="download">Download</button>
            </div>
        </div>
        <!-- Repeat the above card structure for more movies/shows -->
    </main>

    <footer>
        <div class="subscribe">
            <button class="subscribe-btn">Subscribe</button>
        </div>
    </footer>
</body>
</html>

/* Reset some default styles */
body, h1, h2, p {
    margin: 0;
    padding: 0;
}

/* Style the header */
header {
    background-color: #111;
    color: #fff;
    padding: 20px;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo img {
    width: 120px;
    height: auto;
}

.nav-links a {
    color: #fff;
    text-decoration: none;
    margin-right: 20px;
}

/* Style the main content */
main {
    padding: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

.movie-card {
    width: 250px;
    margin-bottom: 20px;
}

.movie-card img {
    width: 100%;
    height: auto;
}

.movie-card h2 {
    margin-top: 10px;
    font-size: 18px;
}

.movie-card p {
    font-size: 14px;
    color: #777;
}

.buttons {
    margin-top: 10px;
}

button {
    padding: 10px 20px;
    margin-right: 10px;
    background-color: #e50914;
    color: #fff;
    border: none;
    cursor: pointer;
}

/* Style the footer */
footer {
    background-color: #111;
    padding: 20px;
    text-align: center;
}

.subscribe-btn {
    padding: 10px 20px;
    background-color: #e50914;
    color: #fff;
    border: none;
    cursor: pointer;
}

function showTime() {
	document.getElementById('currentTime').innerHTML = new Date().toUTCString();
}
showTime();
setInterval(function () {
	showTime();
}, 1000);
