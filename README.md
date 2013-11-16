# LaTeX-mall för sångblad
### ...som de brukar se ut på Fysiksektionen, THS, KTH

0. Du kommer behöva några verktyg som kommer med de flesta standardiserade TeX-distributioner: `dvips`, `psbook`, `psnup`

0. Skriv ditt sångblad enligt mallen, ExempelBlad.tex

0. skapa .dvi-fil

        $ latex filnamn.tex

    *OBS!* Vill man inte sitta och göra alla steg 4-6 kan man köra Python-scriptet sangblad.py Då får man ut en färdig pdf!

        $ python sangblad.py MittSangblad.dvi

0. skapa .ps-fil

        $ dvips -o filnamn.ps filnamn.dvi

0. sortera om sidorna

        $ psbook filnamn.ps > bokfil.ps

0. montera på papper

        $ psnup -W11.5cm -H29.7cm -2 -pa4 bokfil.ps > filforutskrift.ps

0. Skriv ut på dubbelsidigt A4 papper och vi ihop



