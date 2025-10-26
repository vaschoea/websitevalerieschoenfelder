# websitevalerieschoenfelder
Hey, ich bin Valerie – kreativ, offen und immer neugierig auf Neues! In meiner Freizeit bin ich gerne draußen, gehe schwimmen oder entdecke neue Orte mit meiner Kamera. Hier auf meiner Seite bekommst du einen kleinen Einblick in das, was mich begeistert und antreibt.

<!DOCTYPE html>
<html lang="de">

<head>
  <meta charset="UTF-8">
  <title>Meine Website</title>
  <link rel="icon" type="image/jpg" href="images2/valerie1.jpg">
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/uikit@3.24.2/dist/css/uikit.min.css" />


  <style> 
@import url('https://fonts.googleapis.com/css2?family=Bitcount+Grid+Single:wght@100..900&family=Fascinate&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Fascinate+Inline&display=swap');

body{ 
font-size: 18px;
font-style: normal;
color: #660033; 
font-weight: 200;
font-family: serif, Arial, Helvetica, sans-serif;
background-size: cover; 
background-image: url(images2/beige1.jpeg);
margin: 0;
}

header{
text-align: center;
padding: 20px;
}

header img {
width: 200px;
height: auto;
border-radius: 50%;
margin-top: 10px;
transition: transform 0.3s ease, box-shadow 0.3s ease;
cursor: pointer;
}

header img:hover {
transform: scale(2.5);
z-index: 10;
position: relative;
box-shadow: 0 0 20px rgba(0,0,0,0.5);
}

main{
font-size: medium;
font-style: normal;
}

h1 {
font-family: 'Fascinate', cursive;  
font-size: 64px;                     
font-weight: 400;                    
color: #660033;                     
}

h2, h3{
color: #660033;
}

.fancy-title {
font-family: 'Fascinate Inline', cursive;
font-weight: 900; 
font-size: 2.5rem; 
color: #660033; 
text-align: center; 
margin-bottom: 20px; 
}

.center {
text-align: center;
}

.uk-navbar-nav > li > a {
color: #660033;     
font-weight: bold;
transition: 0.3s;
}

.uk-navbar-nav > li > a:hover {
color: #ff66a3;    
}

.navbar-center {
display: flex;
justify-content: center; 
margin: 20px 0;           
width: 100%;
}

table.uk-table {
margin: 0 auto;
text-align: center;
}

table.uk-table th,
table.uk-table td {
color:#7b7175;
border: 2px solid #660033;
text-align: center;
vertical-align: middle;
}

table.uk-table thead tr {
background-color: #fff3f6;
}

table.uk-table tbody tr:nth-child(odd) {
background-color: #ffffff; 
}

table.uk-table tbody tr:nth-child(even) {
background-color: #fff3f6; 
}

.cards-grid {
display: grid;
grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); /* flexible Spalten */
gap: 20px;
max-width: 1200px;
margin: 0 auto;
}

.card {
background: #fff;
border: 2px solid #660033;
border-radius: 16px;
box-shadow: 0 4px 8px rgba(0,0,0,0.1);
padding: 15px;
text-align: center;
display: flex;
flex-direction: column;
justify-content: flex-start;
transition: all 0.4s ease;
cursor: pointer;
transform: scale(0.95); /* etwas kleiner am Anfang */
}

.card:hover {
transform: scale(0.98);
}

.card .uk-card-media-top {
width: 100%;
border-radius: 12px;
overflow: hidden;
margin-bottom: 10px;
}

.uk-card-media-top img {
width: 100%;
height: 200px; /* fixe Höhe für alle Bilder */
object-fit: cover; /* gleiches Bildverhältnis */
border-radius: 8px;
}

.card.active {
transform: scale(1); /* beim Ausfahren größer */
box-shadow: 0 8px 20px rgba(0,0,0,0.2);
}

.card .extra-text {
max-height: 0;
overflow: hidden;
opacity: 0;
transition: max-height 0.6s ease, opacity 0.6s ease;
}


.card.active .extra-text {
max-height: 800px; /* groß genug für langen Text */
opacity: 1;
}

.full-width-card {
width: 100%;
border: 2px solid #8e2e54;
border-radius: 12px;
background-color: #fffaf0;
padding: 20px;
margin-top: 20px;
text-align: center;
}

.full-width-card .card-content p {
margin-bottom: 15px;
font-size: 1rem;
line-height: 1.5;
color: #660033;
}


.card-title{
font-family: Georgia, 'Times New Roman', Times, serif;
color: #660033;
font-weight: bold;
}

#erfahrungen {
aspect-ratio: auto; 
min-height: 400px;   
}

