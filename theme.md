---
title: Light/Dark Mode Example
---

<h2>Light/Dark Mode Toggle</h2>

<button id="toggle-theme">Toggle Light/Dark Mode</button>

<script>
    const button = document.getElementById('toggle-theme');
    const body = document.body;

    button.addEventListener('click', () => {
        body.classList.toggle('dark-mode');
        if (body.classList.contains('dark-mode')) {
            button.textContent = 'Switch to Light Mode';
        } else {
            button.textContent = 'Switch to Dark Mode';
        }
    });
</script>

<style>
    body {
        font-family: Arial, sans-serif;
        transition: background-color 0.3s ease, color 0.3s ease;
    }

    .dark-mode {
        background-color: #333;
        color: #fff;
    }

    #toggle-theme {
        padding: 10px 20px;
        margin-top: 20px;
        cursor: pointer;
        background-color: #007bff;
        color: #fff;
        border: none;
        border-radius: 5px;
    }

    #toggle-theme:hover {
        background-color: #0056b3;
    }
</style>
