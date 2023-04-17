<script>
  import SocialIcons from '@rodneylab/svelte-social-icons';
</script>

<svelte:head>
	<title>Luis Felipe Manfroni</title>
	<meta name="description" content="Meu portfolio" />
	<link rel="preconnect" href="https://fonts.googleapis.com">
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="use-credentials">
	<link href="https://fonts.googleapis.com/css2?family=Merriweather&family=Dancing+Script:wght@500&display=swap" rel="stylesheet">
</svelte:head>

<section>
	<h1 class="title">Luis Felipe Manfroni</h1>
	<div class="profile-picture">
    <img src="profile.jpg" alt="Uma linda foto de um homem chamado Luis." />
  </div>

  <div class="socials">
    <div class="socials-icons">
      <a href="https://instagram.com/luismanfroni">
        <SocialIcons network="instagram" bgColor="#f0f0f0" />
      </a>
      <a href="https://github.com/luismanfroni">
        <SocialIcons network="github" bgColor="#f0f0f0" />
      </a>
      <a href="https://www.linkedin.com/in/luis-felipe-manfroni-b70ba413b/">
        <SocialIcons network="linkedin" bgColor="#f0f0f0" />
      </a>
      <a href="https://twitch.com/luisrebaixado">
        <SocialIcons network="twitch" bgColor="#f0f0f0" />
      </a>
    </div>
  </div>

  <div class="projects">
    <h3 class="projects-title">Projetos</h3>
    <div class="projects-list">
      <div class="project-item">
        <a href="https://github.com/luismanfroni/surviving-items-backpack">
          <h5 class="project-item-title">Algorítimo Genético em JS</h5>
        </a>
        <div class="project-item-description">
          Algorítimo genético feito em Javascript com o conceito de sobrevivência usando mochila e itens.
        </div>
      </div>

      <div class="project-item">
        <a href="https://github.com/luismanfroni/eight-puzzle-nim">
          <h5 class="project-item-title">Resolvendo 8-Puzzle em Nim</h5>
        </a>
        <div class="project-item-description">
          Resolvendo o jogo 8-puzzle usando a linguagem Nim com algoritimo a*.
        </div>
      </div>

      <div class="project-item">
        <a href="https://github.com/luismanfroni/hacker-news-explorer">
          <h5 class="project-item-title">App Hackernews em Flutter</h5>
        </a>
        <div class="project-item-description">
          App mobile explorador de noticias do Hackernews feito em Flutter.
        </div>
      </div>
    </div>
  </div>
</section>

<style>
* {
	font-family: 'Merriweather', serif;
	color: #f0f0f0;
}

.profile-picture {
  display: flex;
  justify-content: center;
}
.profile-picture > img {
  border-radius: 12px;
  box-shadow: 0px 2px 8px 6px #00000070;
}

.title {
  margin-top: 72px;
	font-size: 42pt;
  text-align: center;
  font-family: 'Dancing Script', cursive;
}
.socials {
  margin-top: 48px;
}
.socials-icons {
  display: flex;
  justify-content: center;
  gap: 28px;
}
.projects {
  margin-top: 128px;
}
.projects-title {
  font-size: 26pt;
  text-align: center;
}
.projects-list {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 42px;
}
@media only screen and (max-width: 600px) {
  .project-item {
    width: 320px;
  }
}
@media only screen and (min-width: 600px) {
  .project-item {
    width: 540px;
  }
}
@media only screen and (min-width: 1200px) {
  .project-item {
    width: 780px;
  }
}
.project-item-title {
  font-size: 14pt;
}
</style>