.extra-text {
overflow: visible; 
}


  </style>
  
    <script>
      document.addEventListener("click", function(event) {
        if (!event.target.closest(".card")) {
          cards.forEach(card => card.classList.remove("active"));
        }
      });
    });
    </script>
    

    <script>
    document.addEventListener("DOMContentLoaded", function() {
      const popup = document.getElementById("popup");
      popup.addEventListener("click", function() {
        popup.style.display = "none";
      });
    });
    </script>
    
    <script>
        document.addEventListener("DOMContentLoaded", function() {
          window.scrollTo(0, 0); // Seite immer oben starten
        
          const popup = document.getElementById("popup");
        
          // Event für Desktop (click) und Mobile (touchstart)
          function closePopup() {
            popup.style.display = "none";
          }
        
          popup.addEventListener("click", closePopup);
          popup.addEventListener("touchstart", closePopup);
        });
        </script>

<script>
    document.addEventListener("DOMContentLoaded", function() {
        const popup = document.getElementById("popup");
    
        function closePopup() {
            popup.style.display = "none";  // Popup schließen
            window.scrollTo({ top: 0, behavior: 'smooth' }); // Seite nach oben scrollen
        }
    
        popup.addEventListener("click", closePopup);
        popup.addEventListener("touchstart", closePopup); // für Mobilgeräte
    });
    </script>


<script>
    document.addEventListener("DOMContentLoaded", function() {
        // Klick auf Karte -> Text ausklappen
        const cards = document.querySelectorAll(".card");
    
        cards.forEach(card => {
            card.addEventListener("click", () => {
                // Wenn Karte schon aktiv ist, schließe sie
                if (card.classList.contains("active")) {
                    card.classList.remove("active");
                } else {
                    // Andere Karten schließen
                    cards.forEach(c => c.classList.remove("active"));
                    // Diese Karte öffnen
                    card.classList.add("active");
                }
            });
        });
    });
    </script>
    
    
  

