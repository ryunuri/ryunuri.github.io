---
permalink: /
title: "Nuri Ryu"
author_profile: true
redirect_from: 
  - /about/
  - /about.html

excerpt: |
  <span style="font-size: 0.7em;">
    I am a Ph.D student at the <a href="https://cg.postech.ac.kr/" style="color: #a76bcf;">POSTECH Computer Graphics Lab</a>
    supervised by <a href="https://www.scho.pe.kr/" style="color: #a76bcf;">Prof. Sunghyun Cho</a>.<br>
    My research focuses on 2D/3D generative models and neural rendering.<br>
    I am particularly passionate about making 3D modeling more accessible to the general public by allowing users to create 3D assets just from a single image or a simple text prompt.<br>
    For more information, please check out my publications.
  </span>
classes: wide
header:
  overlay_image: /assets/images/background_cropped.jpg
  overlay_filter: 0.75 # same as adding an opacity of 0.5 to a black background
  caption: "Gyeongju, South Korea"
  actions:
    - label: "About My Work"
      url: "/#publications"
---

<head>
  <!-- Include FontAwesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
  <style>
    table {
      width: 100%;
      border-collapse: collapse;
    }
    table td {
      border: none; /* Make borders invisible */
      padding: 5px;
      vertical-align: top;
    }
    .date {
      width: 20%;
      font-size: 0.9em; /* Make the date slightly smaller */
      white-space: nowrap; /* Prevent date from breaking */
    }
    .content {
      width: 80%;
    }
    .publication-image {
      width: 30%;
    }
    .publication-details {
      width: 70%;
      padding-left: 10px;
    }
    .publication-details h4 {
      font-size: 1.2em; /* Adjust the title font size */
      margin-top: 0; /* Ensure the title is aligned to the top */
      margin-bottom: 0; /* Remove margin below title */
    }
    .publication-details .authors {
      font-size: 0.9em; /* Adjust the font size */
      margin-top: 0; /* Ensure no space above authors */
      margin-bottom: 5px; /* Add space below authors */
    }
    .publication-details .conference {
      font-size: 0.9em; /* Adjust the font size */
      margin-top: 5px; /* Add space above conference */
      margin-bottom: 5px; /* Add space below conference */
    }
    .publication-details .links {
      margin-top: 10px; /* Add space above links */
    }
    .badge {
      display: inline-block;
      padding: 3px 7px; /* Make badges smaller */
      margin-right: 3px; /* Place badges closer to each other */
      border: 1px solid #ddd;
      border-radius: 3px;
      text-decoration: none;
      color: #fff;
      background-color: #444;
      font-size: 0.8em; /* Make font size smaller */
    }
    .badge:hover {
      background-color: #666;
    }
    .badge i {
      margin-right: 3px; /* Place icon closer to text */
    }
    .badge a {
      color: #fff; /* Ensure links in badges are white */
    }
    .bibtex {
      display: none;
      background-color: #222;
      color: #ddd;
      padding: 10px;
      border-radius: 5px;
      margin-top: 10px;
      font-family: monospace;
      white-space: pre-wrap;
      font-size: 0.7em; /* Match the font size of the authors */
      text-align: left; /* Left align the content */
      position: relative;
    }
    .copy-btn {
      position: absolute;
      top: 10px;
      right: 10px;
      background-color: #444;
      color: #fff;
      border: none;
      padding: 5px;
      border-radius: 3px;
      cursor: pointer;
    }
    .copy-btn:hover {
      background-color: #666;
    }
  </style>
  <script>
    function toggleBibtex(id) {
      var bibtex = document.getElementById(id);
      if (bibtex.style.display === "none" || bibtex.style.display === "") {
        bibtex.style.display = "block";
      } else {
        bibtex.style.display = "none";
      }
    }

    function copyBibtex(id) {
      var bibtexContent = document.querySelector(`#${id} .bibtex-content`).innerText;
      navigator.clipboard.writeText(bibtexContent).then(function() {
        console.log('BibTeX copied to clipboard');
      }, function(err) {
        console.error('Failed to copy BibTeX', err);
      });
    }
  </script>
</head>

# Recent News
---

| **09/2024** | Our paper on 3D reconstruction from a single image (POP3D) is accepted to <a href="https://sa2023.siggraph.org/" target="_blank" style="color: #a76bcf;">SIGGRAPH Asia 2023</a>. |
| **09/2023** | Our paper on 3D GAN adaptation to artistic drawings (Dr.3D) is accepted to <a href="https://sa2022.siggraph.org/" target="_blank" style="color: #a76bcf;">SIGGRAPH Asia 2022</a>. |


