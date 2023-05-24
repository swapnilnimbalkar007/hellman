<html>

<head></head>

<body>
    <label for="">Enter P</label>
    <input type="text" id="p"> <br>
    <label for="">Enter G</label>
    <input type="text" name="" id="g"> <br>
    <label for="">deffi</label>
    <textarea name="" id="text" cols="30" rows="10" readonly></textarea>
    <button onclick="clickme()">getkey</button>

    <script>
        function isPrim(n) {

        }
        function clickme() {
            var p = document.getElementById("p").value;
            var g = document.getElementById("g").value;



            var privatekeyofallic = 10;
            var privatekeyofbob = 8;

            x = Math.pow(g, privatekeyofallic) % p;
            y = Math.pow(g, privatekeyofbob) % p;

            secretekeyofalic = Math.pow(y, privatekeyofallic) % p;
            secretekeyofbob = Math.pow(x, privatekeyofbob) % p;

            document.getElementById("text").value = "Secrete key of alic: " + secretekeyofalic + "\n" + "Secrete ket key of bob: " + secretekeyofbob
        }
    </script>
</body>

</html>
