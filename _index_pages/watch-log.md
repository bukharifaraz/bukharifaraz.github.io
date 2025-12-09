---
layout: single
title: Watch Log
---

<style>
    .tabs { margin-bottom: 1rem; border-bottom: 2px solid #ccc; }
    .tab {
        padding: 10px 20px;
        cursor: pointer;
        font-weight: bold;
        border-bottom: 3px solid transparent;
    }
    .tab.active {
        border-bottom-color: #000;
    }
    .tab-content { display: none; }
    .tab-content.active { display: block; }

    .item {
        border: 1px solid #ddd;
        padding: 12px;
        margin-bottom: 10px;
        cursor: pointer;
        background: #fafafa;
    }
    .item:hover {
        background: #f0f0f0;
    }

    .item-details {
        display: none;
        padding: 10px;
        background: #fff;
        border-left: 3px solid #333;
        margin-top: 8px;
    }

    .stars {
        color: #e0b000;
        font-weight: bold;
    }
</style>


<div class="tabs">
    <div class="tab active" data-tab="documentary">Documentary</div>
    <div class="tab" data-tab="movies">Movies</div>
    <div class="tab" data-tab="lectures">Lectures</div>
</div>

<!---------------- Documentary ---------------->
<div id="documentary" class="tab-content active">
    <div class="item" onclick="toggleDetails(this)">
        <strong>The Social Dilemma</strong> — 2024-12-01  
        <div class="stars">★★★★☆</div>
        <div class="item-details">
            A sharp critique of persuasive tech and algorithmic manipulation.  
            I particularly liked the part explaining engagement-driven recommender systems.
        </div>
    </div>

    <div class="item" onclick="toggleDetails(this)">
        <strong>Planet Earth II</strong> — 2024-11-15  
        <div class="stars">★★★★★</div>
        <div class="item-details">
            Stunning cinematography. Especially the mountain and desert ecosystems.
        </div>
    </div>
</div>

<!---------------- Movies ---------------->
<div id="movies" class="tab-content">
    <div class="item" onclick="toggleDetails(this)">
        <strong>Interstellar</strong> — 2024-12-05  
        <div class="stars">★★★★★</div>
        <div class="item-details">
            Beautiful blend of physics, emotion, and cinematography.  
            Loved the time-dilation sequences.
        </div>
    </div>

    <div class="item" onclick="toggleDetails(this)">
        <strong>Arrival</strong> — 2024-11-07  
        <div class="stars">★★★★★</div>
        <div class="item-details">
            A deep take on language, perception, and non-linear time.
        </div>
    </div>
</div>

<!---------------- Lectures ---------------->
<div id="lectures" class="tab-content">
    <div class="item" onclick="toggleDetails(this)">
        <strong>MIT 6.S191: Deep Learning Intro</strong> — 2024-12-10  
        <div class="stars">★★★☆☆</div>
        <div class="item-details">
            Good recap of fundamentals.  
            Covered backprop, computational graphs, and neural net basics.
        </div>
    </div>

    <div class="item" onclick="toggleDetails(this)">
        <strong>Andrew Ng: Machine Learning Foundations</strong> — 2024-10-22  
        <div class="stars">★★★★☆</div>
        <div class="item-details">
            Excellent clarity.  
            Great explanation of bias–variance and regularization.
        </div>
    </div>
</div>


<script>
    // Tab switching
    const tabs = document.querySelectorAll(".tab");
    const contents = document.querySelectorAll(".tab-content");

    tabs.forEach(tab => {
        tab.onclick = () => {
            tabs.forEach(t => t.classList.remove("active"));
            contents.forEach(c => c.classList.remove("active"));

            tab.classList.add("active");
            document.getElementById(tab.dataset.tab).classList.add("active");
        };
    });

    // Expand/collapse item details
    function toggleDetails(el) {
        const details = el.querySelector(".item-details");
        details.style.display = details.style.display === "block" ? "none" : "block";
    }
</script>
