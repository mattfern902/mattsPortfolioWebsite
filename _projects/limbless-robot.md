---
layout: project
title: AquaMILR+ Limbless Robot
cover_image: /assets/aquamilr/ogblackSnakeOpenWater.jpg
description: Design of an untethered limbless robot for complex aquatic terrain navigation. (accepted ICRA 2025)
glb_url: /assets/AquaMILR+/workingAssemC.glb
camera_orbit: 90deg 150deg 1.5m
field_of_view: 20deg
tags:
  - Robotics
  - Aquatic
  - ICRA 2025
order: 2
display_dates: December 2023 - Present
---

## AquaMILR+ Limbless Robot

**Collaborators:** Tianyu Wang, Galen Tunnicliffe, Donoven Dortilus, Peter Gunnarson, John O. Dabiri, Daniel I. Goldman

A novel untethered limbless robot designed for complex aquatic terrain navigation. This project was accepted to ICRA 2025 and features advanced mechanical intelligence for robust movement in challenging environments.

<div style="display:flex;gap:1.5em;justify-content:center;margin:2em 2vw;flex-wrap:nowrap;align-items:flex-end;">
  <div style="text-align:center;">
    <img src="{{ site.baseurl }}/assets/aquamilr/ogblackSnakeOpenWater.jpg" alt="AquaMILR+ in open water" style="height:300px;width:auto;object-fit:contain;display:block;margin-left:auto;margin-right:auto;border-radius:1em;box-shadow:0 2px 12px rgba(0,0,0,0.10);margin-bottom:0.5em;background:#222;">
    <div style="color:#aaa;font-size:1em;">Rendering of AquaMILR+ in the open ocean</div>
  </div>
  <div style="text-align:center;">
    <img src="{{ site.baseurl }}/assets/aquamilr/aquaMILR_CAD_pic.jpg" alt="AquaMILR+ CAD design" style="height:300px;width:auto;object-fit:contain;display:block;margin-left:auto;margin-right:auto;border-radius:1em;box-shadow:0 2px 12px rgba(0,0,0,0.10);margin-bottom:0.5em;background:#222;">
    <div style="color:#aaa;font-size:1em;">CAD Design</div>
  </div>
  <div style="text-align:center;">
    <img src="{{ site.baseurl }}/assets/AquaMILR+/AquaMILR+Pic.jpg" alt="AquaMILR+ assembly" style="height:300px;width:auto;object-fit:contain;display:block;margin-left:auto;margin-right:auto;border-radius:1em;box-shadow:0 2px 12px rgba(0,0,0,0.10);margin-bottom:0.5em;background:#222;">
    <div style="color:#aaa;font-size:1em;">Full Assembly</div>
  </div>
</div>

<div style="display:flex;gap:1.2em;justify-content:flex-start;margin:2em 0 2em 2vw;flex-wrap:nowrap;align-items:flex-start;max-width:1400px;min-height:60vh;">
  <!-- Left column: GLBs stacked -->
  <div style="display:flex;flex-direction:column;gap:0.7em;align-items:center;width:420px;">
    <h3 style="text-align:center;margin:0.7em 0 0.3em 0;">Electronics Module</h3>
    <model-viewer src="{{ site.baseurl }}/assets/AquaMILR+/electronicsModuleC.glb" alt="A 3D model of AquaMILR+ Electronics Module" auto-rotate camera-controls style="width:100%;max-width:420px;height:300px;margin:0 0 1em 0;display:block;background:#23272a;border-radius:1em;"></model-viewer>
    <h3 style="text-align:center;margin:0.7em 0 0.3em 0;">Buoyancy Module</h3>
    <model-viewer src="{{ site.baseurl }}/assets/AquaMILR+/biggerNew_-_Copy.glb" alt="A 3D model of AquaMILR+ Buoyancy Module" auto-rotate camera-controls style="width:100%;max-width:420px;height:300px;margin:0 0 1em 0;display:block;background:#23272a;border-radius:1em;"></model-viewer>
  </div>
  <!-- Middle column: two videos stacked -->
  <div style="display:flex;flex-direction:column;gap:0.7em;align-items:center;width:420px;">
    <h3 style="text-align:center;margin:0.7em 0 0.3em 0;">Depth Control Animations (Patent Pending)</h3>
    <video src="{{ site.baseurl }}/assets/AquaMILR+/sideViewTLS.mp4" controls style="width:100%;max-width:420px;height:180px;margin:0 0 1em 0;display:block;background:#23272a;border-radius:1em;object-fit:cover;"></video>
    <video src="{{ site.baseurl }}/assets/AquaMILR+/in_assembly_animation.mp4" controls style="width:100%;max-width:420px;height:320px;margin:0 0 1em 0;display:block;background:#23272a;border-radius:1em;object-fit:cover;"></video>
  </div>
  <!-- Right column: tall video -->
  <div style="display:flex;flex-direction:column;gap:0.7em;align-items:center;width:420px;">
    <h3 style="text-align:center;margin:0.7em 0 0.3em 0;">Demo Video</h3>
    <video src="{{ site.baseurl }}/assets/AquaMILR+/straightVB.mp4" controls style="width:100%;max-width:420px;height:680px;margin:0 0 1em 0;display:block;background:#23272a;border-radius:1em;object-fit:cover;"></video>
  </div>
