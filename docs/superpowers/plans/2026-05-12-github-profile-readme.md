# GitHub Profile README Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a complete, professional, story-driven GitHub profile README for Vivek Jivani that attracts freelance clients and full-time employers.

**Architecture:** Single `README.md` file built section by section. Uses GitHub-flavored Markdown with inline HTML tables for layout (CSS is stripped by GitHub). All visual elements (badges, stats, typing animation) are hotlinked external images from shields.io, readme-typing-svg, and github-readme-stats — no local assets.

**Tech Stack:** GitHub Flavored Markdown · HTML tables · shields.io · readme-typing-svg.demolab.com · github-readme-stats.vercel.app · streak-stats.demolab.com

---

## File Structure

| File | Action | Purpose |
|---|---|---|
| `README.md` | Rewrite | GitHub profile page — the only deliverable |

---

## Task 1: Header Section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Open README.md in VS Code and enable Markdown Preview**

  Open the file, then press `Ctrl+Shift+V` to open the side-by-side preview. Keep it open for all tasks.

- [ ] **Step 2: Write the header section**

  Replace the entire contents of `README.md` with:

  ````markdown
  <div align="center">

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=30&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&width=700&lines=Hey%2C+I'm+Vivek+Jivani+%F0%9F%91%8B;Full+Stack+Engineer+%26+Architect;Building+things+that+actually+work" alt="Typing SVG" />

  <p>Full Stack Engineer & Architect &nbsp;·&nbsp; Surat, India 🇮🇳</p>

  [![Open to Freelance](https://img.shields.io/badge/%E2%9A%A1_Open_to_Freelance-blue?style=for-the-badge)](https://vivekjivani.com)
  [![Available Now](https://img.shields.io/badge/%E2%9C%85_Available_Now-success?style=for-the-badge)](mailto:vivekjivani17@gmail.com)
  [![Remote Worldwide](https://img.shields.io/badge/%F0%9F%8C%8D_Remote_Worldwide-purple?style=for-the-badge)](https://vivekjivani.com)

  <br/>

  <p><em>I build things that <strong>actually work</strong> — end-to-end products from design to deployment, across web and mobile.</em></p>

  <br/>

  [![Portfolio](https://img.shields.io/badge/🌐_Portfolio-vivekjivani.com-58a6ff?style=flat-square)](https://vivekjivani.com)&nbsp;
  [![LinkedIn](https://img.shields.io/badge/💼_LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/viekjivani)&nbsp;
  [![Email](https://img.shields.io/badge/📧_Email-contact-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:vivekjivani17@gmail.com)

  </div>
  ````

  > **Note:** Verify the LinkedIn URL `linkedin.com/in/viekjivani` is correct by visiting it in a browser. If the correct slug is different, update it now.

- [ ] **Step 3: Verify in VS Code preview**

  Check the preview panel. You should see:
  - A centered block with a blue animated typing text (may not animate in VS Code preview — that's fine, it will on GitHub)
  - Subtitle line with location
  - Three colored `for-the-badge` pills (blue, green, purple)
  - Three smaller flat-square link badges below

- [ ] **Step 4: Commit**

  ```bash
  git add README.md
  git commit -m "feat: add header section to GitHub profile README"
  ```

---

## Task 2: About Me Section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append the About Me section**

  Open `README.md` and append the following after the last line:

  ````markdown

  ---

  ## 🧑‍💻 About Me

  <table>
    <tr>
      <td width="50%" valign="top">
        🏗️ &nbsp;<strong>6+ years</strong> shipping production apps — from B2B diamond trading platforms to cloud-native data automation tools
      </td>
      <td width="50%" valign="top">
        📱 &nbsp;Comfortable across <strong>Flutter mobile</strong> and <strong>Next.js / React web</strong> — one engineer, full product
      </td>
    </tr>
    <tr>
      <td valign="top">
        🤖 &nbsp;AI-powered workflow — I use <strong>Claude &amp; Gemini</strong> daily for architecture, code review, and debugging
      </td>
      <td valign="top">
        🚀 &nbsp;Last big win: architected a serverless platform that delivered a <strong>70% productivity boost</strong> at Nexsales
      </td>
    </tr>
  </table>
  ````

- [ ] **Step 2: Verify in VS Code preview**

  Check the preview. You should see:
  - A horizontal rule divider
  - A `## 🧑‍💻 About Me` heading
  - A two-column HTML table with four info items, two per row

- [ ] **Step 3: Commit**

  ```bash
  git add README.md
  git commit -m "feat: add About Me section to GitHub profile README"
  ```

---

## Task 3: Tech Stack Section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append the Tech Stack section**

  Append the following after the last line of `README.md`:

  ````markdown

  ---

  ## 🛠️ Tech Stack

  **📱 Mobile**

  ![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)

  **🌐 Frontend**

  ![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
  ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
  ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
  ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

  **⚙️ Backend**

  ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
  ![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)

  **🗄️ Databases**

  ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
  ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
  ![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

  **☁️ DevOps & Cloud**

  ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
  ![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
  ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

  **🤖 AI Tools**

  ![Claude](https://img.shields.io/badge/Claude-CC785C?style=for-the-badge&logo=anthropic&logoColor=white)
  ![Gemini](https://img.shields.io/badge/Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)
  ````

- [ ] **Step 2: Verify in VS Code preview**

  Check the preview. You should see:
  - Six bold group labels (Mobile, Frontend, Backend, Databases, DevOps & Cloud, AI Tools)
  - Colored rectangular badge images under each group
  - Badges may appear as broken images in VS Code preview if it blocks external URLs — this is expected; they will render on GitHub

- [ ] **Step 3: Commit**

  ```bash
  git add README.md
  git commit -m "feat: add Tech Stack section to GitHub profile README"
  ```

---

## Task 4: Featured Projects Section

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append the Featured Projects section**

  Append the following after the last line of `README.md`:

  ````markdown

  ---

  ## 🚀 Featured Projects

  <table>
    <tr>
      <td width="50%" valign="top">
        <h3>⚡ Goldmine</h3>
        <em>Data Automation Platform</em>
        <br/><br/>
        Serverless data automation platform that achieved a <strong>70% productivity boost</strong> and <strong>60% cost reduction</strong> through containerized microservices and intelligent workflow orchestration.
        <br/><br/>
        <code>Node.js</code> <code>Docker</code> <code>Serverless</code> <code>PostgreSQL</code>
      </td>
      <td width="50%" valign="top">
        <h3>💎 Craft Diamonds</h3>
        <em>Flutter · iOS & Android</em>
        <br/><br/>
        B2B diamond trading platform — real-time inventory browsing and order management for gem traders on the go.
        <br/><br/>
        <code>Flutter</code> <code>Firebase</code> <code>Node.js</code> <code>B2B</code>
        <br/><br/>
        <a href="https://play.google.com/store/apps/details?id=co.craftdiamonds.app">▶ Play Store</a>
      </td>
    </tr>
    <tr>
      <td width="50%" valign="top">
        <h3>📞 VoiceReach Dialer</h3>
        <em>Cloud Sales Platform</em>
        <br/><br/>
        Cloud-native sales dialer — contributed core features and led Docker-based containerization strategy for scale.
        <br/><br/>
        <code>Node.js</code> <code>Docker</code> <code>GCP</code> <code>REST API</code>
        <br/><br/>
        <a href="https://voicereach.us">🌐 Live</a>
      </td>
      <td width="50%" valign="top">
        <h3>🧾 GST Tools</h3>
        <em>Flutter · Tax Utility App</em>
        <br/><br/>
        Handy GST calculation and filing utility for Indian businesses — offline-first approach, fast lookups, and a clean UI that simplifies tax compliance.
        <br/><br/>
        <code>Flutter</code> <code>Firebase</code> <code>Offline-first</code>
        <br/><br/>
        <a href="https://play.google.com/store/apps/details?id=in.codetailor.gstutils">▶ Play Store</a>
      </td>
    </tr>
    <tr>
      <td width="50%" valign="top">
        <h3>🌸 Reiki Surat</h3>
        <em>Freelance · Wellness Center Website</em>
        <br/><br/>
        Professional website for a wellness and healing center — calming design, service listings, and an easy appointment contact flow.
        <br/><br/>
        <code>HTML/CSS</code> <code>JavaScript</code>
        <br/><br/>
        <a href="https://reikisurat.in">🌐 Live</a>
      </td>
      <td width="50%" valign="top">
        <h3>🦷 Varni Dental Care</h3>
        <em>Freelance · Dental Clinic Website</em>
        <br/><br/>
        Clean, trustworthy website for a dental clinic — service showcase, patient-friendly UX, and a local SEO-ready structure.
        <br/><br/>
        <code>HTML/CSS</code> <code>JavaScript</code>
        <br/><br/>
        <a href="https://varnidentalcare.in">🌐 Live</a>
      </td>
    </tr>
  </table>
  ````

- [ ] **Step 2: Verify in VS Code preview**

  Check the preview. You should see:
  - A `## 🚀 Featured Projects` heading
  - An HTML table with three rows and two columns
  - Each cell has a project name heading, italic type label, description, code tags, and a link where applicable

- [ ] **Step 3: Commit**

  ```bash
  git add README.md
  git commit -m "feat: add Featured Projects section to GitHub profile README"
  ```

---

## Task 5: GitHub Stats + Contact + Footer

**Files:**
- Modify: `README.md`

- [ ] **Step 1: Append the Stats, Contact, and Footer sections**

  Append the following after the last line of `README.md`:

  ````markdown

  ---

  ## 📊 GitHub Stats

  <div align="center">

  <table>
    <tr>
      <td>
        <img src="https://github-readme-stats.vercel.app/api?username=vivekjivani&show_icons=true&theme=github_dark&hide_border=true&count_private=true" alt="Vivek's GitHub Stats" />
      </td>
      <td>
        <img src="https://streak-stats.demolab.com?user=vivekjivani&theme=github-dark-blue&hide_border=true" alt="GitHub Streak" />
      </td>
    </tr>
    <tr>
      <td colspan="2" align="center">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=vivekjivani&layout=compact&theme=github_dark&hide_border=true" alt="Top Languages" />
      </td>
    </tr>
  </table>

  </div>

  ---

  ## 🤝 Let's Work Together

  <div align="center">

  <table>
    <tr>
      <td align="center" width="33%">
        🌐
        <br/>
        <strong>Portfolio</strong>
        <br/>
        <a href="https://vivekjivani.com">vivekjivani.com</a>
      </td>
      <td align="center" width="33%">
        💼
        <br/>
        <strong>LinkedIn</strong>
        <br/>
        <a href="https://linkedin.com/in/viekjivani">in/viekjivani</a>
      </td>
      <td align="center" width="33%">
        📧
        <br/>
        <strong>Email</strong>
        <br/>
        <a href="mailto:vivekjivani17@gmail.com">vivekjivani17@gmail.com</a>
      </td>
    </tr>
  </table>

  <br/>

  *Open to **freelance projects** and **full-time roles** — remote worldwide 🌍*

  <br/>

  <sub>⚡ Powered by coffee, curiosity, and a solid Wi-Fi connection</sub>

  </div>
  ````

- [ ] **Step 2: Verify in VS Code preview**

  Check the preview. You should see:
  - A `## 📊 GitHub Stats` heading with a centered two-row image table (images may not load in VS Code — expected)
  - A `## 🤝 Let's Work Together` heading with a three-column contact table
  - A centered italic line about freelance/full-time availability
  - A small footer tagline

- [ ] **Step 3: Commit**

  ```bash
  git add README.md
  git commit -m "feat: add GitHub Stats, contact, and footer to GitHub profile README"
  ```

---

## Task 6: Push and Verify on GitHub

**Files:**
- No file changes — verification only

- [ ] **Step 1: Push to GitHub**

  ```bash
  git push origin master
  ```

  > **Important:** This repo must be named `vivekjivani` (same as your GitHub username) for the profile README to appear. If it's named differently, rename it in GitHub Settings → Repository name → `vivekjivani`.

- [ ] **Step 2: Open your GitHub profile**

  Visit `https://github.com/vivekjivani` in a browser. The README should render on your profile page.

- [ ] **Step 3: Check each section**

  Walk through this checklist on the live profile:

  - [ ] Typing animation plays in the header
  - [ ] All three status badges (Freelance / Available / Remote) are visible
  - [ ] Tagline and social link badges appear below the subtitle
  - [ ] About Me table renders as two columns, not a broken HTML block
  - [ ] All tech stack badge images load with correct colors and logos
  - [ ] Projects table renders 3 rows × 2 columns cleanly
  - [ ] Play Store links for Craft Diamonds and GST Tools are clickable
  - [ ] VoiceReach and website links open correctly
  - [ ] GitHub Stats, Streak, and Top Languages widgets load (may take 5–10 seconds)
  - [ ] Contact table shows three columns with working links
  - [ ] Footer tagline is centered and readable

- [ ] **Step 4: Fix any rendering issues**

  Common GitHub rendering quirks to watch for:
  - If HTML table columns collapse: add explicit `width="50%"` to `<td>` elements (already included)
  - If stats widgets show "not found": wait 5 minutes and hard-refresh — the service caches on first hit
  - If badge images are broken: visit the shield URL directly to confirm it's valid

  No commit needed if no changes were required. If fixes were made:

  ```bash
  git add README.md
  git commit -m "fix: adjust README rendering for GitHub profile"
  git push origin master
  ```
