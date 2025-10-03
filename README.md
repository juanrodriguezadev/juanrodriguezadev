<!--
  GitHub Profile · Juan Diego Rodríguez
  Professional, clean, and visually engaging profile with custom banners and sections.
-->

<p align="center">
  <img src="./assets/header.svg" width="100%" alt="Juan Diego Rodríguez · Frontend Developer">
</p>

<p align="center">
  <a href="mailto:juanrodriguezadev@gmail.com"><strong>Email</strong></a> •
  <a href="https://www.linkedin.com/in/juanrodriguezadev/"><strong>LinkedIn</strong></a> •
  <a href="https://github.com/juanrodriguezadev"><strong>GitHub</strong></a>
</p>

<p align="center">
  <em>Clean Code · Great UX · Reliable Delivery</em>
</p>

<p align="center">
  <img src="./assets/separator.svg" width="70%" alt="">
</p>

<h3 align="center">Frontend Developer (Angular · TypeScript) — Remote Ready</h3>

<p align="center">
  Passionate about building <strong>scalable web applications</strong> using <strong>Angular</strong>, <strong>TypeScript</strong>, <strong>RxJS</strong>, <strong>Tailwind</strong>, and <strong>Hexagonal Architecture</strong>, with a strong focus on UX, performance, and maintainability.
</p>

---

## 🧭 About Me
- 🌎 Based in Colombia · Open to **remote opportunities (USD/EUR)**
- 💻 Main stack: **Angular (v10+), TypeScript, RxJS, TailwindCSS, Angular Material, Fuse**
- 🧱 Architectures: **Hexagonal · DDD · Clean Code**
- ☁️ Cloud/DevOps: **AWS (S3, basics) · CI/CD basics**
- 🤝 Enthusiastic about mentoring, code reviews, performance optimization, and developer experience

---

## 🛠 Tech Stack
<p>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" alt="Angular"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" alt="TypeScript"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/rxjs/rxjs-original.svg" alt="RxJS"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tailwindcss/tailwindcss-plain.svg" alt="TailwindCSS"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/materialui/materialui-original.svg" alt="Material UI"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-plain.svg" alt="Git"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub"/>
  <img height="32" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/amazonwebservices/amazonwebservices-original.svg" alt="AWS"/>
</p>

<p align="center">
  <img src="./assets/separator.svg" width="70%" alt="">
</p>

---

## 🚀 Featured Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Talent & Learning Platform</h3>
      <p>
        A complete talent management and learning platform built with <strong>Angular + Hexagonal Architecture</strong>.
        Includes modules for courses, learning paths, team management, and AI-powered chatbot.
      </p>
      <ul>
        <li>Clean structure: domain / ports / infrastructure</li>
        <li>Modern UI with Tailwind + Fuse</li>
        <li>Sections, resources with estimated time, drawers, drag & drop</li>
      </ul>
      <p><em>Private repository — demo screens available on request</em></p>
    </td>
    <td width="50%" valign="top">
      <h3>Knowledge Base Chatbot</h3>
      <p>
        Conversational chatbot interface with memory and <strong>citation insights</strong>.
        Shows expandable sources inline or via drawer depending on count.
      </p>
      <ul>
        <li>Organism “citation-viewer” with visual mapper</li>
        <li>Integration with OpenAPI backend · Multi-language support</li>
        <li>Focus on accessibility and smooth UX</li>
      </ul>
      <p><em>Private repository — demo screens available on request</em></p>
    </td>
  </tr>
</table>

<details>
<summary><strong>📂 More projects & case studies</strong></summary>

- **Learning Path View**: route builder with course cards, search, drag & drop ordering, and summary drawers.  
- **Chatbot Management**: complete module (component, infrastructure, ports, models, use cases) built in hexagonal style.  
- **Client Management**: paginated lists, create/edit flows, confirmation dialogs, and state management.  

</details>

<p align="center">
  <img src="./assets/separator.svg" width="70%" alt="">
</p>

---

## 🧪 Code Sample (Angular)
```ts
// Example: safe API call with RxJS, state handling & error management
loadCourses(): void {
  this.loading.set(true);
  this.courses$ = this.courseService.getCourses().pipe(
    finalize(() => this.loading.set(false)),
    catchError(err => {
      this.toast.error('Failed to load courses');
      return of([]);
    })
  );
}