</div>

<div style="display:flex;gap:2.5em;flex-wrap:wrap;justify-content:center;margin-bottom:2.5em;">
  <div style="flex:1;min-width:320px;max-width:700px;display:flex;flex-direction:column;align-items:center;">
    <iframe width="100%" height="480" src="https://www.youtube.com/embed/l1MjoG7HlX8" title="AquaMILR Project Video" frameborder="0" allowfullscreen style="border-radius:1em;box-shadow:0 4px 24px rgba(0,0,0,0.15);"></iframe>
  </div>
  <div style="flex:1;min-width:320px;max-width:700px;display:flex;flex-direction:column;align-items:center;">
    <iframe src="{{ site.baseurl }}/assets/AquaMILR+/ICRA25Paper.pdf" width="100%" height="480" style="border-radius:1em;box-shadow:0 4px 24px rgba(0,0,0,0.15);"></iframe>
    <div style="color:#aaa;font-size:1.05em;margin-top:0.7em;text-align:center;">Preview: ICRA 2025 Paper (PDF)</div>
  </div>
</div>

<div style="margin-bottom:2em;text-align:center;">
  <a href="https://arxiv.org/abs/2409.18383" target="_blank" style="display:inline-block;background:#fff;color:#181a1b;padding:0.9em 2em;border-radius:2em;font-weight:700;text-decoration:none;box-shadow:0 2px 8px #fff;font-size:1.15em;transition:background 0.2s;">View Published Paper on arXiv</a>
  <div style="color:#aaa;font-size:1.1em;margin-top:0.7em;">AquaMILR+: Design of an untethered limbless robot for complex aquatic terrain navigation</div>
</div>

### Related Publications
<div style="background:#23272a;padding:2em 1.5em;border-radius:1em;box-shadow:0 2px 16px var(--accent3);margin-bottom:2em;">
  <h3 style="color:var(--accent3);margin-top:0;">Patent</h3>
  <ul style="color:#e0e0e0;">
    <li><b>M. Fernandez</b>, T. Wang, D. I. Goldman. Compact buoyancy control assembly for underwater robotic systems or equipment (<i>filed patent application 2024</i>)</li>
  </ul>
  <h3 style="color:var(--accent3);margin-top:0;">Peer-Reviewed Publications</h3>
  <ul style="color:#e0e0e0;">
    <li><b>M. Fernandez</b>, T. Wang, G. Tunnicliffe, D. Dortilus, P. Gunnarson, J.O. Dabiri, D. I. Goldman. <b>AquaMILR+: Design of an untethered limbless robot for complex aquatic terrain navigation</b>. <a href="https://arxiv.org/abs/2409.18383" target="_blank" style="color:#181a1b;text-decoration:underline;background:#fff;padding:0.2em 0.7em;border-radius:1em;font-weight:700;">arXiv:2409.18383</a> (<i>accepted ICRA 2025</i>)</li>
    <li>T. Wang, N. Mankame, <b>M. Fernandez</b>, V. H. Kojuoharov, D. I. Goldman. AquaMILR: Mechanical intelligence simplifies control of undulatory robots in cluttered fluid environments (<i>accepted ICRA 2025</i>)</li>
  </ul>
  <h3 style="color:var(--accent3);">Conference Abstracts</h3>
  <ul style="color:#e0e0e0;">
    <li><b>M. Fernandez</b>, T. Wang, G. Tunnicliffe, D. Dortilus, D. I. Goldman. Design of an untethered limbless robot for aquatic locomotion in complex environments. <i>American Physical Society Meeting, March 2025</i>.</li>
    <li>T. Wang, <b>M. Fernandez</b>, G. Tunnicliffe, D. Dortilus, D. I. Goldman. Mechanical and computational intelligence enable agile and robust limbless robotic locomotion in complex aquatic environments. <i>American Physical Society Meeting, March 2025</i>.</li>
    <li><b>M. Fernandez</b>, T. Wang, G. Tunnicliffe, D. Dortilus, D. I. Goldman. Design of an untethered underwater limbless robot for complex aquatic terrain navigation. <i>SICB Annual Meeting, January 2025</i>.</li>
    <li>T. Wang, <b>M. Fernandez</b>, G. Tunnicliffe, D. Dortilus, D. I. Goldman. Mechanically intelligent undulatory robotic locomotion in complex aquatic environments. <i>SICB Annual Meeting, January 2025</i>.</li>
  </ul>
  <h3 style="color:var(--accent3);">Presentations</h3>
  <ul style="color:#e0e0e0;">
    <li>Design of an untethered limbless robot for complex aquatic terrain navigation. <i>IEEE International Conference on Robotics and Automation (ICRA), 2025</i>.</li>
    <li>Design of an untethered limbless robot for aquatic locomotion in complex environments. <i>American Physical Society Meeting, March 2025</i>.</li>
    <li>Mechanically intelligent undulatory robotic locomotion in complex aquatic environments. <i>College of Science Undergraduate Research Showcase, February 2025</i>.</li>
    <li>Design of an untethered underwater limbless robot for complex aquatic terrain navigation. <i>SICB Annual Meeting, January 2025</i>.</li>
  </ul>
</div> 