# Publications
---

<table>
  <tr>
    <td class="publication-image">
      <img src="/assets/images/pop3d.jpg" alt="Image description" style="width: 100%;">
    </td>
    <td class="publication-details">
      <h4>360° Reconstruction From a Single Image Using Space Carved Outpainting</h4>
      <div class="authors"><strong>Nuri Ryu</strong>, Minsu Gong, Geonung Kim, Joo-Haeng Lee, Sunghyun Cho</div>
      <div class="conference">ACM <strong>SIGGRAPH Asia</strong>, Sydney, Australia, 2023</div>
      <div class="links">
        <a href="http://cg.postech.ac.kr/research/POP3D" class="badge"><i class="fas fa-external-link-alt"></i>Project</a>
        <a href="https://arxiv.org/abs/2309.10279" class="badge"><i class="fas fa-file-alt"></i>arXiv</a>
        <a href="https://github.com/ryunuri/POP3D" class="badge"><i class="fas fa-code"></i>Code</a>
        <a href="javascript:void(0);" class="badge" onclick="toggleBibtex('bibtex1')"><i class="fas fa-book"></i>BibTeX</a>
      </div>
      <div id="bibtex1" class="bibtex">
        <button class="copy-btn" onclick="copyBibtex('bibtex1')"><i class="fas fa-copy"></i> Copy</button>
        <pre class="bibtex-content">
@inproceedings{10.1145/3610548.3618240,
  author    = {Ryu, Nuri and Gong, Minsu and Kim, Geonung and Lee, Joo-Haeng and Cho, Sunghyun},
  title     = {360° Reconstruction From a Single Image Using Space Carved Outpainting},
  year      = {2023},
  isbn      = {9798400703157},
  publisher = {Association for Computing Machinery},
  address   = {New York, NY, USA},
  url       = {https://doi.org/10.1145/3610548.3618240},
  doi       = {10.1145/3610548.3618240},
  booktitle = {SIGGRAPH Asia 2023 Conference Papers},
  articleno = {75},
  numpages  = {11},
  location  = {Sydney, NSW, Australia},
  series    = {SA '23}
}
        </pre>
      </div>
    </td>
  </tr>
  <tr>
    <td class="publication-image">
      <img src="/assets/images/dr3d.jpg" alt="Image description" style="width: 100%;">
    </td>
    <td class="publication-details">
      <h4>Dr.3D: Adapting 3D GANs to Artistic Drawings</h4>
      <div class="authors">Wonjoon Jin, <strong>Nuri Ryu</strong>, Geonung Kim, Seung-Hwan Baek, Sunghyun Cho</div>
      <div class="conference">ACM <strong>SIGGRAPH Asia</strong>, Daegu, South Korea, 2022</div>
      <div class="links">
        <a href="https://jinwonjoon.github.io/dr3d/" class="badge"><i class="fas fa-external-link-alt"></i>Project</a>
        <a href="https://arxiv.org/abs/2211.16798" class="badge"><i class="fas fa-file-alt"></i>arXiv</a>
        <a href="https://jinwonjoon.github.io/dr3d/" class="badge"><i class="fas fa-code"></i>Code</a>
        <a href="javascript:void(0);" class="badge" onclick="toggleBibtex('bibtex2')"><i class="fas fa-book"></i>BibTeX</a>
      </div>
      <div id="bibtex2" class="bibtex">
        <button class="copy-btn" onclick="copyBibtex('bibtex2')"><i class="fas fa-copy"></i> Copy</button>
        <pre class="bibtex-content">
@inproceedings{10.1145/3550469.3555422,
  author = {Jin, Wonjoon and Ryu, Nuri and Kim, Geonung and Baek, Seung-Hwan and Cho, Sunghyun},
  title = {Dr.3D: Adapting 3D GANs to Artistic Drawings},
  year = {2022},
  isbn = {9781450394703},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  url = {https://doi.org/10.1145/3550469.3555422},
  doi = {10.1145/3550469.3555422},
  booktitle = {SIGGRAPH Asia 2022 Conference Papers},
  articleno = {9},
  numpages = {8},
  location = {Daegu, South Korea},
  series = {SA '22}
}
        </pre>
      </div>
    </td>
  </tr>
</table>
