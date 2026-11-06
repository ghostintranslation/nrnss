---
pdf_options:
  format: A4
  margin:
    top: 0
    right: 0
    bottom: 0
    left: 0
  printBackground: true
  displayHeaderFooter: false
---

<style>
/* CSS for premium A4 User Manual PDF */

/* Global styles */
body, .markdown-body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  color: #1e293b !important;
  background-color: #ffffff !important;
  line-height: 1.6;
  font-size: 11pt;
}

h1, h2, h3, h4 {
  color: #0f172a !important;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  font-weight: 600;
  margin-top: 1.2em;
  margin-bottom: 0.4em;
}

h1 {
  font-size: 22pt;
  border-bottom: 2px solid #cbd5e1;
  padding-bottom: 0.3em;
  margin-top: 0;
  text-transform: uppercase;
}

h2 {
  font-size: 16pt;
  border-bottom: 1px solid #e2e8f0;
  padding-bottom: 0.2em;
}

h3 {
  font-size: 12pt;
}

p, li {
  color: #334155;
  font-size: 11pt;
}

ul, ol {
  margin-top: 0.4em;
  margin-bottom: 0.8em;
  padding-left: 1.5em;
}

li {
  margin-bottom: 0.3em;
}

a {
  color: #0284c7 !important;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

/* Code and syntax highlighting */
code {
  background-color: #f1f5f9 !important;
  color: #0f172a !important;
  padding: 0.2em 0.4em;
  border-radius: 4px;
  font-family: ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, monospace;
  font-size: 9pt;
}

pre {
  background-color: #f8fafc !important;
  border: 1px solid #e2e8f0;
  padding: 12px;
  border-radius: 6px;
  overflow: auto;
  margin: 1em 0;
}

pre code {
  background-color: transparent !important;
  padding: 0;
  font-size: 9pt;
}

/* Table styles */
table {
  border-collapse: collapse;
  width: 100%;
  margin: 1.2em 0;
  font-size: 9.5pt;
}

th, td {
  padding: 8px 10px;
  border: 1px solid #cbd5e1 !important;
  text-align: left;
}

th {
  background-color: #f1f5f9 !important;
  color: #0f172a !important;
  font-weight: 600;
}

tr:nth-child(even) {
  background-color: #f8fafc !important;
}

/* Page structural styles */
.cover-page {
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
  background-image: linear-gradient(rgba(0, 0, 0, 0.35), rgba(0, 0, 0, 0.35)), url('./nrnss-1.jpg');
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 0 20mm;
  color: #ffffff !important;
  text-align: center;
  break-after: page;
  page-break-after: always;
}

.cover-brand {
  font-size: 16pt;
  font-weight: 300;
  color: #ffffff !important;
  letter-spacing: 4px;
  text-transform: uppercase;
  margin-bottom: 20px;
  margin-top: 0;
}

.cover-title-group h1.cover-title {
  font-size: 92pt !important;
  color: #ffffff !important;
  font-weight: 800;
  letter-spacing: 2px;
  border-bottom: none;
  margin: 0;
  padding: 0;
}

.cover-subtitle {
  font-size: 20pt;
  font-weight: 300;
  margin-top: 15px;
  color: #e2e8f0;
}

.toc-page, .page-body {
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
  margin: 0;
  padding: 20mm 30mm 30mm 30mm; /* Extra bottom space for footer */
  position: relative;
  break-after: page;
  page-break-after: always;
  background-color: #ffffff;
}

/* Table of Contents page specific styles */
.toc-heading {
  font-size: 22pt;
  margin-top: 0;
  margin-bottom: 1.5em;
  border-bottom: 2px solid #0f172a;
  padding-bottom: 0.4em;
  text-transform: uppercase;
}

.toc-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.toc-list li {
  display: flex;
  align-items: baseline;
  margin-bottom: 16px;
  font-size: 12pt;
}

.toc-title {
  font-weight: 500;
  color: #334155;
}

.toc-dots {
  flex-grow: 1;
  border-bottom: 1px dotted #94a3b8;
  margin: 0 12px;
  position: relative;
  top: -4px;
}

.toc-page-num {
  font-weight: 600;
  color: #0f172a;
}

/* Custom footer style */
.page-footer {
  position: absolute;
  bottom: 15mm;
  left: 20mm;
  right: 20mm;
  display: flex;
  justify-content: space-between;
  font-size: 8pt;
  color: #64748b;
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  border-top: 1px solid #e2e8f0;
  padding-top: 8px;
}

/* Printing styling to enforce A4 sizing and zero margins */
@media print {
  @page {
    size: A4;
    margin: 0; /* Let HTML containers specify boundaries */
  }

  body, .markdown-body {
    background-color: #ffffff !important;
    padding: 0 !important;
    margin: 0 !important;
  }

  .cover-page, .toc-page, .page-body {
    width: 210mm;
    height: 297mm;
    margin: 0;
    box-sizing: border-box;
  }
}
</style>

<div class="cover-page">
  <div class="cover-title-group">
    <p class="cover-brand">Ghost In Translation</p>
    <h1 class="cover-title">NRNSS</h1>
    <p class="cover-subtitle">1.0.X</p>
  </div>
</div>

<div class="toc-page">
  <!-- Table of Contents Section -->
  <h2 class="toc-heading">Table of Contents</h2>
  <ul class="toc-list">
    <li>
      <span class="toc-title">1. Introduction</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">3</span>
    </li>
    <li>
      <span class="toc-title">2. Installation</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">4</span>
    </li>
    <li>
      <span class="toc-title">3. How it works</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">5</span>
    </li>
    <li>
      <span class="toc-title">4. Troubleshooting</span>
      <span class="toc-dots"></span>
      <span class="toc-page-num">7</span>
    </li>
  </ul>
  <!-- Page footer with page number 2 -->
  <div class="page-footer">
    <span>NRNSS User Manual</span>
    <span>Page 2</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 1: Introduction -->
  <h1>1. Introduction</h1>

  <p>NRNSS is a minimal mixer module for spacing out your sounds in the stereo field, based on the open source Nearness design but reworked from the ground up to provide more features and better sound quality.</p>

  <h2>Features</h2>

  <ul>
    <li>9 mono inputs</li>
    <li>7 stereo inputs</li>
    <li>Fully DC-coupled</li>
    <li>Very quiet</li>
  </ul>
  
  <h2>Technical Specifications</h1>

  <ul>
    <li><strong>Module Width</strong>: 4 HP</li>
    <li><strong>Depth</strong>: 25 mm</li>
    <li><strong>Power Consumption</strong>:
      <ul>
        <li><strong>+12V</strong>:  mA</li>
        <li><strong>-12V</strong>:  mA</li>
      </ul>
    </li>
  </ul>
  
  <!-- Page footer with page number 3 -->
  <div class="page-footer">
    <span>NRNSS User Manual</span>
    <span>Page 3</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 2: Installation -->
  <h1>2. Installation</h1>

  <p>Turn off and disconnect your Eurorack case from AC mains power before installing this module. Connect the supplied power ribbon cable to the module and your busboard. Make sure that the red stripe on the cable is connected to -12V (as shown on the back of the module).</p>
  
  <!-- Page footer with page number 4 -->
  <div class="page-footer">
    <span>NRNSS User Manual</span>
    <span>Page 4</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 3: Controls and CV Inputs -->
  <h1>3. How it works</h1>

  <p>NRNSS has 16 DC-coupled inputs, meaning that they accept both CV and audio signals. When unpatched, they’re normalled (internally connected) to 0V.</p>

  <p>The left column is made of 9 mono inputs and the right column has the 2 outputs, top and bottom, as well as 7 stereo TRS inputs in between.</p>

  <p>On the left, the closest a mono input is to an output, the greater its influence on it, either audio getting louder or CV getting more or less attenuated. The inputs are scaled with 3 dB between one another, meaning that between each input there is a gain difference that feels linear to the human ear.</p>

  <p>On the right, from top to bottom the stereo inputs have increasing attenuation, also scaled with 3 dB bettween on another. This allows to mix in loud and quiet sources and make them sound equally loud in the final mix.</p>

  
  <!-- Page footer with page number 5 -->
  <div class="page-footer">
    <span>NRNSS User Manual</span>
    <span>Page 5</span>
  </div>
</div>

<div class="page-body">

  <!-- Signal routing and panel layout diagram -->
  <img src="./nrnss_manual_diagram.svg" alt="NRNSS Signal Routing and Panel Layout Diagram" style="display: block; margin: 0 auto; height: 100%;" />
  
  <!-- Page footer with page number 5 -->
  <div class="page-footer">
    <span>NRNSS User Manual</span>
    <span>Page 6</span>
  </div>
</div>

<div class="page-body">
  <!-- Section 9: Troubleshooting -->
  <h1>4. Troubleshooting</h1>

  <h2>No Sound Output</h2>
  <ul>
    <li>Verify that the eurorack power ribbon cable is connected in the right polariry. If not it may damage the module.</li>
    <li>Make sure your audio cables are patched securely.</li>
    <li>Switch off and switch on the module.</li>
  </ul>
  
  <!-- Page footer with page number 12 -->
  <div class="page-footer">
    <span>NRNSS User Manual</span>
    <span>Page 7</span>
  </div>
</div>