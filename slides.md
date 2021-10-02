---
# try also 'default' to start simple
theme: seriph
layout: cover
background: https://images.unsplash.com/photo-1619017120498-872bb10a14a6?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1170&q=80
# apply any windi css classes to the current slide

class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
---

<style>

</style>

## League Client Architecture

Presentation slides for developers

<!-- <div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div> -->

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
layout: image-right
image: https://scontent.fcgh7-1.fna.fbcdn.net/v/t1.6435-9/118209405_3238693856220911_8155388593582273315_n.jpg?_nc_cat=108&ccb=1-5&_nc_sid=174925&_nc_eui2=AeGK8s9NLpl-D0r_NnJuirOe4SPjmkfap1zhI-OaR9qnXKpGdtU7vEK-jEBxExNOsbnzATeyEIgbs42WLnkkj_CM&_nc_ohc=f9LZwUYqGHoAX-REt5L&_nc_ht=scontent.fcgh7-1.fna&oh=db3efb27ded556adcfb67cfff8e22702&oe=617DFDA4
---

# Sobre mim

- Desenvolvedora front-end há 4 anos
- Graduação em ADS pelo IFSP
- Membro da He4rt desde 2018
- Jogadora de League of Legends desde 2014
- Amante de arte, gatos e tecnologia

---

# Como funciona o Client?

As tecnologias do client podem ser dividas entre 2 áreas, cliente e servidor.

![image info](https://techenter.com.br/wp-content/uploads/2019/01/cliente-servidor.png)

<br>
<br>
<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-size: 100%;
  text-align: center;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent; 
  -moz-text-fill-color: transparent;
}
  
  p {
  	text-align: center;
  }
  
  img {
  	height: 400px;
    position: absolute;
    right: 20%;
  }
</style>


---
layout: image-right
image: https://pm1.narvii.com/6454/56332de132336a4d8237207605cb30a752394232_hq.jpg
---

# Arquitetura

Client 2009

- Adobe Air
- Flash
- RTMP



---
layout: image-left
image: >-
  https://www.pcgamesn.com/wp-content/uploads/2020/11/league-of-legends-battle-queen-janna.jpg
---

# Mudanças

Em 2016 a Riot decidiu de vez migrar seu client para uma solução mais leve, a qual iria resolver boa parte de seus problemas, entre eles:

- Aposentadoria do Flash
- Os players querem estar conectados dentro e fora do jogo
- Facilidade e autonomia de desenvolvimento para os novos devs


---

# Arquitetura

Client 2016

- HTML e Javascript
- Ember.js
- Chromium Embedded Framework (CEF)
- C++ Microservices para utilizar o RMTP
- Websockets


<img src='https://technology.riotgames.com/sites/default/files/lcu_architecture_4.png' />


<style>
  img {
  	position: absolute;
    right: 5%;
    top: 10%;
    height: 460px;
    width: 500px;
    border-radius: 4px;
    filter: drop-shadow(0 0 0.55rem black);
  }
</style>


---
class: px-20
---

<h1>Por que o Client Buga tanto?</h1>

<img src='https://media3.giphy.com/media/l2Sq2Iw6xwrlzrLs4/giphy.gif?cid=ecf05e47pvvgf294tnpkdy31extkku2ufvo1cigj1govnj32&rid=giphy.gif&ct=g' />

<style>
  h1 {
    position: absolute;
    top: 55%;
    color: #990000;
    left: 25%;
    
  }
  
  img {
  	height: 250px;
    position: absolute;
    top: 5%;
    left: 36%;
  }
</style>


---
preload: false
---

# Melhorias
de 2020 até 2021

- Feedbacks globais
- Conseguimos reduzir o tempo de iniciação do cliente a 16 segundos para 90% das pessoas que jogam no mundo todo (a média era de 29,5 segundos no início de 2020).
- Resolvemos o problema que fazia com que o cliente travasse completamente e deixasse as pessoas em uma tela preta após o fim de uma partida.
- Reduzimos o tempo de carregamento da aba Runas em 40% e tornamos a interface das Runas mais leve e confiável.
- Atualização do Chromium Embedded Framework (CEF)
- Redução de travamentos do cliente
- Desempenho WebSocket mais rápido
- Melhor uso de CPU


---

# O que esperar do futuro?

<img src='https://media3.giphy.com/media/lqut5VxPEhP9zCJdUT/giphy.gif?cid=ecf05e475fy23ri8qrkb0860p9k5gcx3w33z2pcw4iyf8cjd&rid=giphy.gif&ct=g' />


<style>
  h1 {
    text-align: center;
  }
  
  img {
  	position: absolute;
    right: 32%;
  }
</style>


---
layout: image-right
image: https://www.hotspawn.com/app/uploads/2021/05/Beta-Key-Art_VALORANT-1.jpg
---

# "A melhor experiência de cliente na nossa visão"

- Não ter que baixar ou instalar manualmente nada de novo para fazer as atualizações. 
- Sempre ter acesso a notícias, atualizações e informações relevantes. 	
- Poder acessar o jogo diretamente (e penar bastante para sair do Prata).


---

# Referências

- THE ARCHITECTURE OF THE LEAGUE CLIENT UPDATE: https://technology.riotgames.com/news/architecture-league-client-update

- Descobrimos as Tecnologias por trás do League of Legends - Canal Código Fonte TV: https://www.youtube.com/watch?v=AJHtok_qIvE&t=306s&ab_channel=C%C3%B3digoFonteTV

- Riot Promete Melhorias No Client Em Seis Meses: https://www.pichauarena.com.br/lol/riot-promete-melhorias-no-client-em-seis-meses/

- LIMPEZA DO CLIENTE: RECAPITULAÇÃO DE 2020 E FUTURO     https://www.leagueoflegends.com/pt-br/news/dev/limpeza-do-cliente-recapitulacao-de-2020-e-futuro/

- LIMPEZA DO CLIENTE: 2021 E O QUE VEM POR AÍ https://leagueoflegends.com/pt-br/news/dev/limpeza-do-cliente-2021-e-o-que-vem-por-ai/

- Novo Client Riot Em breve: https://www.riotgames.com/pt-br/not%C3%ADcias/novo-cliente-riot-em-breve


---

# Obrigada!


<img src='https://media2.giphy.com/media/Vr3HlfDMnSllDmnNNh/giphy.gif?cid=790b76117cca821d4818dfe83275c017df44e850f774dc96&rid=giphy.gif&ct=g' class='seraphine' />


<div class='socials'>
	<img src='https://cdn-icons-png.flaticon.com/512/174/174857.png' />
  	<p>Anna Campelo</p>
	<img src='https://logodownload.org/wp-content/uploads/2014/09/twitter-logo-2-1.png' />
  	<p>@Annerland</p>
  	<img class='twitch' src='https://www.freepnglogos.com/uploads/twitch-app-logo-png-3.png' />
  	<p>@Annerland</p>
</div>

<style>
  .seraphine {
    height: 300px
 	position: absolute;
    /
  }
  img {
  	height: 30px;
    margin: 0 8px;
  }
  
  .twitch {
    margin: 0;
  }
  
  .socials {
  	display: flex;
    align-items: center;
    color: #808080;
    position: absolute;
    top: 80%;
  }
</style>
