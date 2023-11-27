<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
	body {
    font-family: 'Noto Sans', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #333; /* Dark Grey Background */
    color: #fff; /* Text color */
}

header {
    background-color: #555; /* Darker Grey Header */
    color: #fff;
    text-align: center;
    padding: 1em 0;
}

nav ul {
    list-style: none;
}

nav li {
    display: inline;
    margin: 0 15px;
}

a {
    text-decoration: none;
    color: #fff;
}

section {
    padding: 50px 20px;
}

.intro, .about-me, .projects, .contact {
    max-width: 800px;
    margin: 0 auto;
}

.project-card {
    border: 1px solid #ddd;
    padding: 15px;
    margin-bottom: 20px;
    overflow: hidden;
}

.project-card img {
    max-width: 100%; 
    height: auto; 
    display: block; 
    margin: 0 auto; 
}

.project-card:hover {
    transform: scale(1.05);
}

#contact-form {
    display: grid;
    gap: 10px;
}

button {
    background-color: #333;
    color: #fff;
    padding: 10px 20px;
    border: 1px solid #fff; /* Add a white border */
    cursor: pointer;
}

button:hover {
    background-color: #555; /* Change color on hover if desired */
}


.social-links {
    display: flex;
    justify-content: center;
    flex-wrap: wrap; /* Allow items to wrap onto multiple lines */
    margin-top: 20px;
}

.social-links a {
    text-decoration: none;
    color: #fff;
    margin: 5px; /* Add margin to create space between links */
}

.social-links a:hover {
    color: #007bff;
}


	</style>
	<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Noto+Sans:wght@400;700&display=swap">
    <title>Dan - Portfolio</title>
</head>
<script>
function hoverProject(element) {
    element.style.boxShadow = '0 0 10px rgba(0, 0, 0, 0.3)';
}

function unhoverProject(element) {
    element.style.boxShadow = 'none';
}

document.getElementById('contact-form').addEventListener('submit', function (event) {
});

</script>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Me</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact Me</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <div class="intro">
		<div style="text-align: center;">
            <h1>Welcome!</h1>
            <p>Thank you for visiting my (first) portfolio page! <br><br> I am Danieal, or you can call me Dan. </br> I am an IM student in UniSZA. <br><br> Curious to know what projects I have done? Go to the 'Projects' section! </br></br></br> P/S: You can click 'Projects' at the top of the page to go there instantly. ;) </p>
        </div>
		</div>
    </section>

    <section id="about">
        <div class="about-me">
            <h2>About Me</h2>
            <img src="https://media.tenor.com/Ow4aJ_k2rgkAAAAC/cat-monday-left-me-broken-cat.gif" alt="dak encem">
            <div style="text-align: center;">
			My full name is Muhammad Danieal bin Rahim, and I am 21 years old. <br><br> I am currently IM3A. I have a passion for graphic designing, but somehow I have to learn how to code a website. </br><br> I am from Johor, and I love Photography, Pokemon, Monster Hunter, and Vocaloid! <br><br> Nice to meet you! </br></br></br></br> </p>
			</div>
		</div>
    </section>

    <section id="projects">
        <div class="projects">
            <h2>Projects</h2>

            <!-- Project 1 -->
            <div class="project-card" onmouseover="hoverProject(this)" onmouseout="unhoverProject(this)">
                <img src="https://i.imgur.com/kctNUy4.png" alt="Lelaki Dewasa Gergaji">
                <h3>Project 1 - To-Do List</h3>
                <p>This is a (very simple) To-Do List app that allows users to add, complete, and delete tasks.</p>
				<p><i> You type what task you want to do for the day inside the input box, and click 'Add Task'. When you done with it, just click 'Delete Task'! </i></p>
                <p>Technologies used: HTML, CSS, JavaScript</p>
                <a href="https://github.com/mhmdanzz/assignment/blob/cc15e9de9f37b7d226eec972e9f3753d1fcbec59/todolist.html" target="_blank">--> GitHub <--</a>
            </div>

			<div class="project-card" onmouseover="hoverProject(this)" onmouseout="unhoverProject(this)">
                <img src="https://i.imgur.com/29LxaqL.png" alt="Lelaki Dewasa Gergaji">
                <h3>Project 2 - Random Quote Generator</h3>
                <p>I call it the Random Motivation Booster Generator. It generate random quotes that you can read to motivate your daily life.</p>
				<p><i> Just click 'Generate Quote', and read the generated quote! </i></p>
                <p>Technologies used: HTML, CSS, JavaScript</p>
                <a href="https://github.com/mhmdanzz/assignment/blob/9421590b7d223ed748b69cd72b5b3e6088550715/quotegenerator.html" target="_blank">--> GitHub <--</a>
            </div>
			
			<div class="project-card" onmouseover="hoverProject(this)" onmouseout="unhoverProject(this)">
                <img src="https://i.imgur.com/PpJRiBv.png" alt="Dota 2-inspired">
                <h3>Project 3 - Trivia Quiz</h3>
                <p>Let's see how much score you can get via this Trivia Quiz! Play while gaining knowledge.</p>
				<p><i> Just click the right answer, and your score will automatically updates as the quiz goes on! </i></p>
                <p>Technologies used: HTML, CSS, JavaScript</p>
                <a href="https://github.com/mhmdanzz/assignment/blob/4da9a63f80a5bb710c63c7ade68b0006b5911aee/triviaquiz.html" target="_blank">--> GitHub <--</a>
            </div>
        </div>
    </section>

    <section id="contact">
    <div class="contact">
        <h2>Contact Me</h2>
        <form id="contact-form">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>

            <button type="submit">Send Message</button>
        </form>


    </div>
	
	<br>
	<br>
	</br>
	</br>
	
	<div style="text-align: center;">
    You can also reach me via social medias, by clicking the links below! ^^
	</div>

    <div class="social-links">
		
        <a href="https://www.instagram.com/mhmdanzz_/" target="_blank">Instagram</a>
        <a href="https://www.facebook.com/mhmdan.02/" target="_blank">Facebook</a>

    </div>
	
</section>


    <script src="script.js"></script>
</body>

</html>
