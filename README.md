# temperature-converter
 By Using HTML, CSS, and JavaScript to convert temperature from Celsius to Fahrenheit

HTML:
<!DOCTYPE html>
<html>
<head>
  <title>Temperature Converter</title>
  <style>
    /* CSS goes here */
  </style>
</head>
<body>
  <h1>Temperature Converter</h1>

  <input type="number" id="celsius" placeholder="Enter Celsius temperature">
  <button type="button" onclick="convertCelsiusToFahrenheit()">Convert to Fahrenheit</button>

  <span class="output" id="fahrenheit"></span>

  <script>
    /* JavaScript goes here */
  </script>
</body>
</html>

CSS:
body {
  font-family: sans-serif;
}

input,
button {
  width: 100%;
  margin-bottom: 10px;
}

.output {
  font-size: 1.5em;
}

JAVASCRIPT :

function convertCelsiusToFahrenheit() {
  // Get the Celsius temperature from the input field.
  const celsius = parseFloat(document.getElementById("celsius").value);

  // Calculate the Fahrenheit temperature using the formula F = (C * 1.8) + 32.
  const fahrenheit = (celsius * 1.8) + 32;

  // Display the Fahrenheit temperature in the output field.
  document.getElementById("fahrenheit").innerHTML = fahrenheit + " &deg;F";
}
