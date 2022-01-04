LOC
Entwickle eine Funktion, die die Lines of Code (LOC) in einem wohlgeformten C# Quelltext zählt.

Der Quelltext wird als String angeliefert, zurückgegeben wird die Zahl der Zeilen, die ausführbaren Code enthalten. Zeilen, die nur aus Kommentar oder Whitespace bestehen, sollen also herausgefiltert werden [1].

Beachte:

C# kennt keine geschachtelten Kommentare
Kommentarzeichen – /*, */, // – öffnen/schließen Kommentare nicht innerhalb von Strings
Strings in Kommentaren werden als solche nicht erkannt, d.h. der Kommentar
/*a“*/“b… endet schon vor „b.
Ausführbarer Code kann in der selben Zeile wie ein Kommentar stehen: vor /* // oder nach */.