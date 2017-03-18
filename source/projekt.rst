Semestrálny projekt
===================

Zadanie
-------

Napíšte program, ktorý umožní jednému alebo viacerým hráčom zahrať sa nejakú doskovú hru. Váš program vykreslí hraciu plochu, umožní hráčom ťahať, bude pritom kontrolovať prípustnosť ťahov a zároveň bude kontrolovať, či niektorý z hráčov nevyhral, resp. neprehral.

Témy
----

Vyberte si jednu z týchto hier, alebo sa nimi inšpirujte:

* hracie dosky s figúrkami:

  * `dáma <http://en.wikipedia.org/wiki/Draughts>`_, `reversi <http://en.wikipedia.org/wiki/Reversi>`_, `šach <http://en.wikipedia.org/wiki/Chess>`_, `mlyn <http://sk.wikipedia.org/wiki/Mlyn_(hra)>`_, `človeče nehnevaj sa <http://sk.wikipedia.org/wiki/%C4%8Clove%C4%8De_nehnevaj_sa>`_, `ludo <http://en.wikipedia.org/wiki/Ludo_(board_game)>`_, `hex <http://en.wikipedia.org/wiki/Hex_(board_game)>`_, `bridge it <http://boardgamegeek.com/boardgame/11052/bridg-it>`_, `monopoly <http://en.wikipedia.org/wiki/Monopoly_(board_game)>`_, `go <http://en.wikipedia.org/wiki/Go_(game)>`_, `lines of action <http://sk.wikipedia.org/wiki/Lines_of_action>`_, `backgammon <http://en.wikipedia.org/wiki/Backgammon>`_, `dots and boxes <http://en.wikipedia.org/wiki/Dots_and_Boxes>`_

* kartičkové hry:

  * `pexeso <http://en.wikipedia.org/wiki/Concentration_(game)>`_, `kartové hry <http://en.wikipedia.org/wiki/Card_game>`_, `domino <http://en.wikipedia.org/wiki/Dominoes>`_, `scrabble <http://en.wikipedia.org/wiki/Scrabble>`_, `mahjong <http://en.wikipedia.org/wiki/Mahjong>`_, `black <http://en.wikipedia.org/wiki/Black_Path_Game>`_, `trax <http://en.wikipedia.org/wiki/Trax_(game)>`_, `blokus <http://en.wikipedia.org/wiki/Blokus>`_, `posúvací puzzle <http://en.wikipedia.org/wiki/Sliding_puzzle>`_

* hry pre jedného hráča:

  * `anglický solitaire <http://en.wikipedia.org/wiki/Peg_solitaire>`_, `pasians <http://en.wikipedia.org/wiki/Patience_(game)>`_, `tangram <http://en.wikipedia.org/wiki/Tangram>`_, `míny <http://en.wikipedia.org/wiki/Minesweeper_(video_game)>`_, `sokoban <http://en.wikipedia.org/wiki/Sokoban>`_, `sudoku <http://en.wikipedia.org/wiki/Sudoku>`_, `puzzle <http://en.wikipedia.org/wiki/Jigsaw_puzzle>`_, `light-bot <http://www.kongregate.com/games/Coolio_Niato/light-bot>`_, `kravička <http://www.herna.biz/hry-online/logicke/335-iq-marathon/>`_

* edukačné hry:

  *  ovládanie robota Karla, programovanie Baltazára, programovanie Logo (kreslenie korytnačkou)

Môžete sa inšpirovať online hrami na internete, napr.

* `logické hry <http://www.hrajhry.sk/hry/puzzle>`_
* `logicke hry <http://logickehry.sk/>`_
* `online hry <http://www.onlinehry.sk/>`_
* `detske hry <http://www.detskehry.sk/>`_
* `logické hry pre deti <http://rexik.zoznam.sk/hry/logicke/>`_
* `one more level <http://www.onemorelevel.com/>`_

Pri výbere hry myslite na to, že by sa mala ovládať najmä myšou (klikanie, ťahanie), mala by obsahovať aspoň jeden animovaný prvok, a samotná hracia plocha sa vnútorne reprezentuje ako nejaké dvojrozmerné pole.

Je vhodné si tému projektu nechať schváliť cvičiacimi, aby ste mali istotu, že to čo idete programovať je dobrá téma. Samozrejme, že tému si môžete hocikedy zmeniť.

Pravidlá vybranej hry si môžete prispôsobiť alebo aj dosť radikálne zmeniť.



Požiadavky
----------

Váš program musí spĺňať nasledovné požiadavky:

* program musí byť realizovaný ako inštancia vašej triedy ``Program``, napr.

  ::

   import tkinter

   class Program:
       def __init__(self):
           ...
           tkinter.mainloop()

       ...

   Program()

* okrem tejto triedy definujte aspoň jednu ďalšiu triedu pre popis nejakej časti hry, napr. figúrky, kartičky, políčka, hráč, nepriateľ, ... túto triedu využijete v hlavnom programe (tieto pomocné triedy môžete definovať buď v tom istom module alebo v ďalšom)
* okrem definícíí týchto tried a inštancie triedy ``Program``, nepoužívajte žiadne globálne premenné ani funkcie
* zvoľte si takú hru, aby sa pri realizácii hracej plochy využilo dvojrozmerné pole (napr. šachovnica, labyrint, ...)


Ďalej musí platiť:

* grafika je realizovaná modulom ``tkinter``:

  * na ovládanie hry použite udalosti myši (klikanie, ťahanie)
  * využite časovač (pomocou ``after()``)
  * môžete využiť aj klávesnicu
  * apoň nejaká časť grafiky musí byť realizovaná obrázkami (.png, .gif), pričom musíte simulovať aspoň jednu animáciu (striedanie niekoľkých obrázkov v časovači)
  * môžete využiť aj také funkcie a vlastnosti ``tkinter``, ktoré sme sa neučili

* program by mal čítať aj zapisovať aspoň jeden textový súbor, napr. rozohratú partiu, úvodné nastavenie, rôzne nastavenia hry, tabuľka najlepších výsledkov a pod.
* môžete ešte použiť aj moduly ``random``, ``math`` a ``json``

Dopredu si dohodnote s cvičiacimi, ak by mala vaša téma problém s niektorou z týchto požiadaviek.

Hodnotenie
----------

Projekt budú hodnotiť vaši cvičiaci, ale musíte ho odovzdať na úlohový server L.I.S.T., pričom

a) za splnenie **všetkých požiadaviek** bude základných 5 bodov (nedáva sa menej ako 5 bodov)
b) za umelecký dojem, pohodlné ovládanie, nové zaujímavé prvky, použitie nejakého náročnejšie algoritmu a pod. do 5 bodov - tieto body sa budú pridávať k základným 5 bodom

Takto získané body sa pripočítavajú k bodom ku skúške len vtedy, ak ich získate ešte **pred samotným termínom skúšky**.