---
layout: single
title: Watch Log
---

<style>
    .watch-log-tabs {display:flex; margin-bottom: 1rem; border-bottom: 2px solid #ccc; }
    .watch-log-tabs .tab {
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


<div class="watch-log-tabs">
    <div class="tab active" data-tab="documentary">Documentaries</div>
    <div class="tab" data-tab="movies">Movies</div>
    <div class="tab" data-tab="lectures">Lectures</div>
</div>

<!---------------- Documentary ---------------->
<div id="documentary" class="tab-content active">
    <div class="item" onclick="toggleDetails(this)">
        <strong>Raam ke Naam</strong> 
        <div class="stars">★★★★★</div>
        <div class="item-details">
            An exhaustive coverage of the events that lead to the demolition of Babari Mosque, in Ayodhya, India. Watch <a href="https://www.youtube.com/watch?v=GMT18TMNQbY&pp=ygUjaW4gdGhlIG5hbWUgb2YgZ29kIGFuYW5kIHBhdHdhcmRoYW4%3D">here</a> on YouTube. 
        </div>
    </div>

    <div class="item" onclick="toggleDetails(this)">
        <strong>Final Solution</strong> 
        <div class="stars">★★★★★</div>
        <div class="item-details">
            An exhaustive coverage of the events, pre- and post- Gujrat Riots of 2002. Watch <a href="https://www.youtube.com/watch?v=AV7rmuWefQI">here </a> on YouTube. 
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
