

# 💫 About Me:
 </>Hi, I am currently working on game development with Unity, android app development, ai, backend eb dev and also im a <br>Software Engineering student. I am trying to get professional with Rust, <br>C#, Java and C++.   </>   I have high proficiency of English, native Turkish and <br>low level of German. FunFacts : •Kinda good at Valorant (jk, depends on the day, mostly bad.)  


## 🌐 Socials:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/www.linkedin.com/in/beren-elçin-polat-078829245) 

# 💻 Tech Stack:
• IronSource Ad SDK <br>
• Opta-Widget (SportsWidgets) <br>
• LeanPlum SDK(Sets the userId for 1 time) <br>
• DOTween Lib <br>
• Unity Engine <br>
• C# <br>
• Java <br>
• OOP <br>
• C <br>
• C# Game Mechanics <br>
• Data Structures <br>
• Data Analysis <br>
• SQL <br>
• HTML/CSS


# 📊 GitHub Stats:
//![](https://github-readme-streak-stats.herokuapp.com/?user=berenpolat&theme=dark&hide_border=false)<br/>
# GitHub Action for generating a contribution graph with a snake eating your contributions.

name: Generate Snake

# Controls when the action will run. This action runs every 24 hours.

on:
  schedule:
    # every 24 hours
    - cron: "0 */24 * * *"

  # This command allows us to run the Action automatically from the Actions tab.
  workflow_dispatch:

  # On changes
  push:
    branches:
      - master

# The sequence of runs in this workflow:
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest
    permissions:
      contents: write
    timeout-minutes: 5
    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:

      # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2

      # Generates the snake
      - uses: Platane/snk/svg-only@v3
        id: snake-gif
        with:
          github_user_name: ${{ github.repository_owner }}
          # these next 2 lines generate the files on a branch called "output". This keeps the main branch from cluttering up.
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

      # show the status of the build. Makes it easier for debugging (if there's any issues).
      - run: git status

      # Push the images to the output branch
      - uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=berenpolat&theme=radical&no-frame=false&no-bg=true&margin-w=4)


### 🔝 Top Contributed Repo
![](https://github-contributor-stats.vercel.app/api?username=berenpolat&limit=5&theme=dark&combine_all_yearly_contributions=true)


---


