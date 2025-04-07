---
layout: archive
permalink: /research/
title: ""
author_profile: true
---

<style>
.collapsible {
  background-color: #f2f2f2;
  color: #333;
  cursor: pointer;
  padding: 10px 20px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 5px;
  transition: background-color 0.2s ease;
  border-radius: 8px;
}

.collapsible:hover {
  background-color: #e2e2e2;
}

.content {
  padding: 0 20px;
  display: none;
  overflow: hidden;
  background-color: #fafafa;
  border-left: 4px solid #ccc;
  border-radius: 0 0 8px 8px;
  margin-bottom: 15px;
  animation: fadein 0.3s ease-in;
}

@keyframes fadein {
  from {opacity: 0;}
  to {opacity: 1;}
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function () {
  var coll = document.getElementsByClassName("collapsible");
  for (let i = 0; i < coll.length; i++) {
    coll[i].addEventListener("click", function () {
      this.classList.toggle("active");
      var content = this.nextElementSibling;
      if (content.style.display === "block") {
        content.style.display = "none";
      } else {
        content.style.display = "block";
      }
    });
  }
});
</script>

<button class="collapsible">Michscan: Black-Box Neural Network Integrity Checking at Runtime Through Power Analysis</button>
<div class="content">
  <p>This project introduces Michscan, a method for verifying the integrity of neural networks during runtime using power side-channel analysis. By modeling expected power behavior and comparing it with live readings, we can detect malicious tampering or unexpected behavior in deployed AI systems.</p>
  
  <p>Key features:</p>
  <ul>
    <li>Black-box methodology (no access to internal weights)</li>
    <li>Runtime detection capability</li>
    <li>Applicable to embedded and edge devices</li>
  </ul>

  <img src="/assets/images/michscan-overview.png" alt="Michscan Overview" style="max-width:100%; margin-top:10px; border-radius:8px;">
</div>
