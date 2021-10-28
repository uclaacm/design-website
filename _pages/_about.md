---
layout: page
title: ACM Design
permalink: "/about/"
---

<div class="about-main">
    <div id="form-follows">
        <span id="text1">Form</span>
        <img src ="/assets/logos/ipad.png" id="img1">
        <span id="text2">Follows</span>
        <img src ="/assets/logos/laptop.png" id="img2">
        <span id="text3">Function</span>
    </div>
    <div id="flexbox1">
        <img src="/assets/logos/quote.png" id="quote1">
        <p class = "about-us" id="aboutPar"><span class = "werd">ACM</span> <span class="werd" id="orange">Design</span> is the premier club on campus for learning graphic design and user experience. ACM Design was founded to develop guidelines, normalize branding, and produce design elements for UCLA ACM. <br><br>
Things we do include projects such as this website and the styleguide, as well as workshops for the general UCLA community!</p>
        <img src="/assets/logos/quote.png" id="quote2">
    </div>
    <h1 id="us">Who we are</h1>
    <div>
        <h3 id="title">Board</h3>
        <div class="headshots1">
            {% for person in card-board %}
                <div>
                    <img src="../assets/headshots/{{person.photo}}" class="headshot-board">
                    <span class="_caps">{{person.name}}</span>
                    <span class="_caps2">{{person.role}}</span>
                </div>
            {% endfor %}
        </div>
    </div>
    <div>
        <h3>Designers</h3>
        <div class="headshots1">
            {% for person in card-des %}
                <div class = "headshot-card">
                    <img src="../assets/headshots/{{person.photo}}" class="headshot-board">
                    <span class="_caps">{{person.name}}</span>
                    <span class="_caps2">{{person.role}}</span>
                </div>
            {% endfor %}
        </div>
    </div>
    <div>
        <h3>Developers</h3>
        <div class="headshots1">
            {% for person in card-dev %}
                <div>
                    <img src="../assets/headshots/{{person.photo}}" class="headshot-board">
                    <span class="_caps">{{person.name}}</span>
                    <span class="_caps2">{{person.role}}</span>
                </div>
            {% endfor %}
        </div>
    </div>
    <div>
        <h3>Alumni</h3>
        <div id="alumnis">
            <div class="alumns">Hakan Alpay</div>
            <div class="alumns">Jennifer Lin</div>
            <div class="alumns">Tomoki Fukazawa</div>
        </div>
    </div>
</div>