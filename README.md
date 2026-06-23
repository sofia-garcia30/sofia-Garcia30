
<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&duration=3000&pause=1000&color=36BCF7&center=true&vCenter=true&width=500&lines=Hola%2C+soy+Sofia+Garcia;Full+Stack+Developer+in+training;Backend+%7C+APIs+REST+%7C+Bases+de+datos" alt="Typing SVG" />
</p>

> **Hola, soy Sofia Garcia**  
> Aprendiz del programa Análisis y Desarrollo de Software y desarrolladora de software en formación. Me interesa especialmente el desarrollo backend, las APIs REST y las bases de datos. Actualmente fortalezco mis conocimientos en Java, Spring Boot, Angular y MySQL con el objetivo de crecer como desarrolladora Full Stack.

---

### > STACK_ARSENAL.exe

⚔️ **Backend**  
`Java` `Spring Boot` `JWT` `APIs REST`  `Python`

🛡️ **Frontend**  
`Angular` `TypeScript` `HTML5` `CSS3` `JavaScript`  

🗄️ **Database**  
`MySQL`  `MongoDB`

🐳 **DevOps & Herramientas**  
`Git` `GitHub` `Docker` `Postman` `Maven` `Railway` `Vercel` `GitLab` `Insomnia`

---

### > SKILLS_PROGRESS.log


text

---

### > CONTRIBUTION_SNAKE.exe

<!-- Snake animation: requiere un GitHub Action (ver instrucciones al final) -->
<source media="..." srcset="https://github.com/sofia-garcia30/sofia-garcia30/blob/output/github-contribution-grid-snake-dark.svg">
<source media="..." srcset="https://github.com/sofia-garcia30/sofia-garcia30/blob/output/github-contribution-grid-snake.svg">
<img alt="Snake animation" src="https://github.com/sofia-garcia30/sofia-garcia30/blob/output/github-contribution-grid-snake.svg">

---

### > PLAYER_STATS.rpg

| ⚔️ ATRIBUTO        | 📊 VALOR                                            |
|------------------- |-------------------------------------------           |
| 🎮 **Class**       | Desarrolladora Full Stack en formación               |
| ⭐ **Level**       | Aprendiz Avanzado                                    |
| 🎯 **Quest**       | Crecer profesionalmente y construir proyectos reales |
| 💪 **Habilidad**   | Aprender rápido y no rendirse                        |

---

### 📊 SKILL TREE

| Tecnología     | Nivel      | Progreso                   |
|----------------|------------|----------------------------|
| ☕ Java        | Avanzado   | ███████████████░ 80%      |
| 🌱 Spring Boot | Intermedio | ██████████████░░ 70%      |
| 🔺 Angular     | Intermedio | █████████████░░░ 60%      |
| 🐳 Docker      | Avanzado   | ███████████████░ 90%      |
| 🗄️ MySQL       | Intermedio | ████████████░░░░ 50%      |
| 🔧 Git/GitHub  | Activo     | ██████████████░░ 70%      |

---

### 🎯 > AREAS_DE_INTERES.txt

- Desarrollo Backend
- Arquitectura de Software
- APIs REST
- Bases de Datos Relacionales
- Desarrollo Full Stack
- Buenas prácticas de desarrollo

---

### 📚 > QUESTS_ACTIVAS.log
[EN PROGRESO] Diseño y arquitectura de aplicaciones
[EN PROGRESO] Integración entre frontend y backend
[EN PROGRESO] Optimización de consultas y bases de datos
[EN PROGRESO] Patrones y buenas prácticas de desarrollo
[EN PROGRESO] Desarrollo Full Stack

text

---

### 💡 > ABOUT_ME.txt

Disfruto comprender cómo funcionan los sistemas detrás de escena y enfrentar nuevos retos tecnológicos como oportunidades de aprendizaje. Busco seguir fortaleciendo mis habilidades técnicas y participar en proyectos que me permitan crecer profesionalmente como desarrolladora de software.

---

### > CONTACT.init

| Plataforma      | Enlace                                |
|-----------------|---------------------------------------|
| 📧 **Email**    | sgarcia30719@gmail.com                |
| 💼 **LinkedIn** | www.linkedin.com/in/sofia-g-991520339 |

name: Generate snake animation
on:
  schedule:
    - cron: "0 0 * * *"  # se ejecuta cada día
  workflow_dispatch:
  push:
    branches:
      - main
jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg?color_snake=#36BCF7&color_dots=#ebedf0,#9be9a8,#40c463,#30a14e,#216e39
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark&color_snake=#36BCF7
      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}