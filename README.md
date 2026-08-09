<!-- GitHub Profile README — Bino Hlongwana | github.com/Robotbino -->

<h1 align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Atkinson+Hyperlegible&size=28&pause=1000&color=DFB11C&center=true&vCenter=true&width=435&lines=Hi%2C+my+name+is+Bino;Software+Developer+%7C+Musician;Curious+about+things+%3A+)" alt="Hi, my name is Bino — Software Developer | Musician" />
</h1>

## About Me

I write enterprise Java web applications during the day, the kind with long-lived business rules, workflow engines and a QA process behind every release. After hours I build the other half of the stack: Spring Boot APIs and Angular/React front ends.

That split is deliberate. Work taught me how software survives in production. My own projects are where I go deep on the modern stack, stateless JWT auth, Angular Signals, WebGL and then write down *why* I chose what I chose.

- 🎓 BSc Information Technology, North-West University (2023)
- 📜 IBM AI Fundamentals · Anthropic Claude 101 & Claude Code 101 · Scrimba JavaScript & HTML/CSS
- 🕹️ Side quests: producing music, soccer, reading, and far too much anime 🗡️
- 🐍 The snake at the bottom of this page eats my commit history. Stick around for it.

## Connect With Me

<p>
  <a href="https://www.linkedin.com/in/bino-hlongwana-162226272" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:Hlongwanabino@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://binohlongwana.netlify.app/" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-DFB11C?style=for-the-badge&logo=firefoxbrowser&logoColor=black" alt="Portfolio" />
  </a>
</p> 

---


## Tech & Tools

<b>Languages</b>
<br/>
<a href="https://skillicons.dev"><img height="40" src="https://skillicons.dev/icons?i=java,python,ts,js" alt="Java, Python, TypeScript, JavaScript" /></a>
<br/><br/>

<b> Frontend</b>
<br/>
<a href="https://skillicons.dev"><img height="40" src="https://skillicons.dev/icons?i=angular,react,html,css,bootstrap" alt="Angular, React, HTML5, CSS3, Bootstrap" /></a>
<br/><br/>

<b> Backend &amp; Database</b>
<br/>
<a href="https://skillicons.dev"><img height="40" src="https://skillicons.dev/icons?i=spring,mysql" alt="Spring Boot, MySQL" /></a>
<br/>
<sub>➕ Spring Security · JWT</sub>
<br/><br/>

<b>🛠️ Tools &amp; Platforms</b>
<br/>
<a href="https://skillicons.dev"><img height="40" src="https://skillicons.dev/icons?i=git,github,postman,maven,idea,vscode,docker,netlify" alt="Git, GitHub, Postman, Maven, IntelliJ IDEA, VS Code, Docker, Netlify" /></a>


---

## 📂 Featured Projects

