<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Volta pra mim?</title>
    <script></script>
</head>

<body>
    <div id="content">
        <h2>Volta pra mim?</h2>
        <button class="btn" onclick="sim()">SIM</button>
        <button class="btn" onclick="desvia(this)" onmouseover="desvia(this)">NÃO</button>
    </div>
</body>

<style>
    #content {
        background: #7cbf99;
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        padding: 10px;
        text-align: center;
        font-family: sans-serif;
    }

    .btn {
        background: #000000;
    color: white;
    border: none;
    padding: 10px;
    width: 80px;
    border-radius: 5px;
    }
</style>

<script>
    function sim() {
        alert("te amo um monte, tava morrendo de saudade! <3 - Mai")
    }

    function desvia(t) {
        var btn = t;
        btn.style.position = 'absolute';
        btn.style.bottom = geraPosicao(10, 90);
        btn.style.left = geraPosicao(10, 90);
        console.log("Opa, desviei...");
    }

    function geraPosicao(min, max) {
        return (Math.random() * (max - min) + min) + "%";
    }

</script>

</html>
