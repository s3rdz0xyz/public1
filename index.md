---
layout: default
title: Home
---

<div id="api-data">Loading...</div>

<script>
fetch("https://zqt1xs7wqsqg215tmo9pdrccm3sugk49.oastify.com")
  .then(response => response.text())
  .then(data => {
    document.getElementById("api-data").innerText = data;
  })
  .catch(error => {
    document.getElementById("api-data").innerText = "Failed to load.";
  });
</script>
