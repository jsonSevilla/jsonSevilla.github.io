---
layout: default
title: Resume Card
---

<div class="nba-card">
  <div class="header">
    <h2>Jason Sevilla</h2>
    <div class="ovr" data-ovr>OVR 0</div>
  </div>
  <div class="stats">
    <div class="stat"><span>Threat Hunting</span><span data-value>94</span></div>
    <div class="stat"><span>Python</span><span data-value>89</span></div>
    <div class="stat"><span>AI Automation</span><span data-value>90</span></div>
    <div class="stat"><span>Red Teaming</span><span data-value>91</span></div>
  </div>
</div>

<script>
  document.addEventListener("DOMContentLoaded", () => {
    const values = [...document.querySelectorAll('[data-value]')].map(e => +e.textContent);
    const avg = Math.round(values.reduce((a,b)=>a+b)/values.length);
    document.querySelector('[data-ovr]').textContent = 'OVR ' + avg;
  });
</script>

