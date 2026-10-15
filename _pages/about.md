---
layout: profile
permalink: /
title: "Xiaoqian Zhang — Medical Imaging & Machine Learning"
excerpt: "Xiaoqian Zhang at Shanghai Jiao Tong University. Medical imaging, representation learning, computational pathology, and research software."
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

<section class="showcase-hero" aria-labelledby="profile-name">
  <div class="showcase-intro">
    <p class="showcase-location">Shanghai Jiao Tong University <span>Shanghai, China</span></p>
    <h1 id="profile-name">Xiaoqian<br>Zhang<span class="showcase-chinese" lang="zh">张啸谦 / Shawno</span></h1>
    <p class="showcase-statement">Medical intelligence.<br>From representations to systems.</p>
    <p class="showcase-bio">I study how machines learn from medical images — and build the research tools around them. M.S. student in Medical Imaging Technology at SJTU, with a background in biomedical engineering at Beihang.</p>
    <div class="showcase-actions">
      <a class="showcase-button" href="#selected-research">Explore my work <span aria-hidden="true">↘</span></a>
      <a class="showcase-text-link" href="/cv/">Curriculum vitae</a>
      <a class="showcase-text-link" href="mailto:xiaoqian_shawno@sjtu.edu.cn">Email me</a>
    </div>
  </div>
  <div class="showcase-visual">
    <div class="showcase-portrait">
      <img src="/images/xiaoqian-zhang-2026.jpg" width="104" height="104" alt="Portrait of Xiaoqian Zhang" fetchpriority="high">
      <div><strong>Research &amp; engineering</strong><span>Medical imaging · Machine learning</span></div>
    </div>
    <section class="showcase-work-preview" aria-labelledby="work-preview-title">
      <div class="showcase-work-preview-heading"><h2 id="work-preview-title">Selected work</h2><span>Papers &amp; systems</span></div>
      <a class="showcase-work-preview-item" href="/publication/2026-01-23-vqpet/">
        <div class="showcase-work-preview-meta"><span>Journal article</span><span>2026</span></div>
        <h3><span class="showcase-work-title"><span class="work-badge work-badge--journal" aria-label="Journal: IEEE TMI">IEEE TMI</span><span>— VQPET</span></span><span aria-hidden="true">↗</span></h3>
        <p>Learning codebook priors for PET image synthesis.</p>
      </a>
      <a class="showcase-work-preview-item" href="/publication/2026-03-01-momil/">
        <div class="showcase-work-preview-meta"><span>Journal article</span><span>2026</span></div>
        <h3><span class="showcase-work-title"><span class="work-badge work-badge--journal" aria-label="Journal: Image and Vision Computing">IVC</span><span>— MoMIL</span></span><span aria-hidden="true">↗</span></h3>
        <p>Multiple instance learning for whole-slide pathology.</p>
      </a>
      <a class="showcase-work-preview-item" href="https://github.com/Xiaoqian-Zhang-Shawno/ShawnoBot">
        <div class="showcase-work-preview-meta"><span>Open-source system</span><span>Python</span></div>
        <h3><span class="showcase-work-title"><span class="work-badge work-badge--repo">Repo</span><span>— ShawnoBot</span></span><span aria-hidden="true">↗</span></h3>
        <p>A controlled gateway to the research workstation.</p>
      </a>
    </section>
  </div>
</section>

<nav class="showcase-index" aria-label="Profile sections">
  <a href="#selected-research">Selected research <span aria-hidden="true">↓</span></a>
  <a href="#projects">Open-source systems <span aria-hidden="true">↓</span></a>
  <a href="#background">Background <span aria-hidden="true">↓</span></a>
  <a href="https://scholar.google.co.jp/citations?user=maQlQdIAAAAJ&amp;hl=zh-CN">Google Scholar <span aria-hidden="true">↗</span></a>
</nav>

<section class="showcase-section" id="selected-research" aria-labelledby="selected-title">
  <div class="showcase-section-heading"><div><p class="showcase-caption">Research in focus</p><h2 id="selected-title">Learning the structure<br>behind the image.</h2></div><a class="showcase-text-link" href="/publications/">All publications <span aria-hidden="true">↗</span></a></div>
  <p class="showcase-section-intro">My work connects representation learning with medical imaging: aggregating whole-slide information, learning synthesis priors, and understanding complementary imaging modalities.</p>
  <div class="showcase-papers">
    {% assign selected_papers = site.publications | sort: "date" | reverse %}
    {% for post in selected_papers limit:3 %}
    <article class="showcase-paper">
      <div class="showcase-paper-meta"><span>{{ post.venue | split: "," | first }}</span><span>{{ post.date | date: "%Y" }}</span></div>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.excerpt }}</p>
      <div class="showcase-paper-bottom"><span>{{ post.topics | first }}</span><a href="{{ post.paperurl }}" aria-label="Read paper: {{ post.title | escape }}">Read paper <span aria-hidden="true">↗</span></a></div>
    </article>
    {% endfor %}
  </div>
  <div class="showcase-research-note"><strong>Also exploring</strong><p>3D perception and spatially aware representations for volumetric medical data.</p><a href="/research/">Research directions</a></div>
