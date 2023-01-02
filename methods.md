## Connect CSS to HTML methods:
1. [+] inline

<tag style="CSS block></tag>

2. [+] global
       <head>
          ...
          <style>
             selector {
                property1: value1;
                property2: value2;
                ...
             }

    Exista 5 categorii de selectori>
    a. tag
    b. class
    c. id
    d. pseudo
    e. advanced

          </style>
          ...
       </head>

       <body>
          ...
          <tag></tag>
          ...
       </body>

    ***Facem diferenta dintre inline si global prin urmatorul exemplu>
    elementele - sunt oamenii, dar stilurile - hainele
    1) inline style: e omul care poarta anumite haine, cu un anumit stil, dupa care si il putem identifica
    2) global style: oamenii merg la teatru, cinematograf si hainele care sunt mai grele le lasa la garderoba, iar oamneii merg in sala pentru a privi piesa sau filmul si desi proprietarii hainelor se afla in sala, dar hainele in spatiul propriu-zis, oricum, intre ele exista o conexiune, stabilita prin geton (cu un anumit numar identificator) sau alt instrument 
    (selectors-e ca o conexiune care leaga stirule de diferite elemente)

    ***Global style - nu se creeaza atributul "style", ca in Inline style, dar elementul "style"

3. [ ] external