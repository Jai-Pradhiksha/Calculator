# Ex.08 Design of a Standard Calculator
## Date:
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
### calculator.html
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <title>Jai Pradhiksha</title>
    <script>
        function fn(e) {
            if (e.innerHTML == '=') {

                output.value = eval(output.value);
            }
            else if (e.id == 'back') {
                v = output.value;
                output.value = v.substring(0, v.length - 1);
            }
            else if (e.innerHTML == 'C') {
                output.value = '';
            }
            else {
                output.value += e.innerHTML;
            }
        }
    </script>
</head>
<body style="background-color:rgb(124, 188, 249);">

    <div class="mx-auto text-center text-white"
        style="width:24rem; margin-top: 50px; padding-top: 20px; padding-bottom: 20px;">
        <b style="color: rgb(4, 4, 82); font-family: 'Times New Roman';">Jai Pradhiksha D P</b>
        <b style="color: rgb(4, 4, 82); font-family: 'Times New Roman';">(212221040062)</b>
    </div>
    <div class="row mx-auto text-center rounded-4" style="width:24rem; background-color:aliceblue; ">
        <div class="col-12 my-4"><input type="text" name="" id="output"
                style="width: 100%; height: 50px; border-radius: 25px;"></div>
        <div class="m-3 col-2 btn btn-outline-primary rounded-4" onclick="fn(this)">(</div>
        <div class="m-3 col-2 btn btn-outline-primary rounded-4" onclick="fn(this)">)</div>
        <div class="m-3 col-2 btn btn-outline-danger rounded-4" onclick="fn(this)">C</div>
        <div class="m-3 col-2 btn btn-outline-danger rounded-4" onclick="fn(this)" id="back"><i
                class="bi bi-backspace"></i>
        </div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">7</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">8</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">9</div>
        <div class="m-3 col-2 btn btn-outline-primary rounded-4" onclick="fn(this)">*</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">4</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">5</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">6</div>
        <div class="m-3 col-2 btn btn-outline-primary rounded-4" onclick="fn(this)">-</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">1</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">2</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">3</div>
        <div class="m-3 col-2 btn btn-outline-primary rounded-4" onclick="fn(this)">+</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">0</div>
        <div class="m-3 col-2 btn btn-outline-success rounded-4" onclick="fn(this)">.</div>
        <div class="m-3 col-2 btn btn-outline-primary rounded-4" onclick="fn(this)">%</div>
        <div class="m-3 col-2 btn btn-outline-primary rounded-4" onclick="fn(this)">/</div>
        <div class="m-3 col-11 btn btn-outline-warning rounded-4" onclick="fn(this)">=</div>
    </div>
</body>
</html>
```
## OUTPUT:
![image](https://github.com/Jai-Pradhiksha/Calculator/assets/100289733/aee8ce8a-cbd7-46c8-abf6-db4a2fa3dae6)
## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
