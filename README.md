# Be-my-Valentine
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Valentine Proposal 💖</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
        background-color: #ffe6eb;
        height: 100vh;
        overflow: hidden;
    }

    h1 {
        margin-top: 100px;
        color: #d6336c;
    }

    button {
        font-size: 20px;
        padding: 12px 25px;
        margin: 20px;
        border: none;
        border-radius: 8px;
        cursor: pointer;
    }

    #yes {
        background-color: #28a745;
        color: white;
    }

    #no {
        background-color: #dc3545;
        color: white;
        position: absolute;
    }
</style>
</head>
<body>

<h1>Will you be my Valentine? 💘</h1>

<button id="yes" onclick="yesClicked()">Yes 💕</button>
<button id="no" onmouseover="moveNo()">No 😜</button>

<script>
    function moveNo() {
        const noBtn = document.getElementById("no");
        const x = Math.random() * (window.innerWidth - 100);
        const y = Math.random() * (window.innerHeight - 100);
        noBtn.style.left = x + "px";
        noBtn.style.top = y + "px";
    }

    function yesClicked() {
        document.body.innerHTML = "<h1>Yay! 💖 I knew it 😍</h1><p>Happy Valentine’s Day ❤️</p>";
    }
</script>

</body>
</html>
