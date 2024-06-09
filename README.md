
# My portfolio

This module is based on my portfolio which includes my work History and my personal information.


## Deployment

To deploy this project run  

https://dosanjhkiran.github.io/myportfolio/

### Screenshot
filepath: (advanced-css/screenshot)

## Features
. full screen mode
. live previews
. easily accesible


### 🛠 Skills
HTML, CSS, github, ...

## License

[MIT](https://github.com/dosanjhkiran/myportfolio/blob/main/LICENSE)


## 🔗 Links
git hub: https://github.com/dosanjhkiran



##HTML

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Advanced CSS</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Navigation bar -->
  <header class="header-background">
      <h1>Welcome to My Portfolio</h1>
  </header>
  <nav>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
  <main>
     <!-- About me content -->
     <section id="about">
        <h2>~ About Me ~</h2>
        <img src="../images/ab.jpg" alt="Kirandeep's Profile">
        <p>Hello there! I work with EnergyAustralia and I have done a Bachelor's of Computer Application.</p>
        <p>I am enjoying learning new skills every day from this course. By the end of the course, I hope to have learned most coding concepts, which will help me to obtain my desired job.</p>
    </section>
    <!-- Portfolio content -->
    <section id="portfolio">
      <h2>My Work History</h2>
      <div class="project">
        <img src="../images/download.jpeg" alt="Project 1">
        <p>Project 1</p>
      </div>
      <div class="project">
        <img src="../images/aiam.jpg" alt="Project 2">
        <p>Project 2</p>
      </div>
      <div class="project">
        <a href="https://dosanjhkiran.github.io/html-module/" target="_blank">
          <img src="../images/photos.jpeg" alt="Project 3">
          <p>Project 3</p>
        </a>
      </div>
      <div class="project">
        <img src="../images/tech.jpg" alt="Project 4">
        <p>Project 4</p>
      </div>        
    </section>
    <section id="contact">
        <h2>~ Keep in Touch ~</h2>
        <button class="btn">Send me a message!</button>
    </section>
  </main>
  <footer>
      <p>I made it with pure love</p>
  </footer>
</body>
</html>


### CSS 
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header.header-background {
    background-color: #df9191;
    padding: 20px;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
    text-align: center;
}

nav ul li {
    display: inline-block;
    margin: 0 10px;
    font-weight: bold;
}

nav ul li a {
    text-decoration: none;
    color: #921919;
    padding: 10px 15px;
    transition: background-color 0.3s ease, color 0.3s ease;
}

nav ul li a:hover {
    background-color: #e0f7fa;
    color: #000;
}

main {
    padding: 20px;
}

section#about, section#portfolio, section#contact {
    margin-bottom: 50px;
    font-weight: bold;
}

h2 {
    text-align: center;
    font-size: 24px;
    margin-bottom: 20px;
}

section#about img, section#portfolio img {
    display: block;
    margin: 0 auto 20px;
    max-width: 200px; /* Adjusted size */
    height: auto;
    border-radius: 10px;
}

section#about p, section#portfolio p, section#contact p {
    text-align: center;
    font-size: 18px;
    line-height: 1.5;
}

.project {
    text-align: center;
    margin-bottom: 30px;
    display: inline-block;
    width: 100%;
    margin: 2.5%;
    padding: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
    transition: transform 0.3s ease, background-color 0.3s ease;
}

.project p {
    background-color: #f4f4f4;
    padding: 5px;
    border-radius: 10px;
    transition: background-color 0.3s ease;
}

.project:hover {
    transform: scale(1.05);
    background-color: #327b85;
}

.project p:hover {
    background-color: #007bff;
    color: #fff;
}

.project img {
    width: 100%;
    max-width: 150px;
    height: auto;
    margin-bottom: 10px;
    border-radius: 10px;
}

section#contact .btn {
    display: block;
    width: 200px;
    margin: 20px auto;
    padding: 10px 20px;
    font-size: 18px;
    text-align: center;
    text-decoration: none;
    color: #fff;
    background-color: #007bff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

@media (max-width: 600px) {
    nav ul li {
        display: block;
        margin: 10px 0;
    }

    .project {
        width: 100%;
        margin: 10px 0;
    }

    .project img {
        max-width: 100px;
    }
}


