[<kbd> <br> Home <br> </kbd>](../README.md) [<kbd> <br> Week 2 <br> </kbd>](Week2.md) [<kbd> <br> Week 3 <br> </kbd>](Week3.md) [<kbd> <br> Week 4 <br> </kbd>](Week4.md) [<kbd> <br> Week 5 <br> </kbd>](Week5.md) [<kbd> <br> Week 7 <br> </kbd>](Week7.md) [<kbd> <br> Week 8 <br> </kbd>](Week8.md) [<kbd> <br> Week 9 <br> </kbd>](Week9.md) [<kbd> <br> Week 10 <br> </kbd>](Week10.md) 

# Week 3 
## Generating musicXML and MEI files

 This week I converted my musescore file into musicXML and MEI files; <br>
  Download my MusicXML file <a href="../week3/Summer.musicxml">here!</a> <br>
  Download my MEI file <a href="../week3/Summer.mei">here!</a>


# Verovio

If below fails to load click to see my piece in <a href="../week3/verovio.html" target="_blank">Verovio!</a>


<head>
    <meta charset="utf-8">
    <title>My Piece in Verovio</title>
    <style>
    html, body {
        width: 100%;
        height: 100%;
        margin: 0;
    }
    .box {
        display: flex;
        flex-flow: column;
        height: 100%;
    }
    .box .header {
       flex: 0 1 auto;
    }
    .box #app {
        flex: 1 1 auto;
    }
    </style>
</head>
<body>
    <div class="box">
    <div class="header"><h1>Violin Concerto in G minor, 'Summer' - Antonio Vivaldi</h1>
        <p> </p></div>
    <div id="app">Verovio is loading...</div>
    <script type="module">
        import 'https://www.verovio.org/javascript/app/verovio-app.js';
        const options = {
            defaultView: 'responsive', // default is 'responsive', alternative is 'document'
            defaultZoom: 3, // 0-7, default is 4
            enableResponsive: true, // default is true
            enableDocument: true // default is true
        }
        // A MusicXML file
        var file = '../week3/Summer_verovio.mei';
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
    </div>
</body>

