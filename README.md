<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Writers Club</title>
    <style>
        body {
            font-family: 'Georgia', serif;
            margin: 0;
            padding: 0;
            background-color: #f4f1ea;
            color: #4b3832;
        }
        header {
            background-color: #2a1a15;
            color: #f4f1ea;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
            font-style: italic;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #4b3832;
            padding: 10px 0;
        }
        nav a {
            color: #f4f1ea;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1.2em;
        }
        nav a:hover {
            text-decoration: underline;
        }
        .language-select {
            position: absolute;
            top: 10px;
            right: 20px;
        }
        .language-select select {
            padding: 5px;
            font-size: 1em;
        }
        main {
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        .poetry-card {
            background-color: #ffffff;
            border: 1px solid #dcd7c9;
            padding: 20px;
            margin-bottom: 20px;
            border-radius: 5px;
        }
        .poetry-card h2 {
            margin-top: 0;
            font-size: 1.8em;
        }
        footer {
            text-align: center;
            padding: 15px 0;
            background-color: #2a1a15;
            color: #f4f1ea;
            position: relative;
            bottom: 0;
            width: 100%;
        }
        footer a {
            color: #f4f1ea;
            text-decoration: none;
        }
        footer a:hover {
            text-decoration: underline;
        }
        .search-bar {
            text-align: center;
            margin: 20px 0;
        }
        .search-bar input {
            width: 60%;
            padding: 10px;
            font-size: 1em;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .search-bar button {
            padding: 10px 20px;
            font-size: 1em;
            color: #fff;
            background-color: #4b3832;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .search-bar button:hover {
            background-color: #2a1a15;
        }
        .form-section {
            background-color: #ffffff;
            border: 1px solid #dcd7c9;
            padding: 20px;
            margin: 20px 0;
            border-radius: 5px;
        }
        .form-section h2 {
            margin-top: 0;
        }
        .form-section label {
            display: block;
            margin: 10px 0 5px;
        }
        .form-section input, .form-section textarea, .form-section select, .form-section button {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1em;
        }
        .form-section button {
            background-color: #4b3832;
            color: #fff;
            cursor: pointer;
        }
        .form-section button:hover {
            background-color: #2a1a15;
        }
    </style>
</head>
<body>
    <header>
        <h1>Writers Club</h1>
        <p>"Dive into the timeless world of words"</p>
        <div class="language-select">
            <label for="language">Language: </label>
            <select id="language">
                <option value="en">English</option>
                <option value="hi">Hindi</option>
                <option value="mr">Marathi</option>
            </select>
        </div>
    </header>
    <nav>
        <a href="#">Home</a>
        <a href="#explore">Explore</a>
        <a href="#upload">Upload</a>
        <a href="#register">Register</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>
    <main>
        <div class="search-bar">
            <input type="text" placeholder="Search poetry...">
            <button>Search</button>
        </div>

        <section id="explore">
            <h2>Explore Poetry</h2>
            <div class="poetry-card">
                <h2>Title: Ghazal of Time</h2>
                <p>A mesmerizing ghazal to soothe your soul...</p>
            </div>
            <div class="poetry-card">
                <h2>Title: Shayari on Love</h2>
                <p>Delicate shayari expressing eternal emotions...</p>
            </div>
        </section>

        <section id="upload">
            <h2>Upload Your Work</h2>
            <form>
                <label for="title">Title:</label><br>
                <input type="text" id="title" name="title" required><br><br>
                <label for="category">Category:</label><br>
                <select id="category" name="category">
                    <option value="ghazal">Ghazal</option>
                    <option value="nazm">Nazm</option>
                    <option value="kavita">Kavita</option>
                    <option value="shayari">Shayari</option>
                    <option value="sher">Sher</option>
                    <option value="muktak">Muktak</option>
                </select><br><br>
                <label for="content">Content:</label><br>
                <textarea id="content" name="content" rows="10" cols="50" placeholder="Write your poetry here..." required></textarea><br><br>
                <button type="submit">Upload</button>
            </form>
        </section>

        <section id="register">
            <h2>Create an Account</h2>
            <div class="form-section">
                <form>
                    <label for="username">Username:</label>
                    <input type="text" id="username" name="username" placeholder="Enter your username" required>

                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" placeholder="Enter your email" required>

                    <label for="password">Password:</label>
                    <input type="password" id="password" name="password" placeholder="Create a password" required>

                    <label for="confirm-password">Confirm Password:</label>
                    <input type="password" id="confirm-password" name="confirm-password" placeholder="Re-enter your password" required>

                    <button type="submit">Register</button>
                </form>
            </div>
        </section>
    </main>
    <footer>
        <p>Follow us on <a href="#">Instagram</a> | &copy; 2024 Writers Club</p>
    </footer>
</body>
</html>
