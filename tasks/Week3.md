[<kbd> <br> Home <br> </kbd>](../README.md) [<kbd> <br> Week 2 <br> </kbd>](Week2.md) [<kbd> <br> Week 3 <br> </kbd>](Week3.md) [<kbd> <br> Week 4 <br> </kbd>](Week4.md) [<kbd> <br> Week 5 <br> </kbd>](Week5.md) [<kbd> <br> Week 7 <br> </kbd>](Week7.md) [<kbd> <br> Week 8 <br> </kbd>](Week8.md) [<kbd> <br> Week 9 <br> </kbd>](Week9.md) [<kbd> <br> Week 10 <br> </kbd>](Week10.md) 

<html>
<body>

  <h1>Week 3</h1>

  <h2>Generating musicXML and MEI files</h2>
  <p>Download my MusicXML file <a href="../data/Summer.musicxml">here!</a>
  Download my MEI file <a href="../data/Summer.mei">here!</a>
  
  </p>
    <script type="module">
        import 'https://www.verovio.org/javascript/app/verovio-app.js';
        const options = {
            defaultView: 'responsive', // default is 'responsive', alternative is 'document'
            defaultZoom: 3, // 0-7, default is 4
            enableResponsive: true, // default is true
            enableDocument: true // default is true
        }
        // A MusicXML file
        var file = 'data/summer.mei';
        // A MEI file
        //var file = 'https://www.verovio.org/editor/brahms.mei';
        const app = new Verovio.App(document.getElementById("app"), options);
        fetch(file)
            .then(function(response) {
                return response.text();
            })
            .then(function(text) {
                app.loadData(text);
            });
    </script>
</body>
</html>
