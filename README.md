# Calculator
My First GitHub Project
[10/7/2026 8:30 PM] Baba Mehdi: <!DOCTYPE html>

<html>

<head>

    <title>My Calculator</title>

</head>

<body>

    <h1>My Calculator</h1>

    <input type="text" id="display" readonly>

    <br><br>

    <button onclick="clearDisplay()">C</button>

    <button onclick="addToDisplay('/')">÷</button>

    <button onclick="addToDisplay('*')">×</button>

    <button onclick="addToDisplay('-')">−</button>

    <br><br>

    <button onclick="addToDisplay('7')">7</button>

    <button onclick="addToDisplay('8')">8</button>

    <button onclick="addToDisplay('9')">9</button>

    <button onclick="addToDisplay('+')">+</button>

    <br><br>

    <button onclick="addToDisplay('4')">4</button>

    <button onclick="addToDisplay('5')">5</button>

    <button onclick="addToDisplay('6')">6</button>

    <br><br>

    <button onclick="addToDisplay('1')">1</button>

    <button onclick="addToDisplay('2')">2</button>

    <button onclick="addToDisplay('3')">3</button>

    <br><br>

    <button onclick="addToDisplay('0')">0</button>

    <button onclick="calculate()">=</button>

    <script>

        function addToDisplay(value) {

            document.getElementById("display").value += value;

        }

        function clearDisplay() {

            document.getElementById("display").value = "";

        }

        function calculate() {

            let expression = document.getElementById("display").value;

            document.getElementById("display").value = eval(expression);

        }

    </script>

</body>

</html>