</section>

<section class="showcase-section showcase-systems" id="projects" aria-labelledby="systems-title">
  <div class="showcase-section-heading"><div><p class="showcase-caption">Built for the workflow</p><h2 id="systems-title">Research needs<br>good systems, too.</h2></div><a class="showcase-text-link" href="https://github.com/Xiaoqian-Zhang-Shawno">On GitHub <span aria-hidden="true">↗</span></a></div>
  <div class="showcase-project showcase-project-featured">
    <div class="showcase-project-body"><p class="showcase-caption">Research infrastructure</p><h3>ShawnoBot</h3><p>A controlled bridge between Feishu and a local research workstation. Inspect GPU usage, training logs, and jobs; run allowlisted tasks and sandboxed Codex workflows from chat.</p><ul class="showcase-tags" aria-label="ShawnoBot technologies"><li>Python</li><li>Feishu</li><li>Codex CLI</li><li>GPU monitoring</li></ul><a class="showcase-project-link" href="https://github.com/Xiaoqian-Zhang-Shawno/ShawnoBot">Explore ShawnoBot <span aria-hidden="true">↗</span></a></div>
    <div class="showcase-workflow" aria-label="ShawnoBot workflow"><div><span>Interface</span><strong>Feishu message</strong></div><span class="showcase-workflow-line" aria-hidden="true"></span><div><span>Control</span><strong>Authorization &amp; allowlists</strong></div><span class="showcase-workflow-line" aria-hidden="true"></span><div><span>Workstation</span><strong>GPU · Logs · Codex tasks</strong></div></div>
  </div>
  <div class="showcase-project-pair">
    <article class="showcase-project"><p class="showcase-caption">Literature intelligence</p><h3>notion-monthly-research</h3><p>From recent arXiv papers to a structured research digest. Scheduled collection, model-assisted trend synthesis, and archival in Notion.</p><ul class="showcase-tags"><li>Python</li><li>GitHub Actions</li><li>LLM</li><li>Notion API</li></ul><a class="showcase-project-link" href="https://github.com/Xiaoqian-Zhang-Shawno/notion-monthly-research">Explore the workflow <span aria-hidden="true">↗</span></a></article>
    <article class="showcase-project"><p class="showcase-caption">Local-first application</p><h3>BetDogEye</h3><p>A sports-betting portfolio analysis app with exposure and return analytics, local storage, data portability, and optional AI-assisted insights.</p><ul class="showcase-tags"><li>JavaScript</li><li>PWA</li><li>Data visualization</li></ul><a class="showcase-project-link" href="https://github.com/Xiaoqian-Zhang-Shawno/BetDogEye">Explore the application <span aria-hidden="true">↗</span></a></article>
  </div>
</section>

<section class="showcase-section showcase-background" id="background" aria-labelledby="background-title">
  <div><p class="showcase-caption">The foundation</p><h2 id="background-title">Engineering roots.<br>Medical perspective.</h2><p>Biomedical engineering training, medical imaging research, and hands-on experience with tissue data.</p><a class="showcase-text-link" href="/cv/">Full curriculum vitae <span aria-hidden="true">↗</span></a></div>
  <div class="showcase-timeline">
    <article><span>2021–2025</span><h3>Beihang University</h3><p>B.E. in Biomedical Engineering</p></article>
    <article><span>Jun–Nov 2024</span><h3>BGI Research Institute</h3><p>Research internship · Spatial transcriptomics, tissue annotation, and image segmentation</p></article>
    <article><span>2025–2028 · Expected</span><h3>Shanghai Jiao Tong University</h3><p>M.S. in Medical Imaging Technology<br>School of Medical Technology</p></article>
    <article><span>Jul–Dec 2026 · Expected completion</span><h3>United Imaging Zhirong</h3><p>Internship · Multi-view endoscopic reconstruction and research engineering</p></article>
  </div>
</section>

<section class="showcase-contact" aria-labelledby="contact-title"><div><p class="showcase-caption">Start a conversation</p><h2 id="contact-title">Shared questions.<br>Better research.</h2><p>Interested in medical imaging, representation learning, or tools for research? Let’s talk.</p><a class="showcase-contact-email" href="mailto:xiaoqian_shawno@sjtu.edu.cn">xiaoqian_shawno@sjtu.edu.cn <span aria-hidden="true">↗</span></a></div><div class="showcase-contact-links"><a href="https://github.com/Xiaoqian-Zhang-Shawno">GitHub</a><a href="https://scholar.google.co.jp/citations?user=maQlQdIAAAAJ&amp;hl=zh-CN">Google Scholar</a><a href="https://orcid.org/0009-0004-5587-2188">ORCID</a></div></section>
