<script>
	export let name;
	let colleagues = [
		{ name: "Téo Berton", image: "/www/Portfolio/static/berton.jfif", portfolio: "https://teoberton.com" },
		{ name: "Téo Georges", image: "/www/Portfolio/static/golem.png", portfolio: "https://georgesteo.fr" },
		{ name: "Haik Khatchatrian", image: "/www/Portfolio/static/haik.png", portfolio: "http://khhaik.fr" },
	];
</script>
  
  <main>
	<header>
	  <nav>
		<a href="#introduction">Introduction</a>
		<a href="#formations">Formations</a>
		<a href="#skills">Skills</a>
		<a href="#experiences">Experiences</a>
		<a href="#projects">Projects</a>
	  </nav>	  
	</header>
  
	<section id="introduction" class="introduction">
	  <img src="/www/Portfolio/static/photo.jpg" alt="{name}'s photo" class="profile-photo" />
	  <h2>Hello, I'm {name}</h2>
	  <p>I am a passionate developer with experience in various technologies.</p>
	</section>

	<section id="formations" class="formations">
		<h2>Formations</h2>
		<div class="formation-container">
		  <div class="formation">
			<h3>Engineer Diploma</h3>
			<h4>CESI École d'Ingénieur</h4>
			<p>2022 - Now</p>
			<p>Field : IT</p>
			<p>Nancy, France</p>
		  </div>
		  <div class="formation">
			<h3>Integrated Preparatory Cycle</h3>
			<h4>CESI École d'Ingénieur</h4>
			<p>2020 - 2022</p>
			<p>Field : IT</p>
			<p>Nancy, France</p>
		  </div>
		  <div class="formation">
			<h3>Secondary Diploma</h3>
			<h4>Institut Notre-Dame de la Providence</h4>
			<p>2008 - 2020</p>
			<p>Field : Science</p>
			<p>Thionville, France</p>
		  </div>
		  <!-- Ajoutez d'autres formations au besoin -->
		</div>
	</section>

	<h2>Skills</h2>
	<section id="skills" class="skills">
		
		<div class="skill-list">
		  <div class="skill-sublist">
			<h3>Web Development</h3>
			<ul>
			  <li>HTML</li>
			  <li>CSS</li>
			  <li>JavaScript</li>
			  <li>Svelte/SvelteKit</li>
			</ul>
		  </div>
		  <div class="skill-sublist">
			<h3>Back-end Development</h3>
			<ul>
			  <li>Node.js</li>
			  <li>SQL</li>
			  <li>FastAPI</li>
			  <li>PHP</li>
			</ul>
		  </div>
		  <div class="skill-sublist">
			<h3>Programming</h3>
			<ul>
			  <li>C#</li>
			  <li>C++</li>
			  <li>Python</li>
			</ul>
		  </div>
		  <div class="skill-sublist">
			<h3>Frameworks & Libraries</h3>
			<ul>
			  <li>.Net Framework</li>
			  <li>WinForm</li>
			  <li>WPF</li>
			</ul>
		  </div>
		  <div class="skill-sublist">
			<h3>Operating System</h3>
			<ul>
			  <li>Windows</li>
			  <li>Linux</li>
			  <li>Ubuntu</li>
			  <li>WSL</li>
			</ul>
		  </div>
		</div>
	</section>
	  
	<section id="experiences" class="formations">
		<h2>Experiences</h2>
		<div class="formation-container">
		  <div class="formation">
			<h3>IT Research Engineer</h3>
			<h4>TechLab Mines</h4>
			<p>2023</p>
			<p>Internship</p>
			<p>Nancy, France</p>
		  </div>
		  <div class="formation">
			<h3>Fullstack Developer</h3>
			<h4>PIXY'IT</h4>
			<p>2022</p>
			<p>Internship</p>
			<p>Nancy, France</p>
		  </div>
		  <div class="formation">
			<h3>Maintenance Agent</h3>
			<h4>Centre Hospitalier Emile Mayrisch (CHEM)</h4>
			<p>2021</p>
			<p>Fixed-term contract</p>
			<p>Esch-sur-Alzette, Luxembourg</p>
		  </div>
		  <div class="formation">
			<h3>Architecture Intern</h3>
			<h4>WW+ Design</h4>
			<p>2018</p>
			<p>Observation Internship</p>
			<p>Esch-sur-Alzette, Luxembourg</p>
		  </div>
		  <div class="formation">
			<h3>Technical Engineering Intern</h3>
			<h4>Engie Solelec SA</h4>
			<p>2017</p>
			<p>Observation Internship</p>
			<p>Esch-sur-Alzette, Luxembourg</p>
		  </div>
		</div>
	</section>

	<h2>Projects</h2>
	<section id="projects" class="projects">
	  <div class="project">
		<h3>Arduino Weather Station</h3>
		<p>A C-coded Arduino weather station with humidity, solar, temperature and GPS sensors.</p>
	  </div>
  
	  <div class="project">
		<h3>Database Management Application</h3>
		<p>A Winform application with integrated C++ interface for database management</p>
	  </div>
  
	  <div class="project">
		<h3>Backup Management Application</h3>
		<p>A WPF application with integrated interface coded in C# for managing backup jobs, encrypting them or scheduling backups.</p>
	  </div>
	</section>

	<section id="get-in-touch" class="get-in-touch">
		<h2>Get in touch</h2>
		<div class="contact">
		  <a class="contact-link" href="https://www.linkedin.com/in/hugomztl" target="_blank"><img class="logo" src="/www/Portfolio/static/in.png" alt="LinkedIn">Hugo MAZZITELLI</a>
		  <a class="contact-link" href="mailto:hugo.mazzitelli@viacesi.fr"><img class="logo" src="/www/Portfolio/static/mail.png" alt="Email">hugo.mazzitelli@viacesi.fr</a>
		  <a class="contact-link" href="tel:+33625786064"><img class="logo" src="/www/Portfolio/static/tel.png" alt="Phone">+33 6 25 78 60 64</a>
		</div>
	</section>
	  
	<section id="colleagues" class="colleagues">
		<h2>My Colleagues</h2>
		<div class="colleague-container">
			{#each colleagues as colleague (colleague.name)}
				<div class="colleague">
					<img src="{colleague.image}" alt="{colleague.name}'s photo" class="colleague-photo" />
					<h3>{colleague.name}</h3>
					<a href="{colleague.portfolio}" target="_blank">View Portfolio</a>
				</div>
			{/each}
		</div>
	</section>

  </main>
  
<style>
	main {
	  text-align: center;
	  padding: 1em;
	  max-width: 800px;
	  margin: 0 auto;
	}
	
	.contact {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 1em;
    margin-top: 2em;
  }
  
  .contact-link {
    display: flex;
    align-items: center;
    text-decoration: none;
    color: #333;
	transition: 330ms;
  }

  .contact-link:hover{
	border-radius: 5px;
	transition: 330ms;
	scale: 110%;
  }
  
  .logo {
    width: 24px;
    height: 24px;
    margin-right: 0.5em;
  }

	header {
	  margin-bottom: 2em;
	}
  
	h2 {
	  font-size: 2em;
	  margin-bottom: 0.5em;
	}
  
	.introduction {
	  display: flex;
	  flex-direction: column;
	  align-items: center;
	  margin-bottom: 2em;
	}
  
	.profile-photo {
	  width: 150px;
	  height: 150px;
	  border-radius: 50%;
	  object-fit: cover;
	  margin-bottom: 1em;
	}
  
	.projects {
	  display: grid;
	  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
	  gap: 1em;
	}
  
	.project {
	  background-color: #f1f1f1;
	  padding: 1em;
	  border-radius: 5px;
	}
  
	@media (min-width: 640px) {
	  main {
		max-width: none;
	  }
	}

	nav {
		display: flex;
		justify-content: center;
		gap: 1em;
		margin-bottom: 1em;
		align-items: center; /* Ajoutez cette ligne pour aligner les liens sur la même ligne que les boutons */
	}

	nav a {
		text-decoration: none;
		color: #333;
		padding: 0.25em 0.5em; /* Modifiez cette ligne pour réduire la taille du padding */
		font-size: 1.25em; /* Ajoutez cette ligne pour réduire la taille du texte */
		border: 1px solid #333;
		border-radius: 3px;
		transition: background-color 0.3s;
	}


	nav a:hover {
		background-color: #333;
		color: #fff;
	}

	header {
		background-color: #f1f1f1;
		padding: 1em 0;
		box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
		position: sticky;
		top: 0;
		z-index: 1000;
  	}

.skills {
  margin-bottom: 2em;
  display: flex;
  justify-content: center;
}

.skill-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 2em;
  list-style-type: none;
  padding: 0;
  max-width: 1200px; /* Limiter la largeur de la liste principale */
}


