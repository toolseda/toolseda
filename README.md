> [!IMPORTANT]
> **DEMONSTRATION PROFILE:** This README is a reference example for **Dev Academy Aotearoa** students. It illustrates how to present technical skills, group collaboration, and personal projects to industry recruiters.

>[!Note]
> <details>
>  <summary>📎Pinned Repositories & Forking</summary>
>  
>  ### 👤 Individual clones
>  To follow industry best practices and keep your profile professional, the projects pinned below are **individual clones or clean repositories** rather than simple forks.
>  * **Why not just fork?** During bootcamp, group projects usually live in the shared organization. Forking them to your profile often brings unnecessary commit history and prevents you from easily customizing the README or adding individual features later.
>  * **The Best Practice:** We recommend creating a new repository on your personal account and pushing the code there. This allows you to:
>    1.  Own the repository and show up in your "Top Repositories" list.
>    2.  Write a personalized README that highlights *your* specific contributions.
>    3.  Continue developing the project independently to show post-bootcamp growth.
>        
>  ### 🌐 Open Source & The "Good" Fork
>  While we avoid forking for bootcamp work, **forking is the essential first step for Open Source contributions.**
>  * **When to fork:** If you are contributing a bug fix or feature to a public library (like Vite, React, or a local community tool), you *should* fork the repository. 
>  * **Suitability:** A fork on your profile is highly "suitable" when it is followed by a **Pull Request** to the original project. It shows you can navigate large codebases and contribute to the wider ecosystem.
>
> </details>

> [!Tip]
> **Cloning:** Creating your own individual clone
>
> <details>
>  <summary>🛠️ Git Guide: Moving to Your Personal Profile</summary>
>
> This guide walks you through transitioning a project from a shared organization (like a bootcamp repo) to your personal GitHub profile. This process turns a group project into a "portfolio piece" while respecting the work of your teammates.
>  
>  ---
>  
>  ## 🏗️ Step 1: Create the Destination
>  Before touching the terminal, you need a place for the code to land.
>  
>  1.  Go to your GitHub profile and click **New Repository**.
>  2.  **Name it** something that reflects the project (e.g., `community-toolshed`).
>  3.  **Keep it Empty:** Do not check the boxes for "Add a README" or "Add a .gitignore." You already have these files!
>  4.  Copy the **SSH URL** (it looks like `git@github.com:your-username/repo-name.git`).
>  
>  ---
>  
>  ## 🛰️ Step 2: Redirecting the Remote
>  Right now, your local folder thinks its "home" is the bootcamp organization. We need to tell it that its new home is your personal profile.
>  
>  [Image of git architecture showing a local repository connecting to an origin remote and an upstream remote]
>  
>  1.  **Open your terminal** in the project folder.
>  2.  **Rename the old link:** Instead of deleting the bootcamp link, rename it to `upstream`. This respects the project's roots and keeps a reference to the original source and your teammates' contributions.
>      ```bash
>      git remote rename origin upstream
>      ```
>  3.  **Add your new link:** Now, set your personal repo as the new `origin`.
>      ```bash
>      git remote add origin <PASTE_YOUR_COPIED_URL_HERE>
>      ```
>  4.  **Verify:** Check that both are listed correctly.
>      ```bash
>      git remote -v
>      ```
>  
>  ---
>  
>  ## 🛠️ Step 3: Choose Your History Strategy
>  You have two ways to proceed. Both are valid; choose the one that fits your goals for this project.
>  
>  ### Option A: Preserve the Collaboration (Recommended)
>  If you want to show recruiters how you worked with your team, keep the full history. It provides a transparent look at your journey, your fixes, and how you interacted with others' code.
>  ```bash
>  git push -u origin main
>  ```
>  
>  ### Option B: The "Clean Slate" (Optional)
>  If you intend to work on this project extensively as a solo venture—refactoring the code, adding major features, or changing the tech stack—you might want a clean starting point. This treats the bootcamp version as a "Version 1.0" foundation.
>  
>  > [!NOTE]
>  > Only use this if you want to start a fresh development chapter for this repository.
>  
>  1.  **Create a clean branch:**
>      ```bash
>      git checkout --orphan temp_branch
>      ```
>  2.  **Stage all your files:**
>      ```bash
>      git add -A
>      ```
>  3.  **Create your new starting point:**
>      ```bash
>      git commit -m "Initial commit: Base project established from [Project Name]"
>      ```
>  4.  **Swap the branches and push:**
>      ```bash
>      git branch -D main
>      git branch -m main
>      git push -f origin main
>      ```
>  
>  ---
>  
>  ## 💡 Pro-Tips for Success
>  * **Respect the Craft:** Keeping the original history acknowledges the contributions of your peers. It shows you value the collaborative process.
>  * **Intentionality:** If you choose to squash, framing it as "the start of a new development phase" tells recruiters you have a plan for the project's future.
>  * **Give Credit:** Regardless of the method, your README should still link back to the original group project or the Dev Academy organization to give credit where it's due.

