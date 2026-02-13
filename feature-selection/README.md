    Your page should have an h1 element with the text Feature Selection.
    Your page should have a div element with the class feature-card-container.
    Your page should have at least two label elements each with the class feature-card inside the div.
    Each of your label elements should have label text and an input element of type checkbox in them.
    Create a selector that targets the checkboxes, and apply the following styling:
        All of your checkbox elements should be set to appearance: none; in your CSS.
        All of your checkbox elements should have a border width, color and style of your choosing.
    When the checkbox is checked, it should display a checkmark ✓ in the center of the checkbox.
    When the checkbox is checked, the background color of the checkbox should change to a color of your choosing.
    When the checkbox is checked, the border color of the checkbox should change to a color of your choosing.

Note: Be sure to link your CSS file in your HTML.

// running tests 13. When the checkboxes are selected, there should be a checkmark ✓ in the center of the checkbox. 14. When the checkbox is checked, the background color of the checkbox should change to a color of your choosing. 15. When the checkbox is checked, the border color of the checkbox should change to a color of your choosing.
// tests completed

<!--codigo original-->

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Feature Selection Page</title>
  <link rel="stylesheet" href="styles.css">
</head>

<body>
  <h1>Feature Selection</h1>
  <div class="feature-card-container">

    <label for="adult-channel" class="feature-card">Adult Channel
      <input type="checkbox" value="" id="adult-channel">
    </label>

    <label for="teen-channel" class="feature-card">Teen Channel
      <input type="checkbox" value="1" id="teen-channel">
    </label>

    <label for="children-channel" class="feature-card">Children Channel
      <input type="checkbox" value="2" id="children-channel">
    </label>

    <label for="family-channel" class="feature-card">Family Channel
      <input type="checkbox" value="3" id="family-channel">
    </label>

    <label for="sports-shannel" class="feature-card">Sports Channel
      <input type="checkbox" value="4" id="sports-shannel">
    </label>

    <label for="news-channel" class="feature-card">News Channel
      <input type="checkbox" value="5" id="news-channel">
    </label>

  </div>

</body>
</html>

<!--codigo css-->

- {
  padding: 0;
  border: 0;
  }

h1 {
text-align: center;
margin: 50px auto 5px;
}

body {
display: flex;
justify-content: center;
align-items: center;
flex-direction: column;
height: 100vh;
}

.feature-card {
display: flex;
align-items: center;
padding: 5px;
border: 1px solid lawngreen;
margin: 15px;
cursor: pointer;
}

.feature-card-container {
margin-top: 1px;
border: 1px solid black;
border-radius: 15px solid black;
margin-bottom: auto;
}

input[type="checkbox"] {
width: 15px;
height: 15px;
border: 1px solid gray;
display: flex;
margin: auto;
cursor: pointer;
}

.input[type="checkbox"]:checked + label::after {
content: "✓";
display: inline-block;
font-size: 18px;
color: #0fbf12;
margin-left: -22px;
margin-top: -2px;
cursor: pointer;
background-color: bisque;
}

<!-- html -->

- {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  }

h1 {
text-align: center;
margin: 50px auto 5px;
}

body {
display: flex;
justify-content: center;
align-items: center;
flex-direction: column;
height: 100vh;
}

.feature-card {
display: flex;
align-items: center;
padding: 5px;
border: 1px solid lawngreen;
margin: 15px;
cursor: pointer;
position: relative;
}

.feature-card-container {
margin-top: 1px;
border: 1px solid black;
border-radius: 15px;
margin-bottom: auto;
}

input[type="checkbox"] {
appearance: none;
-webkit-appearance: none;
-moz-appearance: none;
position: absolute;
opacity: 0;
width: 0;
height: 0;
cursor: pointer;
}

.custom-checkbox {
display: inline-block;
width: 15px;
height: 15px;
margin: 0 0 0 10px;
border: 1px solid gray;
border-radius: 2px;
transition: all 0.2;
}

.custom-checkbox::after {
content: "✓";
position: absolute;
/_ top: 50%;
left: 50%; _/
transform: translate(-50%, 50%);
font-size: 12px;
font-weight: bold;
color: white;
opacity: o;
transition: opacity 0.2 ease;
}

