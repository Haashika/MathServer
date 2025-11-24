# Ex.04 Design a Website for Server Side Processing
## Date:09-10-2025

## AIM:
To create a web page to calculate vehicle mileage and fuel efficiency using server-side scripts.

## FORMULA:
M = D / F
<br> M --> Mileage (in km/l)
<br> D --> Distance Travelled (in km)
<br> F --> Fuel Consumed (in l)

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM:
```html
<html>
<head>
    <title>Mileage Calculator</title>
    <style>
        body {
            background: #2b134b;
            font-family: Georgia, serif;
        }

        h1 {
            border: 2px solid #a56bff;
            padding: 20px;
            margin: 10px;
            border-radius: 5px;
            position: fixed;
            top: 150px;
            right: 430px;
            left: 430px;
            text-align: center;
            font-size: xx-large;
            font-weight: bold;
            font-variant: small-caps;
            background: linear-gradient(to right, #6d3ebc, #b084ff, #6d3ebc);
            color: #ffffff;
            box-shadow: 0px 0px 15px rgba(255,255,255,0.2);
        }

        form {
            border: 2px solid #c09bff;
            background-color: rgba(255, 255, 255, 0.07);
            padding: 30px;
            margin: 10px;
            border-radius: 10px;
            width: 425px;
            position: fixed;
            top: 260px;
            left: 520px;
            backdrop-filter: blur(4px);
        }

        label {
            color: white;
            font-size: 16px;
            font-weight: bold;
        }

        input[type="text"] {
            width: 220px;
            padding: 8px;
            margin-left: 10px;
            background: #ffffff;
            border: none;
            border-radius: 5px;
        }

        input[type="submit"] {
            padding: 10px 20px;
            background-color: #b98aff;
            border: none;
            border-radius: 6px;
            margin-top: 10px;
            cursor: pointer;
            font-weight: bold;
        }

        input[type="submit"]:hover {
            background-color: #d6baff;
        }
    </style>
</head>

<body>
    <h1> Mileage Calculator </h1>

    <form align="center" method="POST">
        {% csrf_token %}
         
        <div class="power">
            <label for="distance">DISTANCE (km):</label>
            <input type="text" name="distance" id="distance" value="{{d}}">
        </div>

        <br>

        <div class="power">
            <label for="fuel">FUEL (liters):</label>
            <input type="text" name="fuel" id="fuel" value="{{f}}">
        </div>

        <br>

        <input type="submit" value="CALCULATE">

        <br><br>

        <div class="power">
            <label for="mileage">MILEAGE:</label>
            <input type="text" name="mileage" id="mileage" value="{{mileage}}">
        </div>
    </form>
</body>
</html>
```
## OUTPUT - SERVER SIDE:

<img width="1919" height="1138" alt="image" src="https://github.com/user-attachments/assets/5a2db148-6853-45b8-93ee-2f9656dd9e8c" />

## OUTPUT - WEBPAGE:

<img width="1858" height="1086" alt="image" src="https://github.com/user-attachments/assets/8a750aac-c8fe-4bde-a53b-ad489cd17110" />

## RESULT:
The a web page to calculate vehicle mileage and fuel efficiency using server-side scripts is created successfully.
