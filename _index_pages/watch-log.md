---
layout: single
title: Watch Log
---
/* Container */
.tab-container {
  margin-top: 20px;
  font-family: Arial, sans-serif;
}

/* TAB HEADER BAR */
.tab-header {
  border-bottom: 2px solid #ccc;
  margin-bottom: 10px;
}

/* TAB BUTTONS */
.tab-btn {
  background: #eee;
  display: inline-block;
  padding: 10px 16px; 
  margin-right: 4px;
  border: none;
  cursor: pointer;
  border-radius: 6px 6px 0 0;
}

.tab-btn.active {
  background: #fff;
  border-bottom: 2px solid white;
  font-weight: bold;
}

/* CONTENT */
.tab-content {
  display: none;
  padding: 10px;
  background: #fff;
}

.tab-content.active {
  display: block;
}

/* ITEMS */
.item {
  border-bottom: 1px solid #ddd;
  margin-bottom: 10px;
  padding-bottom: 8px;
}

.item-title {
  cursor: pointer;
  padding: 5px;
  font-weight: bold;
}

.item-details {
  display: none;
  padding: 8px;
  background: #fafafa;
  border-left: 3px solid #ccc;
  margin-top: 5px;
}


<div class="tab-container">

  <!-- TAB HEADERS -->
  <div class="tab-header">
    <button class="tab-btn active" data-tab="documentary">Documentary</button>
    <button class="tab-btn" data-tab="movies">Movies</button>
    <button class="tab-btn" data-tab="lectures">Lectures</button>
  </div>

  <!-- TAB CONTENT: DOCUMENTARY -->
  <div id="documentary" class="tab-content active">

    <div class="item">
      <div class="item-title" onclick="toggleItem(this)">
        Planet Earth II — (2025-01-12) ★★★★☆
      </div>
      <div class="item-details">
        A stunning documentary showing ecosystems across the world...
      </div>
    </div>

    <div class="item">
      <div class="item-title" onclick="toggleItem(this)">
        Oppenheimer’s Legacy — (2025-02-01) ★★★★★
      </div>
      <div class="item-details">
        Explores the consequences of nuclear innovation...
      </div>
    </div>

  </div>

  <!-- TAB CONTENT: MOVIES -->
  <div id="movies" class="tab-content">
    <div class="item">
      <div class="item-title" onclick="toggleItem(this)">
        Interstellar — (2025-01-03) ★★★★★
      </div>
      <div class="item-details">
        Nolan’s masterpiece on time, gravity, and human emotion.
      </div>
    </div>
  </div>

  <!-- TAB CONTENT: LECTURES -->
  <div id="lectures" class="tab-content">
    <div class="item">
      <div class="item-title" onclick="toggleItem(this)">
        MIT Deep Learning Lecture 1 — (2025-01-20) ★★★★☆
      </div>
      <div class="item-details">
        Great intro to neural networks and ML foundations.
      </div>
    </div>
  </div>

</div>



<script>
function openTab(tabName) {
  document.querySelectorAll('.tab-content').forEach(t => t.classList.remove('active'));
  document.getElementById(tabName).classList.add('active');

  document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
  document.querySelector('.tab-btn[data-tab="'+tabName+'"]').classList.add('active');
}

document.querySelectorAll('.tab-btn').forEach(btn => {
  btn.addEventListener('click', () => {
    openTab(btn.dataset.tab);
  });
});

function toggleItem(element) {
  const detail = element.nextElementSibling;
  detail.style.display = (detail.style.display === "block") ? "none" : "block";
}
</script>
