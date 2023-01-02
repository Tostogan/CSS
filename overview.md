## CSS (Cascading Style Sheets)

> It's a RULE based language used to STYLE elements in the DOM (Document Object model)
* !!! in order to understand CSS one must understand the document HIERARCHY !!!

*** Daca HTML se ocupa de structura, CSS se ocupa de stilizare (culori, forme, marimi, pozitionare + putem si animatii crea, filtre)

*** HIERARCHY - este o structura creata dupa anumite reguli. DOC HTML este alcatuit din mai multe elemente, scrise intr-o anumita ierarhie, de ex. la crearea tabelului (td>tr>td). E important de inteles: elementul parinte, copil, mostenitor.

# the DOM (document)

document
   |
  html
   |
   |_ _ head
          |                          |-------------rule-------------|
         body                        |                              |
          |                          |    property1: val1;          |
         Element <----- styles ----- |    property2-detail: val2;   |
                                     |     ...                      |
                                     |------------------------------|
<element style="inline style block">

*** Ex. retetele noi le vedem cel mai des pe foaie. Ne imaginam ca avem o foaie printata si pe ea este notata o reteta, e ca un file HTML. In momentul in care bucatarul citeste acea reteta, creeaza noi obiecte. Asa si in html, mai intii se creeaza un doc. apoi rez. se vede in browser.

*** DECLARATION - e ca un detaliu, stilul caruia il modificam, ex: color: green;
    background: black;

# Element BOX and CONTENT are NOT THE SAME !!!

-----------BOX------------
|                        |------- BOX STTLING:
|         CONTENT x      |            * width (grosimea)
|                   \    |            * height (inaltimea)
|                     \  |            * padding (tab-ul din interior)
--------------------------            * border (rama)
                         \            * margin (tab-ul exterior)
                           \          * background (culoarea fonului)
                             \
                        TEXT CONTENT STYLING:
                           * font (shrift)
                           * text (parametrii-text, cel mai des indreptarea)
                           * color (culoarea textului)

## LET's do an example - an AD BOARd

document
   | 
  html
   |
   |
   |----- head 
   |       |
   |------body
           |
            ---- header      <------style: color -----> inheritance
                   |
                   -------- h1
                   |        |
                   |        ----- #text: "Welcome to the CSS"
                   |        | 
                            ---- small   <--- style: ....
                   |        |        |
                   |        |         ------ #text: (Cascading Style Sheets)
                   |        |
                   |        |---- #text: "training !!!" 
                   |
                   |
                   --- p
                       |
                       -----------#text: "This training will focus on BASICS of styling in details. You can apply for
                       it "
                       |
                       |
                       ----------- a   <--- style: ....
                       |           |
                       |           ---- #text: "here"
                       |  
                       |
                       ------- #text: ". Good luck!"    

## CSS (Cascading Style Sheets)     
> SELECTORS are formulas that indicate the "SEARCH PATH" in the DOM

## Let's work wit an IMAGE ELEMENT's BOX

------------- BOX ---------------
|<---------- width (600)------->|
| ^                             |
| |                             |
| |                             |
| height (400)                  |
| |                             |
| |                             |
| v                             |           
---------------------------------