<script src="https://cdn.jsdelivr.net/npm/uikit@3.24.2/dist/js/uikit.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/uikit@3.24.2/dist/js/uikit-icons.min.js"></script>


  <body> 
    <header> 
        <div id="popup" style="
        position: fixed;
        top: 0; left: 0; width: 100%; height: 100%;
        background: rgba(255,255,255,0.95);
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        font-family: Arial, sans-serif;
        color: #660033;
        z-index: 9999;
        cursor: pointer;
        ">
        <p style="font-size: 1.2rem; max-width: 400px;">
         Diese Webseite wurde von Valerie Leona Schönfelder erstellt.<br>
        Klicken Sie, um mehr über mich zu erfahren.
        </p>
        </div>

        <h1>Willkommen auf meiner Website! </h1>
        <p>Valerie Leona Schönfelder</p>
        <div uk-lightbox="animation: fade">
        <img src="images2/valerie1.jpg" alt="1">
        <img src="images2/valerie.jpg" alt="Das bin ich!">
        <img src="images2/valerie2.jpg" alt="2">
        </div>
    </header>
    <nav class="uk-navbar-container" style="background: transparent; margin: 20px 0;" uk-navbar>
        <div class="navbar-center">
            <ul class="uk-navbar-nav">
                <li><a href="#skifahren" class="nav-link">Skifahren</a></li>
                <li><a href="#studium" class="nav-link">Studium</a></li>
                <li><a href="#fotografieren" class="nav-link">Fotografieren</a></li>
                <li><a href="#schwimmen" class="nav-link">Schwimmen</a></li>
                <li><a href="#erfahrungen" class="nav-link">Berufserfahrungen</a></li>
            </ul>
        </div>
    </nav>
    
    
    <main> 
        <br><h2 class="center, fancy-title">Vorstellung</h2>
        <p class="center"> In der folgenden Tabelle erfahrt ihr die Basics über mich:</p>
        <table class="uk-table uk-table-divider uk-table-small">
              <tbody>
                <tr>
                  <td>Name</td>
                  <td>Valerie Leona Schönfelder</td>
                </tr>
                <tr>
                  <td>Alter</td>
                  <td>21 Jahre</td>
                </tr>
                <tr>
                  <td>Hobbys</td>
                  <td>Schwimmen, Lesen, Fotografieren, Skifahren</td>
                </tr>
                <tr>
                  <td>Studium</td>
                  <td>Media Management (aktuell im 3.Semester)</td>
                </tr>
              </tbody>
        </table>
        
        <div class="uk-card uk-card-default"> <br><br>
            <h3 class="uk-card-title, fancy-title" style="text-align: center;">Worüber möchtest du mehr erfahren?</h3>

            <section class="cards-grid">
                <div class="card" id="skifahren">
                    <h4 class="card-title">1</h4>
                    <p class="card-title">Erfahre mehr über mein Hobby <br>Skifahren</p>
                    <div class="uk-card-media-top">
                        <img src="images2/skifahrer3.jpg" alt="Skifahren">
                    </div>
                    <div class="extra-text">
                        <p>Ich fahre Ski, seit ich drei Jahre alt bin, und ich liebe es einfach! Für mich gibt es kaum etwas Besseres, als über die Pisten zu gleiten, den Schnee unter den Skiern zu spüren und die frische Bergluft einzuatmen. Skifahren macht mich einfach glücklich!</p>
                    </div>
                </div>
            
                <div class="card" id="studium">
                    <h4 class="card-title">2</h4>
                    <p class="card-title">Erfahre mehr über mein Media Management Studium</p>
                    <div class="uk-card-media-top">
                        <img src="images2/fotostudio2.jpg" alt="Media Management">
                    </div>
                    <div class="extra-text">
                        <p>Ich studiere seit Oktober 2024 Media Managment an der Hochschule Rhein-Main am Campus Unter den Eichen in Wiesbaden. In meinem aktuellen Semester erlerne ich in dem Schwerpunkt Interaktive Medien, alles Wichtige über das Programmieren und Websites erstellen, was ich persönlich interessant finde. Jedoch möchte ich unbedingt Erfahrungen in dem Bereich Videoproduktion sammeln, weshalb ich mich derzeit für Praktika in der Branche bewerbe.</p>
                    </div>
                </div>
            
                <div class="card" id="fotografieren">
                    <h4 class="card-title">3</h4>
                    <p class="card-title">Erfahre mehr über mein Hobby Fotografieren</p>
                    <div class="uk-card-media-top">
                        <img src="images2/fotografieren1.jpg" alt="Fotografieren">
                    </div>
                    <div class="extra-text">
                        <p>In meiner Freizeit fotografiere ich total gern. Einfach so, privat, wenn ich mal die Zeit finde. Dabei geht’s mir gar nicht um Perfektion, sondern darum, besondere Momente einzufangen, die mich berühren oder mir ein Lächeln ins Gesicht zaubern. Auf meinem Instagram-Account (@momentlichkeit) teile ich ab und zu ein paar dieser Aufnahmen. Kleine Augenblicke, die für mich das Leben schön machen.</p>
                    </div>
                </div>
            
                <div class="card" id="schwimmen">
                    <h4 class="card-title">4</h4>
                    <p class="card-title">Erfahre mehr über mein Hobby Schwimmen</p>
                    <div class="uk-card-media-top">
                        <img src="images2/schwimmen1.jpg" alt="Schwimmen">
                    </div>
                    <div class="extra-text">
                        <p>Früher war ich Leistungsschwimmerin und habe oft bis zu siebenmal pro Woche trainiert – das Schwimmbad war also fast wie mein zweites Zuhause. Der Sport hat mir nicht nur Disziplin und Durchhaltevermögen beigebracht, sondern auch unglaublich viel Freude bereitet. Ein besonderes Highlight war, als ich bei den Süddeutschen Meisterschaften über 200 Meter Kraul den 8. Platz belegt habe. Das war ein Moment, auf den ich bis heute stolz bin.</p>
                    </div>
                </div>
            
                <div class="card" id="erfahrungen">
                    <h4 class="card-title">4</h4>
                    <p class="card-title">Meine bereits gesammmelten <br> Berufserfahrungen</p>
                    <div class="uk-card-media-top">
                        <img src="images2/erfahrungen1.jpeg" alt="erfahrungen">
                    </div>
                    <div class="extra-text">
                        <p>Aufgrund meiner Fachhochschulreife mit der Fachrichtung Sozialassistenz habe ich ein Jahrespraktikum an der Grundschule der Obermayr absolviert und konnte dabei wertvolle Einblicke in die Arbeit mit Kindern gewinnen. Außerdem habe ich ein einmonatiges Praktikum im Altenheim auf der Station für demenziell erkrankte Menschen gemacht, wodurch ich viel über Pflege, Empathie und den Umgang mit älteren Menschen lernen konnte. 
                        <p>Seit 2021 arbeite ich zudem als Hostess beim Rheingau Musik Festival, was mir organisatorische Fähigkeiten und Erfahrung im Umgang mit Menschen in einem professionellen Umfeld vermittelt hat. </p>
                        <p>Mit Beginn meines Studiums habe ich als Werkstudentin bei der Wiesbadener Volksbank im Social-Media-Team gearbeitet. Dort konnte ich praktische Erfahrung in der Content-Erstellung, beim Videodreh und bei der Umsetzung von Social-Media-Kampagnen sammeln.</p>
                    </div>
                </div>

            </section>
            
            
        </div>
    </main>
    <footer>

    </footer>
  </body>
  <footer>
    <br><p class="center">Ich hoffe, euch hat gefallen, was ihr über mich erfahren habt:) Diese kleinen Einblicke zeigen, was mir wichtig ist und was mich begeistert und vielleicht konntet ihr mich dadurch ein bisschen besser kennenlernen. </p>
  </footer>
</html>
