<h1 align="center"> МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</h1>

<p align="center">Лабораторная работа №6 "JS" </p>

<p align="right">Выполнил: Алексеев Максим Максимович</p>
<p align="right">Проверил: Соболев Е. И.</p>

<p align="center">г. Южно-Сахалинск <br> 2023 год</p>

<h2 align="center">Введение</h2>
<p align="justify">Лабораторная работа по созданию скриптов на языке JavaScript.</p>

<h2>Цели и задачи</h2>
Сделать много чего.
<h2>Решение задач</h2>


```javascript
  
let count = 0;
function func2()
{
    let text = prompt("Изменение input");
    document.getElementById("input").value = text;
}

function func3()
{
    let text = document.getElementById("input").value;
    alert(text);
}

function func4()
{
    let num = parseInt(document.getElementById("input").value);
    alert(num * num);
}

function func5()
{
    let text = document.getElementById("input1").value; 
    document.getElementById("input1").value = document.getElementById("input2").value;
    document.getElementById("input2").value = text;
}

function func6()
{
    document.getElementById("button6").innerText = "Поменял текст";
}

function func7()
{
    document.getElementById("input3").style.color = 'red';
}

function inputon()
{
    document.getElementById("input4").removeAttribute('disabled');
}

function inputoff()
{
    document.getElementById("input4").setAttribute('disabled', '');
}

function func9()
{
    alert("Вы навели мышкой на кнопку!");
}

function func10()
{
    alert("Вы дважды нажали на кнопку!");
}

function func11()
{
    alert("Вы навели мышкой на элемент div!");
}

function func12()
{
    var element = document.getElementById("image");
    if(element.getAttribute('src') == "one.jpg")
        element.setAttribute('src','two.jpg');
    else 
        element.setAttribute('src','one.jpg');
}


function func15()
{
    this.setAttribute('disabled','');
}

function func16(element)
{
    count++;
    element.innerText = count.toString();
}

function func17()
{
    document.body.style.cursor = 'pointer';
}

function func18()
{
    document.getElementById('hide').style.visibility = 'hidden';
}

function sum(){
    let a = parseInt(document.getElementById('a').value);
    let b = parseInt(document.getElementById('b').value);
    document.getElementById('result').innerText = `${a} + ${b} = ${a+b}`;
}

function difference(){
    let a = parseInt(document.getElementById('a').value);
    let b = parseInt(document.getElementById('b').value);
    document.getElementById('result').innerText = `${a} - ${b} = ${a-b}`;
}

function multiply(){
    let a = parseInt(document.getElementById('a').value);
    let b = parseInt(document.getElementById('b').value);
    document.getElementById('result').innerText = `${a} * ${b} = ${a*b}`;
}

function division(){
    let a = parseInt(document.getElementById('a').value);
    let b = parseInt(document.getElementById('b').value);
    document.getElementById('result').innerText = `${a} / ${b} = ${a/b}`;
}

```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>lab6</title>
    <script src="script.js"></script>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <button onclick="alert('alert')">Задача 1</button><br>
    <div>
        <input type="text" id="input"/><br>
        <button onclick="func2()">Задача 2</button><br>
        <button onclick="func3()">Задача 3</button><br>
        <button onclick="func4()">Задача 4</button><br>
    </div>
    <div>
        <button onclick="func5()">Задача 5</button><br>
        <input type="text" id="input1"/><br>
        <input type="text" id="input2"/><br>
    </div>
    <button onclick="func6()" id="button6">Задача 6</button><br>
    <div>
        <button onclick="func7()">Задача 7</button><br>
        <input type="text" id="input3"/><br>
    </div>
    <div>
        <p>Задача №8</p>
        <input type="text" id="input4" /><br>
        <button onclick="inputon()">Включить</button>
        <button onclick="inputoff()">Выключить</button><br>
    </div>
    <button onmouseenter="func9()">Задача 9</button><br>
    <button ondblclick="func10()">Задача 10</button><br>
    <div onmouseenter="func11()" style="height: 100px; width: 100px;">
        <p>Задача 11</p>
    </div>
    <div>
        <p><img id="image" src="one.jpg"></p>
        <button onclick="func12()">Изменить</button><br>
    </div>
    <button onclick="alert(this)">Задача 13</button><br>
    <div>
        <p>Задача 14</p>
        <input type="text" id="input5" value="text">
        <button onclick="this.previousElementSibling.value = prompt()">change</button>
    </div>
    <button onclick="this.setAttribute('disabled','')">Задача 15</button><br>
    <button onclick="func16(this)">Задача 16</button><br>
    <button onclick="func17()">Задача 17</button><br>
    <div>
        <p>Задача 18</p>
        <input onclick="func18()" type="button" id="hider" value="Нажмите, чтобы спрятать текст"/> 
        <div id="hide">Текст</div> 
    </div>
    <button onclick="this.style.visibility = 'hidden'">Задача 19</button><br>
    <div>
        <p>Задача 20</p>
        <p>a: <input type="number" id="a"></p>
        <p>b: <input type="number" id="b"></p>
        <p><button onclick="sum()">+</button><button onclick="difference()">-</button></p>
        <p><button onclick="multiply()">*</button><button onclick="division()">/</button></p>
        <p id="result"></p>
    </div>
</body>
</html>
```

<h2>Вывод</h2>
Я научился скрипты hbs, pug и ejs.
