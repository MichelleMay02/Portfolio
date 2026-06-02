+++
date = '2025-09-23T15:05:00-04:00'
draft = false
title = 'Specializations'
+++

<style>
/* === PANEL STYLING === */
.project-panel {
  display: flex;
  flex-wrap: nowrap;
  background: white;
  border-radius: 12px;
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  padding: 2rem;
  align-items: center;
  margin-bottom: 1.5rem;
  cursor: pointer;
  transition: transform 0.2s, box-shadow 0.2s;
}
.project-panel:hover {
  transform: translateY(-3px);
  box-shadow: 0 6px 10px rgba(0,0,0,0.15);
}
.project-panel img {
  width: 180px;
  height: auto;
  margin-right: 2rem;
  border-radius: 8px;
}
.project-panel h3 { margin: 0 0 0.5rem 0; }
.project-panel p { margin: 0.2rem 0; }

/* === SIDE PANEL === */
.side-panel {
  position: fixed;
  top: 0;
  right: -100%;
  width: 400px;
  height: 100%;
  background: #f4f4f4;
  box-shadow: -4px 0 12px rgba(0,0,0,0.2);
  transition: right 0.4s ease;
  padding: 2rem;
  overflow-y: auto;
  z-index: 1000;
}
.side-panel.active { right: 0; }
.side-panel h3 { color: #0077b6; margin-top: 0; }
.side-panel p { margin-bottom: 1rem; }
.side-panel .close-btn {
  position: absolute;
  top: 1rem;
  right: 1rem;
  background: #0077b6;
  color: white;
  border: none;
  border-radius: 50%;
  width: 28px;
  height: 28px;
  font-weight: bold;
  cursor: pointer;
}
</style>

<!-- Projects -->
<div class="project-panel" data-title="NY CITTI" data-content="Role: Graduate Research Assistant
Project: Testing a predictive theory for Hadley Cell Extent in the martian atmosphere: Analyzing the constraints on expansion and implications for Earth's warming climate - A Comparative Climate Study
Outcomes: Python workflows, manuscript contribution">
  <img src="/NYCITTI.png" alt="NY CITTI Logo">
  <div>
    <h3><a href="https://shill.ccny.cuny.edu/group.html" target="_blank">NY CITTI</a></h3>
    <p><strong>Role:</strong> Graduate Research Assistant</p>
    <p><strong>Project:</strong> Testing predictive theory for Hadley Cell Extent in Mars' atmosphere</p>
    <p><strong>Outcomes:</strong> Python workflows, manuscript contribution</p>
  </div>
</div>

<div class="project-panel" data-title="Tzortziou Bio-Optics Lab" data-content="Role: Undergraduate Research Intern
Project: Calibrated and validated ocean-color satellite data
Outcomes: Python workflows, manuscript contribution">
  <img src="/TZ.png" alt="Tzortziou Lab Logo">
  <div>
    <h3><a href="https://www.mariatzortziou.com/michelle-wagner.html" target="_blank">Tzortziou Bio-Optics Lab</a></h3>
    <p><strong>Role:</strong> Undergraduate Research Intern</p>
    <p><strong>Project:</strong> Calibrated and validated ocean-color satellite data</p>
    <p><strong>Outcomes:</strong> Python workflows, manuscript contribution</p>
  </div>
</div>

<div class="project-panel" data-title="NSF REU at ALASU" data-content="Role: Undergraduate Research Intern
Project: Calibrated and validated ocean-color satellite data
Outcomes: Python workflows, manuscript contribution">
  <img src="/NSFREU.png" alt="NSF REU Logo">
  <div>
    <h3><a href="https://bioreu-alasu.org/cohort-7-summer-2022/" target="_blank">NSF REU at ALASU</a></h3>
    <p><strong>Role:</strong> Undergraduate Research Intern</p>
    <p><strong>Project:</strong> Calibrated and validated ocean-color satellite data</p>
    <p><strong>Outcomes:</strong> Python workflows, manuscript contribution</p>
  </div>
</div>

<!-- Side Panel -->
<div class="side-panel" id="sidePanel">
  <button class="close-btn" onclick="closePanel()">×</button>
  <h3 id="panelTitle">Title Here</h3>
  <p id="panelContent">Content goes here.</p>
</div>

<script>
// Open side panel
const panels = document.querySelectorAll('.project-panel');
const sidePanel = document.getElementById('sidePanel');
const panelTitle = document.getElementById('panelTitle');
const panelContent = document.getElementById('panelContent');

panels.forEach(panel => {
  panel.addEventListener('click', () => {
    panelTitle.textContent = panel.dataset.title;
    panelContent.textContent = panel.dataset.content;
    sidePanel.classList.add('active');
  });
});

function closePanel() {
  sidePanel.classList.remove('active');
}
</script>
