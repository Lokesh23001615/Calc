# Ex.08 Design of a Standard Calculator
## Date:23.04.2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
calc.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
        <h2>LOKESH M (212223230114)<h2>

<div class="calculator">
    <input type="text" id="display" readonly>
    <br>
    <input type="button" value="7" onclick="appendToDisplay('7')">
    <input type="button" value="8" onclick="appendToDisplay('8')">
    <input type="button" value="9" onclick="appendToDisplay('9')">
    <input type="button" value="+" onclick="appendToDisplay('+')">
    <br>
    <input type="button" value="4" onclick="appendToDisplay('4')">
    <input type="button" value="5" onclick="appendToDisplay('5')">
    <input type="button" value="6" onclick="appendToDisplay('6')">
    <input type="button" value="-" onclick="appendToDisplay('-')">
    <br>
    <input type="button" value="1" onclick="appendToDisplay('1')">
    <input type="button" value="2" onclick="appendToDisplay('2')">
    <input type="button" value="3" onclick="appendToDisplay('3')">
    <input type="button" value="*" onclick="appendToDisplay('*')">
    <br>
    <input type="button" value="C" onclick="clearDisplay()">
    <input type="button" value="0" onclick="appendToDisplay('0')">
    <input type="button" value="=" onclick="calculate()">
    <input type="button" value="/" onclick="appendToDisplay('/')">
</div>

<script src="index.js"></script>

</body>
</html>


style.css

body {
    font-family: Arial, sans-serif;
    text-align: center;
}
.calculator {
    width: 300px;
    margin: 50px auto;
    border: 1px solid white;
    background-color:bisque;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
.calculator input[type="button"] {
    width: 50px;
    height: 50px;
    background-color:darkseagreen;
    font-size: 20px;
    margin: 5px;
    cursor: pointer;
    border-radius: 5px;
    border: none;
    
}
.calculator input[type="text"] {
    width: 100%;
    height: 50px;
    background-color: white;
    font-size: 24px;
    margin-bottom: 10px;

}


index.js

function appendToDisplay(value) {
    document.getElementById('display').value += value;
}

function clearDisplay() {
    document.getElementById('display').value = '';
}

function calculate() {
    try {
        var result = eval(document.getElementById('display').value);
        document.getElementById('display').value = result;
    } catch (error) {
        document.getElementById('display').value = 'Error';
    }
}

```

## OUTPUT:

![alt text](<Screenshot 2024-04-23 201310-1.png>)

![alt text](<Screenshot 2024-04-23 201320-1.png>)
## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
