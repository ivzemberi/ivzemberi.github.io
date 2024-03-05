---
title: "Flutter App: whodunit"
subtitle: Murder Mystery Chat Game
layout: page
show_sidebar: false
hero_image: /images/whodunit-hero.png
hero_darken: true
---

<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
<body>
    <div class="section is-centered" style="font-size: large">
        <h3 class="is-size-4-mobile">Project Summary</h3>
        <div class="columns is-centered">
            <div class="column">
                <p>whodunit follows a compelling murder mystery storyline inspired by the book “And Then There Were None” 
                by Agatha Christie. Users can engage in a series of chat conversations with various characters involved 
                in the story to solve the murder case.
                </p>
                <figure>
                <a href="/images/whodunit-feature-graphics.png">
                    <img src="/images/whodunit-feature-graphics.png" alt="App screenshots.">
                </a>
                </figure>
            </div>
            <div class="column">
                <center>
                <video controls autoplay muted>
                    <source src="/videos/whodunit-demo.mp4" type="video/mp4">
                </video></center>
            </div>
        </div>
    </div>
        <div class="section is-centered" style="font-size: large">
        <h3 class="is-size-4-mobile">About the project</h3>
        <p>The app was developed for a course Mobile App Development at Uni Bremen in the Winter Semester 2023/24. 
        I developed it together with Yuliya Litvin and Srujana Madam Sampangiramu. My tasks included:
            <ul>
                <li>Creating an adaptive launcher app icon and a monochrome icon</li>
                <li>Implementing the Introduction Story Screen with text animations</li>
                <li>Implementing an overlay explaining where to start the game on the first run of the app</li>
                <li>Establishing connection to Firebase and saving chats there</li>
                <li>Prompt engineering the initial context for each character</li>
                <li>Generating UUIDs on the first run of the app</li>
            </ul>
        </p>
        <figure class="is-desktop is-hidden-mobile">
        <a href="/images/whodunit-features.png">
            <img src="/images/whodunit-features.png" height="60%" width="60%" alt="App features displayed.">
        </a>
        </figure>
        <figure class="is-mobile is-hidden-tablet is-hidden-desktop">
            <a href="/images/whodunit-features.png">
                <img src="/images/whodunit-features.png" alt="App features displayed.">
            </a>
        </figure>
    </div>
    <div class="section is-centered" style="font-size: large">
        <h3 class="is-size-4-mobile">Launcher icons</h3>
        <p>The launcher icons follow the murder mystery game theme but their style is still flat and minimalistic.
        </p>
        <figure>
        <a href="/images/whodunit-icons.png">
            <img src="/images/whodunit-icons.png" alt="whodunit launcher icons.">
        </a>
        </figure>
    </div>
    <div class="section is-centered" style="font-size: large">
    <h3 class="is-size-4-mobile">Tools, Frameworks & Technologies</h3>
            <ul style="list-style-type:none">
                <div class="columns">
                    <div class="column">
                    <li><span class="icon"><i class="fas fa-arrow-right"></i></span>
                    <strong> Figma</strong></li>
                    <li><span class="icon"><i class="fas fa-arrow-right"></i></span> 
                    <strong> Inkscape</strong></li>
                    <li><span class="icon"><i class="fas fa-arrow-right"></i></span>
                    <strong> Android Studio</strong></li>
                </div>
                <div class="column">
                    <li><span class="icon"><i class="fas fa-arrow-right"></i></span>
                    <strong> Flutter + Dart</strong></li>
                    <li><span class="icon"><i class="fas fa-arrow-right"></i></span>
                    <strong> Firebase Console</strong></li>
                    <li><span class="icon"><i class="fas fa-arrow-right"></i></span>
                    <strong> OpenAI API</strong></li>
                </div>
                </div>
            </ul>
    </div>
</body>
</html>