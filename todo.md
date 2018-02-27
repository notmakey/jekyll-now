---
layout: page
title: To-Do
permalink: /todo/
---

function save(){
    var checkbox = document.getElementById('checkbox1zaal1');
    localStorage.setItem('checkbox1zaal1', checkbox.checked);
}

function load(){    
    var checked = JSON.parse(localStorage.getItem('checkbox1zaal1'));
    document.getElementById("checkbox1zaal1").checked = checked;
}

function wis(){
    location.reload();
    localStorage.clear()

}

load();

<input type="button" id="ReserveerButton1" value="save" onclick="save()"/>
<input type="button" id="Wisbutton1" value="delete" onclick="wis()"/>
<input type="checkbox" id="checkbox1zaal1">1e film van de dag</input>

