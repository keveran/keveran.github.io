  <!DOCTYPE html>
<html lang="da" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Socialdemokratiet</title>
    <link href="https://fonts.googleapis.com/css?family=Reem+Kufi|Roboto&display=swap" rel="stylesheet">
    <link rel="shortcut icon" href="../images/logo.ico">
  </head>
  <body>

                                                                    <!-- CSS -->

    <style media="screen">
      * {
        font-family: 'Reem Kufi';
      }

      header {                     /* Header */
        background-color: #DF594E;
        display: flex;
        flex-direction: row;
      }

      #logotop {
        padding: 10px;
      }

      nav ul {
        display: flex;
        flex-direction: row;
        background-color: white;
        list-style: none;
        width: 100%;

        box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
      }

      nav ul li {
        padding-right: 20px;
      }

      nav ul li a {
        padding-right: 20px;
        text-decoration: none;
        color: #DF594E;
      }

      #motto {
        font-size: 16pt;
        color:  white;
      }

      h1 {
        color: white;

      }

      #search1 {
        height: 100%;
      }

      footer {                      /* Footer */
        width: 100%;
        height: 165px;

        margin: 0;
        padding: 0;

        display: flex;
        flex-direction: row;
        justify-content: center;
        background-color: #F2F2F2;
        position: sticky;
      }

      #search2 {
        height: 30px;
        width: 150px;

        border: 0.5px solid #BDBDBD;
        box-sizing: border-box;
      }

      .bottomnav ul li a {
        text-decoration: none;
      }

      .bottomnav ul li {
        list-style: none;
      }

      #tilmeld {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 30%;
        text-align: center;
        height: 100%;
        padding: 0;
        margin: 0;
      }

      #tilmelddigher {
        font-weight: normal;
        font-size: 20px;
        line-height: 21px;

      }

      .tilmeldInput {
        text-align: center;
        width: 170px;
        height: 100%;
      }

      #tilmeldknap {
        background-color: black;
        color: white;
        width: 150px;
        border: none;
        margin: 0;
        font-family: Roboto;
        height: 25px;
      }

      #copyrighttext {
        width: 20%;
      }

      #logobot {
        width: 100px;
        height: 100px;
        padding: 10px;
      }

      .billedHjul {
        width: 500px;
      }

      #left {
        height: 50px;
        align-self: center;
        position: absolute;
        right: 465px;
      }

      #right {
        height: 50px;
        align-self: center;
        position: absolute;
        right: 0px;
      }

      .billedhjulDiv {
        display: flex;
        position: relative;
        width: 500px;
      }

      #socialMedia {
        list-style: none;
      }

      #socialMedia li a {
        text-decoration: none;
        color: black;
      }



    </style>

                                                             <!-- JavaScript -->



    <header>
      <a href="index.html"><img src="../images/logo.png" alt="logo" id="logotop"></a>
      <h1>Socialdemokratiet</h1>
      <p id="motto">"Venstre er uduelige, vi vil gøre det umulige"</p>

      <br>




    </header>

    <nav id="navbar">
      <ul>
        <li class="navitem"><a href="omos.html">Om os</a></li>
        <li>|</li>
        <li class="navitem"><a href="kontakt.html">Kontakt</a></li>
        <li>|</li>
        <li class="navitem"><a href="melddigind.html">Meld dig ind i dig</a></li>
        <li>|</li>
        <li class="navitem"><a href="stem.html">Stem på os</a></li>
        <li><input type="search" name="search1" placeholder="Søg:" id="search1"></li>
      </ul>
    </nav>
    <br>
    <br>
    <br>
    <br>
    <br>
    <main>
      <div class="billedhjulDiv">
        <button id="left" onclick="plusDivs(-1)">&#10094;</button>
        <img class="billedHjul" src="billede1.jpg" alt="billede1">
        <img class="billedHjul" src="billede2.jpg" alt="billede2">
        <img class="billedHjul" src="billede3.jpg" alt="billede3">
        <button id="right" onclick="plusDivs(+1)">&#10095;</button>
      </div>
    </main>
    <br>
    <br>
    <br>
    <br>
    <br>
    <footer>

      <input type="search" name="search2" placeholder="Søg:" id="search2"> <!-- Det kan være en god ide at undgå "ø" -->


      <form action="index.html" method="post" id="tilmeld">
        <p class="tilmeldTekst" id="tilmelddigher">TILMELD DIG HER</p>
        <input type="email" name="email" placeholder="Din email" class="tilmeldInput">
        <br>
        <input type="name" name="navn" placeholder="Dit navn" class="tilmeldInput">
        <br>
        <input type="submit" name="tilmeld" value="TILMELD" id="tilmeldknap">
        <p class="tilmeldTekst">Information omkring behandlingen af dine data finder du her.</p>
      </form>

      <div class="bottomnav">
        <ul>
          <li><a href="#">Om os</a></li>
          <li><a href="#">Kontakt os</a></li>
          <li><a href="#">Sociale medier</a></li>
        </ul>
      </div>

      <ul id="socialMedia">
        <li><a href="#">Facebook</a></li>
        <li><a href="#">Instagram</a></li>
        <li><a href="#">Youtube</a></li>
      </ul>

      <img src="../images/logo.png" alt="logo" id="logobot">

      <p id="copyrighttext">Administrer cookies © 2020, S APS. ALL RIGHTS RESERVED   |  MADE BY NICLAS, KEVIN OG ALBERTHE</p>
    </footer>

    <script type="text/javascript">
      var slideIndex = 1;
      showDivs(slideIndex);

      function plusDivs(n) {
        showDivs(slideIndex += n);
      }

      function showDivs(n) {
        var i;
        var x = document.getElementsByClassName("billedHjul");
        if (n > x.length) {slideIndex = 1} ;
        if (n < 1) {slideIndex = x.length} ;
        for (i = 0; i < x.length; i++) {
          x[i].style.display = "none";
        }
        x[slideIndex-1].style.display = "block";
      }
    </script>

  </body>
</html>
