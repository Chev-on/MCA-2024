[<kbd> <br> Home <br> </kbd>](../README.md) [<kbd> <br> Week 2 <br> </kbd>](Week2.md) [<kbd> <br> Week 3 <br> </kbd>](Week3.md) [<kbd> <br> Week 4 <br> </kbd>](Week4.md)  [<kbd> <br> Week 5 <br> </kbd>](Week5.md) [<kbd> <br> Week 7 <br> </kbd>](Week7.md) [<kbd> <br> Week 8 <br> </kbd>](Week8.md) [<kbd> <br> Week 9 <br> </kbd>](Week9.md) [<kbd> <br> Week 10 <br> </kbd>](Week10.md) 

# Week 7

 To this week's MEI I have added genre and info for the creative commons licence. 

 .github.io/MCA-2024/metaRAW.html.

<html>
<head>
  <title>My Piece</title>
  <meta charset="utf-8">
  <link rel="stylesheet" href="css/myMeta.css" media="all" />
  <link rel="stylesheet" href="css/style.css" media="all" />
  <script src="js/CETEI.js"></script>
</head>
<body>
  <div id="MEImeta"></div>
  <div id="app" class="panel" style="border: 1px solid light gray; min-height: 800px;">Verovio is loading...</div>
  <div><p> To improve the presentation of the metadata, I would include more info about the metadata itself. As a list it is hard to tell which is a title, who actually composed the piece, who arranged the piece ect.

    I would also improve the formatting so it is more legible. 

    
  </p></div>
  <script type="module">
      import 'https://www.verovio.org/javascript/app/verovio-app.js';
        const app = new Verovio.App(document.getElementById("app"), {});

    // Load a file (MEI or MusicXML)
    fetch("data/Summer_wk7.mei")
        .then(function(response) {
            return response.text();
        })
        .then(function(text) {
            app.loadData(text);
        });
    </script>
  <script>
    // Get, parse, and show TEI data
    var CETEIcean = new CETEI()
    CETEIcean.getHTML5("data/Summer_wk7.mei", function(data) {
      document.getElementById("TEI").appendChild(data)
    })
    // Get, parse and show MEI header data
    var CETEI4MEI = new CETEI()
    CETEI4MEI.addBehaviors({
      namespaces: {
        mei: "http://www.music-encoding.org/ns/mei"
      }
    })
    CETEI4MEI.getHTML5("data/Summer_wk7.mei", function(data) {
      // get header
      var meiHead = data.querySelector('mei-meiHead')
      document.getElementById("MEImeta").appendChild(meiHead)
    })
    var vrvToolkit = new verovio.toolkit()
    vrvToolkit.setOptions(options = {
        pageHeight: 500,
        pageWidth: 1000,
        ignoreLayout: 1,
        border: 20,
        scale: 50,
        adjustPageHeight: true
    })
    fetch("data/Summer_wk7.mei").then(function( response ) {
        response.text().then(function( data ) {
          var svg = vrvToolkit.renderData(data, {})
          document.getElementById('MEI').innerHTML = svg
        })
    })
  </script>
</body>
<footer><p>Score rendering provided by <a href="http://www.verovio.org">Verovio</a>. Metadata rendered by <a href="https://github.com/TEIC/CETEIcean/"> CETEIcean</a>.</p></footer>
</html>
