---
layout: page
title: ACM Design
permalink: "/about/"
---

<link rel="stylesheet/less" type="text/css" href="styles.less" />
<script src="less.js" type="text/javascript"></script>
<div>
    <div class="center" style="margin-top: 2.5em">    
        <img src="../assets/slogan.svg" 
        alt="Forms Follows Function with images of a laptop and a tablet">
    </div>
    <div>
        <p>
            ACM Design is the premier club on campus for learning graphic design and user experience. Lorem ipsum something something ACM Design started as something origin story is probably like a line or two.     
        </p>
        <p>
            Things we do include projects and stuff such as this website and the styleguide haha find it in projects or something something ok bye wee        
        </p>
    </div>
    <h1 class="center">Who we are </h1>
    <div style="margin-right: 15em ;margin-left: 15em">
        <h1>Board</h1>
        {% for person in card_board %}
        <div>
            <img src="../assets/headshots/{{person.photo}}">
            <p>{{person.name}}</p>
            <p>{{person.role}}</p>
        </div>
        {% endfor %}
    </div>
    <div style="margin-right: 15em ;margin-left: 15em">
        <h1>Designers</h1>
        {% for person in card_designer %}
        <div>
            <img src="../assets/headshots/{{person.photo}}">
            <p>{{person.name}}</p>
            <p>{{person.role}}</p>
        </div>
        {% endfor %}
    </div>
    <div style="margin-right: 15em ;margin-left: 15em">
        <h1>Developers</h1>
        {% for person in card_developer %}
        <div>
            <img src="../assets/headshots/{{person.photo}}">
            <p>{{person.name}}</p>
            <p>{{person.role}}</p>
        </div>
        {% endfor %}
    </div>
    <div style="margin-right: 15em ;margin-left: 15em">
        <h1>Emeritus</h1>
        {% for person in card_emeritus %}
        <div>
            <img src="../assets/headshots/{{person.photo}}">
            <p>{{person.name}}</p>
            <p>{{person.role}}</p>
        </div>
        {% endfor %}
    </div>
</div>