| Project | What it is | Links |
| :--- | :--- | :--- |
| **🎮 GameStore** | Game storefront + admin portal on a secured Spring Boot API | [Backend](https://github.com/Robotbino/gameStore-backend) · [Frontend](https://github.com/Robotbino/gameStore) |
| **👔 Employee Management System** | Stateless JWT auth done properly across an API and an Angular client | [Backend](https://github.com/Robotbino/EmployeeManager-Application) · [Frontend](https://github.com/Robotbino/EmployeeManager-Application-Frontend) |
| **🃏 Code Pairs** | Memory game rebuilt on Angular standalone components + Signals | [Repo](https://github.com/Robotbino/CodePairs) · [Live](https://codepairsgame.netlify.app/) |
| **🌌 Personal Portfolio** | One looping scroll over a WebGL aurora — no router, ADR-documented | [Repo](https://github.com/Robotbino/PorfolioWebsite) · [Live](https://binohlongwana.netlify.app/) |

<br/>

### 🎮 GameStore: storefront and admin portal, end to end

Started as a React UI exercise. I kept asking what an actual store needs behind the pretty grid, and it turned into a full-stack MVP.

- **Two audiences, one API.** Customers register, search the catalogue live, open game detail pages and build a personal library. Admins get a separate portal with full CRUD over games and users.
- **Security is the backbone, not a bolt-on.** Spring Security with JWT bearer tokens, USER/ADMIN role separation, and fully stateless sessions — no server-side session state to scale around.
- **Documented like a system, not a demo.** The request flow, auth handshake and data model are drawn out as Mermaid diagrams in the repo, so a reviewer can understand the architecture without reading every class.

<p>
  <img src="https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React 19" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" alt="Spring Security" />
  <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL" />
</p>

🔗 [Backend](https://github.com/Robotbino/gameStore-backend) · [Frontend](https://github.com/Robotbino/gameStore)

---

### 👔 Employee Management System: stateless auth across two apps

Plenty of tutorials stop at "login works". I built this one to find out where token-based auth actually leaks: the seam between an API that trusts nothing and a client that has to remember everything.

- **Java 17 / Spring Boot REST API** over employee records — CRUD, validation, and a Spring Security 6 filter chain that issues and verifies JWTs on every request.
- **The Angular side holds up its end.** An HTTP interceptor attaches the token to outbound calls; route guards keep protected routes protected instead of just hiding the nav link.
- **Ships with an architecture and MVP roadmap doc** — scope, data model, and what deliberately got left for v2.

<p>
  <img src="https://img.shields.io/badge/Java_17-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java 17" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/Spring_Security_6-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" alt="Spring Security 6" />
  <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular" />
</p>

🔗 [Backend](https://github.com/Robotbino/EmployeeManager-Application) · [Frontend](https://github.com/Robotbino/EmployeeManager-Application-Frontend)

---

### 🃏 Code Pairs: a memory game, rebuilt to learn Signals

A code-themed card matching game that I tore down and rebuilt on Angular's standalone components and Signals — the rewrite was the point.

- **Game state as derived state.** Score, remaining attempts and win conditions fall out of signals instead of manual change-detection wrangling, which killed a whole class of stale-UI bugs.
- **Difficulty tiers** change the grid size and the attempt budget, so the rules live in one place rather than scattered across components.
- **Brutalist visual language** with 3D CSS flip animations — no animation library, just transforms and `backface-visibility`.

<p>
  <img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular" />
  <img src="https://img.shields.io/badge/Signals-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular Signals" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3" />
</p>

🔗 [Repository](https://github.com/Robotbino/CodePairs) · [Live Demo](https://codepairsgame.netlify.app/)

---

### 🌌 Personal Portfolio: an cool Awwwards.com themed site

I didn't want a résumé with a nav bar, that's boring. This one is a single continuous scroll: five destinations that wrap into a seamless loop, floating over a WebGL aurora.

- **No router.** The whole site is one scroll loop with a cloned first section at the end, so reaching the bottom wraps back to the top without a jump or a route change.
- **WebGL aurora shader** rendered with OGL, plus a constellation that morphs between the four route shapes as you travel — driven by a shared viewport-observer service rather than a dozen loose IntersectionObservers.
- **Every real decision is an ADR.** Eight of them so far, covering the loop wrap, nav muting and surface treatment. The repo also ships an interactive onboarding guide for anyone reading the code cold.

<p>
  <img src="https://img.shields.io/badge/Angular_19-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular 19" />
  <img src="https://img.shields.io/badge/Signals-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular Signals" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/OGL_(WebGL)-000000?style=flat-square&logo=webgl&logoColor=white" alt="OGL WebGL" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3" />
</p>

🔗 [Repository](https://github.com/Robotbino/PorfolioWebsite) · [Live Demo](https://binohlongwana.netlify.app/)

---

## GitHub Activity

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Robotbino&theme=github-dark&hide_border=true" alt="Contribution activity graph" />
</p>

## Contribution Snake

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Robotbino/Robotbino/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Robotbino/Robotbino/output/github-contribution-grid-snake.svg" />
    <img src="https://raw.githubusercontent.com/Robotbino/Robotbino/output/github-contribution-grid-snake.svg" alt="Contribution snake animation" />
  </picture>
</p>
