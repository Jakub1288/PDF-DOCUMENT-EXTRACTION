## PDF Extrakce požadovaných hodnot z výročních zpáv penzijních společností

Cílem je automaticky extrahovat dané hodnoty z výročních zpráv penzijních společností a uložit je do dict. proměnné což umožňuje další manipulaci/nahrání/odeslání výsledných hodnot.

Pro extrakci je použita knihovna tabula-py. Extrakce hodnot z PDF souborů může být problematická v případě, kdy každý dokument má jinou strukturu, což je i tento případ. Proto je třeba pokrýt co největší množství rozložení a formátování stránek u všech PDF souborů. K tomu v tomto případě nejlépe posloužil package tabula-py a funkce read_pdf s parametrem Stream=True. 