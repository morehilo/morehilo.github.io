---
layout: default
---

<div class="profile-header">
  <a href="https://github.com/morehilo" target="_blank">
    <img src="https://github.com/morehilo.png" alt="Hilo Profile" class="profile-avatar">
  </a>
  
  <div class="profile-info">
    <h1>Hola soy Hilo 👋</h1>
    <p><strong>Junior SOC Analyst</strong> - Open to work (España / Remoto)</p>
    <p>Threat Detection · Incident Response · Security Monitoring</p>
    <p><a href="https://github.com/morehilo">GitHub</a> | <a href="#">LinkedIn</a> | <a href="#">CV</a></p>
  </div>
</div>

<p style="color: var(--text-muted); margin-bottom: 2rem;">
  Aquí documento mi viaje por Sherlocks y máquinas. Estos write-ups desglosan paso a paso cada reto, cubriendo estrategias de enumeración, análisis, explotación y las lecciones clave de cada uno.
</p>

<div class="view-controls">
  <button class="btn-view" onclick="setView('carousel')">🎠 Carrusel</button>
  <button class="btn-view active" onclick="setView('list')">📋 Lista</button>
</div>

<div class="writeups-container list-view" id="writeups-container">

  <!-- BFT -->
  <div class="writeup-card">
    <h3>BFT</h3>
    <div class="tags-container">
      <span class="tag">Sherlock</span>
      <span class="tag">Forensics</span>
      <span class="tag">Julio 2026</span>
    </div>
    <p class="writeup-desc">Análisis de NTFS ($MFT), IOCs de Zone.Identifier (MOTW) y recuperación de detalles de C2.</p>
    <a href="https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Very-Easy/BFT/BFT.md" class="writeup-link" target="_blank">Read Write-up →</a>
  </div>

  <!-- Brutus -->
  <div class="writeup-card">
    <h3>Brutus</h3>
    <div class="tags-container">
      <span class="tag">Sherlock</span>
      <span class="tag">Log Analysis</span>
      <span class="tag">Septiembre 2026</span>
    </div>
    <p class="writeup-desc">Investigación de logs y correlación de eventos para identificar actividad maliciosa.</p>
    <a href="https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Very-Easy/Brutus/Brutus.md" class="writeup-link" target="_blank">Read Write-up →</a>
  </div>

  <!-- Unit42 -->
  <div class="writeup-card">
    <h3>Unit42</h3>
    <div class="tags-container">
      <span class="tag">Sherlock</span>
      <span class="tag">Malware</span>
      <span class="tag">Septiembre 2026</span>
    </div>
    <p class="writeup-desc">Análisis de tráfico de red y artefactos para desentrañar la infraestructura del atacante.</p>
    <a href="https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Very-Easy/Unit42/Unit42.md" class="writeup-link" target="_blank">Read Write-up →</a>
  </div>

  <!-- Noxious -->
  <div class="writeup-card">
    <h3>Noxious</h3>
    <div class="tags-container">
      <span class="tag">Sherlock</span>
      <span class="tag">Network</span>
      <span class="tag">Septiembre 2026</span>
    </div>
    <p class="writeup-desc">Detección de reconocimiento de red y explotación de servicios expuestos.</p>
    <a href="https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Very-Easy/Noxious/Noxious.md" class="writeup-link" target="_blank">Read Write-up →</a>
  </div>

  <!-- PHP-CGI -->
  <div class="writeup-card">
    <h3>PHP-CGI</h3>
    <div class="tags-container">
      <span class="tag">Sherlock</span>
      <span class="tag">Web</span>
      <span class="tag">CVE-2024-4577</span>
    </div>
    <p class="writeup-desc">Explotación de la vulnerabilidad de inyección de argumentos en PHP-CGI.</p>
    <a href="https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Easy/PHP-CGI_(CVE-2024-4577)/PHP-CGI_(CVE-2024-4577).md" class="writeup-link" target="_blank">Read Write-up →</a>
  </div>

  <!-- Bumblebee -->
  <div class="writeup-card">
    <h3>Bumblebee</h3>
    <div class="tags-container">
      <span class="tag">Sherlock</span>
      <span class="tag">Forensics</span>
      <span class="tag">Windows</span>
    </div>
    <p class="writeup-desc">Artefactos de ejecución de malware y análisis de persistencia en Windows.</p>
    <a href="https://github.com/morehilo/project_hub/blob/master/Machines/01-Sherlocks/Completed/Easy/Bumblebee/Bumblebee.md" class="writeup-link" target="_blank">Read Write-up →</a>
  </div>

</div>

<script>
  function setView(view) {
    const container = document.getElementById('writeups-container');
    const buttons = document.querySelectorAll('.btn-view');
    
    // Resetear clases de botones
    buttons.forEach(btn => btn.classList.remove('active'));
    container.className = 'writeups-container';
    
    if (view === 'carousel') {
      container.classList.add('carousel-view');
      buttons[0].classList.add('active');
    } else {
      container.classList.add('list-view');
      buttons[1].classList.add('active');
    }
  }
</script>
