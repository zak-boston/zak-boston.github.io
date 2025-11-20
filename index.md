---
---
layout: default
---

<div style="text-align:center; padding:7rem 2rem; background:linear-gradient(135deg, #0f0c29, #302b63, #24243e); margin:-2rem -2rem 5rem;">
  <h1 style="font-size:4.5rem; margin:0;">Zak Boston</h1>
  <p style="font-size:1.8rem; opacity:0.9; margin:1.5rem 0;">
    Data Scientist • Problem Solver • Builder of Things That Shouldn’t Work
  </p>
</div>

<div style="max-width:1200px; margin:0 auto; padding:0 2rem; display:grid; grid-template-columns: repeat(auto-fit, minmax(360px, 1fr)); gap:2.5rem;">

  <!-- Card 1: Project Euler -->
  <a href="/euler" style="text-decoration:none; color:inherit;">
    <div style="background:rgba(88,166,255,0.15); border-radius:16px; overflow:hidden; border:2px solid #58a6ff; transition:transform 0.3s; box-shadow:0 10px 30px rgba(0,0,0,0.3);" onmouseover="this.style.transform='translateY(-12px)'" onmouseout="this.style.transform='translateY(0)'">
      <div style="height:180px; background:linear-gradient(135deg, #58a6ff, #1e90ff); display:flex; align-items:center; justify-content:center;">
        <h2 style="font-size:4rem; margin:0; color:white; opacity:0.8;">π</h2>
      </div>
      <div style="padding:2rem;">
        <h3 style="margin:0 0 1rem; font-size:1.8rem; color:#58a6ff;">Project Euler Solutions</h3>
        <p style="opacity:0.8; line-height:1.6;">
          {{ site.posts.size }} elegant Python solutions to the hardest math + programming problems.
          Clean code, explanations, and performance notes.
        </p>
        <strong style="color:#58a6ff;">→ Explore all problems</strong>
      </div>
    </div>
  </a>

  <!-- Card 2: Python Games -->
  <a href="/games" style="text-decoration:none; color:inherit;">
    <div style="background:rgba(139,92,246,0.15); border-radius:16px; overflow:hidden; border:2px solid #8b5cf6; transition:transform 0.3s; box-shadow:0 10px 30px rgba(0,0,0,0.3);" onmouseover="this.style.transform='translateY(-12px)'" onmouseout="this.style.transform='translateY(0)'">
      <div style="height:180px; background:linear-gradient(135deg, #8b5cf6, #6366f1); display:flex; align-items:center; justify-content:center;">
        <h2 style="font-size:4rem; margin:0; color:white;">♜</h2>
      </div>
      <div style="padding:2rem;">
        <h3 style="margin:0 0 1rem; font-size:1.8rem; color:#c4b5fd;">Python Tkinter Games</h3>
        <p style="opacity:0.8; line-height:1.6;">
          Fully playable games built with nothing but Tkinter and Python — running right in your browser via Pyodide.
        </p>
        <strong style="color:#c4b5fd;">→ Play now</strong>
      </div>
    </div>
  </a>

  <!-- Card 3: NLP Projects -->
  <a href="/nlp" style="text-decoration:none; color:inherit;">
    <div style="background:rgba(34,197,94,0.15); border-radius:16px; overflow:hidden; border:2px solid #22c55e; transition:transform 0.3s; box-shadow:0 10px 30px rgba(0,0,0,0.3);" onmouseover="this.style.transform='translateY(-12px)'" onmouseout="this.style.transform='translateY(0)'">
      <div style="height:180px; background:linear-gradient(135deg, #22c55e, #16a34a); display:flex; align-items:center; justify-content:center;">
        <h2 style="font-size:4rem; margin:0; color:white;">✍</h2>
      </div>
      <div style="padding:2rem;">
        <h3 style="margin:0 0 1rem; font-size:1.8rem; color:#86efac;">NLP & Generative Projects</h3>
        <p style="opacity:0.8; line-height:1.6;">
          Haiku generator • Shakespeare sonnet writer • Pun machine • Markov chains gone wild.
        </p>
        <strong style="color:#86efac;">→ Generate something weird</strong>
      </div>
    </div>
  </a>

</div>