.skill-sublist h3 {
  font-size: 1.2em;
  margin-bottom: 0.5em;
}

.skill-sublist ul {
  list-style-type: none;
  padding: 0;
}

.skill-sublist li {
  background-color: #f1f1f1;
  padding: 1em;
  border-radius: 5px;
  margin-bottom: 1em;
}

	.formations {
		margin-bottom: 2em;
		background-color: #f8f9fa;
		padding: 1em;
		border-radius: 5px;
	}

	.formation-container {
		display: grid;
		grid-template-columns: repeat(2, 1fr);
		flex-wrap: wrap;
		gap: 1em;
		justify-content: center;
	}

	.formation {
		flex: 1;
		min-width: 250px;
		background-color: #fff;
		padding: 1em;
		border-radius: 5px;
		box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
	}

	.formation h3 {
		font-size: 1.5em;
		margin-bottom: 0.5em;
	}

	.formation h4 {
		font-size: 1.2em;
		margin-bottom: 0.5em;
	}

	.colleagues {
		margin-bottom: 2em;
	}

	.colleague-container {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
		gap: 2em;
	}

	.colleague {
		background-color: #f1f1f1;
		padding: 1em;
		border-radius: 5px;
		text-align: center;
	}

	.colleague-photo {
		width: 100px;
		height: 100px;
		border-radius: 50%;
		object-fit: cover;
		margin-bottom: 1em;
	}

	.colleague a {
		text-decoration: none;
		color: #333;
		padding: 0.25em 0.5em; /* Modifiez cette ligne pour réduire la taille du padding */
		font-size: 1.25em; /* Ajoutez cette ligne pour réduire la taille du texte */
		border: 1px solid #333;
		border-radius: 3px;
		transition: background-color 0.3s;
	}
	.colleague a:hover{
		background-color: #333;
		color: #fff;
	}
</style>
  