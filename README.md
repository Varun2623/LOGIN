<!DOCTYPE html>
<html>
<head>
    <title>GitHub Collaboration Demo</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
            margin-top: 50px;
        }
        .container {
            background: white;
            width: 400px;
            margin: auto;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0px 0px 10px gray;
        }
        input, button {
            padding: 8px;
            margin: 8px 0;
            width: 90%;
        }
        button {
            background-color: #007bff;
            color: white;
            border: none;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
        #output {
            margin-top: 15px;
            font-weight: bold;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>GitHub Collaboration Project</h2>
    <p>Simple Feature Added Using Branch & Pull Request</p>

    <input type="text" id="name" placeholder="Enter your name">
    <button onclick="greetUser()">Generate Greeting</button>

    <div id="output"></div>
</div>

<script>
    function greetUser() {
        var name = document.getElementById("name").value;

        if (name === "") {
            document.getElementById("output").innerHTML = "Please enter your name!";
        } else {
            document.getElementById("output").innerHTML =
                "Hello, " + name + "! Welcome to the GitHub collaboration demo.";
        }
    }
</script>

</body>
</html>