.input[type="checkbox"]:checked + .custom-checkbox {
background-color: azure;
border-color: aqua;
}

.input[type="checkbox"]:checked + .custom-checkbox::after {
opacity: 1;
}

<!-- css -->

- {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  }

h1 {
text-align: center;
margin: 50px auto 5px;
}

body {
display: flex;
justify-content: center;
align-items: center;
flex-direction: column;
height: 100vh;
}

.feature-card {
display: flex;
align-items: center;
padding: 5px;
border: 1px solid lawngreen;
margin: 15px;
cursor: pointer;
position: relative;
}

.feature-card-container {
margin-top: 1px;
border: 1px solid black;
border-radius: 15px;
margin-bottom: auto;
}

input[type="checkbox"] {
appearance: none;
-webkit-appearance: none;
-moz-appearance: none;
position: absolute;
opacity: 0;
width: 0;
height: 0;
cursor: pointer;
}

.custom-checkbox {
display: inline-block;
width: 15px;
height: 15px;
margin: 0 0 0 10px;
border: 1px solid gray;
border-radius: 2px;
transition: all 0.2;
}

.custom-checkbox::after {
content: "✓";
position: absolute;
/_ top: 50%;
left: 50%; _/
transform: translate(-50%, 50%);
font-size: 12px;
font-weight: bold;
color: white;
opacity: o;
transition: opacity 0.2 ease;
}

.input[type="checkbox"]:checked + .custom-checkbox {
background-color: azure;
border-color: aqua;
}

.input[type="checkbox"]:checked + .custom-checkbox::after {
opacity: 1;
}

<!-- * {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

h1 {
  text-align: center;
  margin: 50px auto 5px;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}

.feature-card {
  display: flex;
  align-items: center;
  padding: 5px;
  border: 1px solid lawngreen;
  margin: 15px;
  cursor: pointer;
  position: relative;
}

.feature-card-container {
  margin-top: 1px;
  border: 1px solid black;
  border-radius: 15px;
  margin-bottom: auto;
}

input[type="checkbox"] {
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  position: absolute;
  opacity: 0;
  width: 0;
  height: 0;
  cursor: pointer;
}

.custom-checkbox {
  display: inline-block;
  width: 15px;
  height: 15px;
  margin: 0 0 0 10px;
  border: 1px solid gray;
  border-radius: 2px;
  transition: all 0.2s;
  position: relative;
}

.custom-checkbox::after {
  content: "✓";
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, 50%);
  font-size: 12px;
  font-weight: bold;
  color: white;
  opacity: 0;
  transition: opacity 0.2 ease;
}

input[type="checkbox"]:checked + .custom-checkbox {
  background-color: azure;
  border-color: aqua;
}

input[type="checkbox"]:checked + .custom-checkbox::after {
  opacity: 1;
}
 -->

 <!-- deepseek -->

- {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  }

h1 {
text-align: center;
margin: 50px auto 5px;
}

body {
display: flex;
justify-content: center;
align-items: center;
flex-direction: column;
height: 100vh;
}

.feature-card {
display: flex;
align-items: center;
padding: 5px;
border: 1px solid lawngreen;
margin: 15px;
cursor: pointer;
position: relative;
padding-left: 30px; /_ AÑADIDO: espacio para el checkbox _/
}

.feature-card-container {
margin-top: 1px;
border: 1px solid black;
border-radius: 15px;
margin-bottom: auto;
}

/_ Ocultar checkbox nativo _/
input[type="checkbox"] {
appearance: none;
-webkit-appearance: none;
-moz-appearance: none;
position: absolute;
left: 5px; /_ AÑADIDO: posicionar dentro del label _/
width: 15px;
height: 15px;
border: 1px solid gray;
background-color: white;
cursor: pointer;
border-radius: 2px;
}

/_ Checkmark usando ::before en el input - SOLUCIÓN SIMPLE _/
input[type="checkbox"]:checked {
background-color: #4caf50; /_ Color de fondo _/
border-color: #388e3c; /_ Color del borde _/
}

/_ O si prefieres usar el símbolo ✓ con ::before _/
input[type="checkbox"]:checked::before {
content: "✓";
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
color: white;
font-size: 10px;
font-weight: bold;
}
