---
layout: default
---

<div class="sidebar">
  <h1>Hi, I'm Hilo 👋</h1>
  <p>Threat Detection · Incident Response · Security Monitoring</p>
  <p><strong>Portfolio Junior SOC Analyst - Open to work España/Remoto</strong> Aquí documento mi viaje por Sherlocks y máquinas.</p>
  <hr>
  <p><a href="https://github.com/morehilo/project_hub">GitHub</a> | <a href="#">LinkedIn</a> | <a href="#">CV</a></p>
</div>

<div class="content">
  <h2>Featured Write-up</h2>
  
  {% assign projects = "BFT,Brutus,Unit42,Noxious,PHP-CGI,Bumblebee" | split: "," %}
  {% assign links = "https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Very-Easy/BFT/BFT.md,https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Very-Easy/Brutus/Brutus.md,https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Very-Easy/Unit42/Unit42.md,https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Very-Easy/Noxious/Noxious.md,https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Easy/PHP-CGI_(CVE-2024-4577)/PHP-CGI_(CVE-2024-4577).md,https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Easy/Bumblebee/Bumblebee.md" | split: "," %}
  
  {% for project in projects %}
    {% assign index = forloop.index0 %}
    {% assign link = links[index] %}
    
    <div class="writeup-card">
      <h3>{{ project }}</h3>
      <span class="tag">Sherlock</span>
      <span class="tag">Forensics</span>
      <p style="margin-top: 10px; font-size: 0.9rem; color: #8b949e;">
        Walkthrough detallado cubriendo enumeración, análisis y lecciones aprendidas.
      </p>
      <a href="{{ link }}" style="color: #58a6ff; text-decoration: none; font-weight: bold;">Read Write-up →</a>
    </div>
    
  {% endfor %}
</div>
