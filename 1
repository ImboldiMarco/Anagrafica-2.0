<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Anagrafica 2.0</title>

  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f5f6fa;
      color: #2f3640;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #273c75;
      color: white;
      text-align: center;
      padding: 20px 0;
      font-size: 1.8em;
      font-weight: bold;
      letter-spacing: 1px;
    }

    main {
      width: 80%;
      margin: 30px auto;
      background: white;
      padding: 20px 30px;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }

    .controls {
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      justify-content: center;
      margin-bottom: 25px;
    }

    .controls div {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    label {
      font-weight: bold;
    }

    input {
      padding: 6px 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    button {
      background-color: #40739e;
      color: white;
      border: none;
      border-radius: 5px;
      padding: 7px 15px;
      cursor: pointer;
      transition: background-color 0.2s;
    }

    button:hover {
      background-color: #487eb0;
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 15px;
      text-align: center;
    }

    th {
      background-color: #273c75;
      color: white;
      padding: 10px;
    }

    td {
      border-bottom: 1px solid #ddd;
      padding: 8px;
    }

    tr:nth-child(even) {
      background-color: #f0f3f8;
    }

    tr:hover {
      background-color: #dcdde1;
    }
  </style>
</head>

<body>
  <header>Anagrafica 2.0</header>

  <main>
    <div class="controls">
      <div>
        <label>Ricerca per età minima:</label>
        <input type="number" id="anni" placeholder="es. 30">
        <button onclick="ricercaEta()">Cerca</button>
      </div>

      <div>
        <label>Ricerca per iniziale cognome:</label>
        <input type="text" id="iniziale" maxlength="1" placeholder="es. R">
        <button onclick="ricercaIniziale()">Cerca</button>
      </div>

      <div>
        <button onclick="generazione()">Mostra Generazione</button>
      </div>

      <div>
        <button onclick="inizio()">Tabella Completa</button>
      </div>
    </div>

    <table id="demo"></table>
  </main>

  <script>
    var xmlhttp = new XMLHttpRequest();
    var stampa = "", stampa2 = "", stampa3 = "", stampa4 = "", x = 0;

    // Mostra tabella iniziale
    xmlhttp.open("GET", "elenco.xml", true);
    xmlhttp.send();
    xmlhttp.onreadystatechange = function() {
      if (xmlhttp.readyState == 4 && xmlhttp.status == 200) {
        var xmlDoc = xmlhttp.responseXML;
        var persone = xmlDoc.getElementsByTagName("persona");
        for (x = 0; x < persone.length; x++) {
          var nome = persone[x].getElementsByTagName("nome")[0].childNodes[0].nodeValue;
          var cognome = persone[x].getElementsByTagName("cognome")[0].childNodes[0].nodeValue;
          var anni = persone[x].getElementsByTagName("anni")[0].childNodes[0].nodeValue;
          var DN = persone[x].getElementsByTagName("DN")[0].childNodes[0].nodeValue;
          stampa += `<tr><td>${nome}</td><td>${cognome}</td><td>${anni}</td><td>${DN}</td></tr>`;
        }
        document.getElementById("demo").innerHTML = `<tr><th>Nome</th><th>Cognome</th><th>Anni</th><th>Data di nascita</th></tr>${stampa}`;
        stampa = "";
      }
    };

    // Tabella completa
    function inizio() {
      var req = new XMLHttpRequest();
      req.open("GET", "elenco.xml", true);
      req.send();
      req.onreadystatechange = function() {
        if (req.readyState == 4 && req.status == 200) {
          var xmlDoc = req.responseXML;
          var persone = xmlDoc.getElementsByTagName("persona");
          for (x = 0; x < persone.length; x++) {
            var nome = persone[x].getElementsByTagName("nome")[0].childNodes[0].nodeValue;
            var cognome = persone[x].getElementsByTagName("cognome")[0].childNodes[0].nodeValue;
            var anni = persone[x].getElementsByTagName("anni")[0].childNodes[0].nodeValue;
            var DN = persone[x].getElementsByTagName("DN")[0].childNodes[0].nodeValue;
            stampa += `<tr><td>${nome}</td><td>${cognome}</td><td>${anni}</td><td>${DN}</td></tr>`;
          }
          document.getElementById("demo").innerHTML = `<tr><th>Nome</th><th>Cognome</th><th>Anni</th><th>Data di nascita</th></tr>${stampa}`;
          stampa = "";
        }
      };
    }

    // Ricerca per età
    function ricercaEta() {
      var minEta = document.getElementById("anni").value;
      document.getElementById("anni").value = "";
      var r = new XMLHttpRequest();
      r.open("GET", "elenco.xml", true);
      r.send();
      r.onreadystatechange = function() {
        if (r.readyState == 4 && r.status == 200) {
          var xmlDoc = r.responseXML;
          var persone = xmlDoc.getElementsByTagName("persona");
          for (x = 0; x < persone.length; x++) {
            var cognome = persone[x].getElementsByTagName("cognome")[0].childNodes[0].nodeValue;
            var anni = persone[x].getElementsByTagName("anni")[0].childNodes[0].nodeValue;
            if (anni >= minEta) {
              stampa2 += `<tr><td>${cognome}</td><td>${anni}</td></tr>`;
            }
          }
          document.getElementById("demo").innerHTML = `<tr><th>Cognome</th><th>Anni</th></tr>${stampa2}`;
          stampa2 = "";
        }
      };
    }

    // Ricerca per iniziale cognome
    function ricercaIniziale() {
      var iniziale = document.getElementById("iniziale").value.toUpperCase();
      document.getElementById("iniziale").value = "";
      var z = new XMLHttpRequest();
      z.open("GET", "elenco.xml", true);
      z.send();
      z.onreadystatechange = function() {
        if (z.readyState == 4 && z.status == 200) {
          var xmlDoc = z.responseXML;
          var persone = xmlDoc.getElementsByTagName("persona");
          for (x = 0; x < persone.length; x++) {
            var nome = persone[x].getElementsByTagName("nome")[0].childNodes[0].nodeValue;
            var cognome = persone[x].getElementsByTagName("cognome")[0].childNodes[0].nodeValue;
            var anni = persone[x].getElementsByTagName("anni")[0].childNodes[0].nodeValue;
            var DN = persone[x].getElementsByTagName("DN")[0].childNodes[0].nodeValue;
            if (cognome.startsWith(iniziale)) {
              stampa3 += `<tr><td>${nome}</td><td>${cognome}</td><td>${anni}</td><td>${DN}</td></tr>`;
            }
          }
          document.getElementById("demo").innerHTML = `<tr><th>Nome</th><th>Cognome</th><th>Anni</th><th>Data di nascita</th></tr>${stampa3}`;
          stampa3 = "";
        }
      };
    }

    // Tabella con generazione
    function generazione() {
      var g = new XMLHttpRequest();
      g.open("GET", "elenco.xml", true);
      g.send();
      g.onreadystatechange = function() {
        if (g.readyState == 4 && g.status == 200) {
          var xmlDoc = g.responseXML;
          var persone = xmlDoc.getElementsByTagName("persona");
          for (x = 0; x < persone.length; x++) {
            var nome = persone[x].getElementsByTagName("nome")[0].childNodes[0].nodeValue;
            var cognome = persone[x].getElementsByTagName("cognome")[0].childNodes[0].nodeValue;
            var anni = persone[x].getElementsByTagName("anni")[0].childNodes[0].nodeValue;
            var DN = persone[x].getElementsByTagName("DN")[0].childNodes[0].nodeValue;
            var gen = "";
            if (DN >= 2013) gen = "Generazione Alpha";
            else if (DN >= 1997) gen = "Generazione Z";
            else if (DN >= 1981) gen = "Millennials";
            else if (DN >= 1965) gen = "Generazione X";
            else if (DN >= 1946) gen = "Baby Boomers";
            else if (DN >= 1928) gen = "Generazione Silenziosa";
            else gen = "Greatest Generation";
            stampa4 += `<tr><td>${nome}</td><td>${cognome}</td><td>${anni}</td><td>${DN}</td><td>${gen}</td></tr>`;
          }
          document.getElementById("demo").innerHTML = `<tr><th>Nome</th><th>Cognome</th><th>Anni</th><th>Data di nascita</th><th>Generazione</th></tr>${stampa4}`;
          stampa4 = "";
        }
      };
    }
  </script>
</body>
</html>