> </details>

---

# ✨ Hi, I'm Tools

I’m a passionate **Full Stack Web Developer** based in Wellington, New Zealand. I specialize in building functional, community-focused applications using **React, TypeScript, Node.js, and Relational Databases**.

I prioritize writing clean, readable code and focus on delivering small, complete projects that solve real-world problems.

---

## 📈 About Me
I recently graduated from an intensive 17-week bootcamp at Dev Academy. My approach to development is centered on **Agile methodologies** and collaborative problem-solving. I love the "aha!" moment when a complex backend logic finally connects seamlessly with a polished frontend.

* **My Philosophy:** Keep it simple, make it accessible, and always consider the person who will be reading my code next.
* **Personal Interests:** When I’m not at my desk, you’ll find me in Mākara Peak and Mt Vic. exploring the bike trails. I’m also a big gaming enthusiast, which originally sparked my curiosity about how software is built.

---

## 📂 Featured Projects

### 🏗️ [ToolShed](https://github.com/toolseda/ToolShed) (Group Project)
**Why we built this:** Our team wanted to tackle the inefficiency of household waste. We built ToolShed to facilitate a "circular economy," allowing neighbors to list and borrow tools.
* **My Role:** I led the **Backend API development** and Database architecture. I was responsible for ensuring the relational logic between "Owners" and "Borrowers" remained intact across the app.
* **Tech:** React, Redux, Express, Knex, SQLite3.
* **The "Why":** This project demonstrated my ability to work in a high-velocity team, manage complex merge conflicts, and use Kanban boards to hit deadlines.

### 🚵 [CycleSnap](https://github.com/toolseda/CycleSnap)
**Why I built this:** As a rider, I found that weather apps didn't tell the whole story of trail conditions. I built this micro-blog so riders could share real-time updates and gear recommendations.
* **Tech:** React, Tailwind CSS, Express, Multer for image handling.
* **The "Why":** I wanted to master **CRUD operations** and external file storage. It taught me how to handle asynchronous data fetching while maintaining a smooth user experience.

### 🧪 [RoastRef](https://github.com/toolseda/RoastRef)
**Why I built this:** To move beyond generic "To-Do" list tutorials, I created a specialized coffee tasting journal.
* **Tech:** React, Material-UI, Express, SQLite3.
* **The "Why":** I used this project to deep-dive into **complex form state management** and custom UI components (like a dynamic tasting wheel). It shows my attention to detail in UX/UI.

---

## 🛠️ Tech Stack
- **Frontend:** React, TypeScript, Redux, Tailwind CSS, Material-UI
- **Backend:** Node.js, Express, Knex, SQLite3
- **Testing/Tools:** Vitest, ESLint, Git, GitHub (Agile Workflow), Vite
- **Deployment:** Render, Vercel

---

## 📈 Currently Working On
- 👥 Adding a real-time messaging system to **ToolShed** for user coordination.
- 🌲 Integrating a Map API into **CycleSnap** to pin trail locations.
- 🔍 Actively seeking a Junior Developer role where I can contribute to a collaborative team.

---

## 🤝 Let's Connect
- [🛠️ LinkedIn](https://linkedin.com/in/your-profile)
- [🌐 Portfolio](https://your-portfolio-site.com)
- [📂 GitHub](https://github.com/your-username)
