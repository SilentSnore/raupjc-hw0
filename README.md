#1
Nakon dodavanja class library reference u Debug folderu se pojavljuje ClassLibrary.dll datoteka. Aplikacija se ruši uz FileNotFoundException zato jer pokušavamo pozvati metodu MyConsole klase za koju neznamo gdje joj se nalazi aseblij, tj. CLR od GAC-a ne dobiva tu informaciju. Poslao bih ConsoleApp.exe i ClassLibrary.dll datoteke.
#2
Aplikacija je koristila staru verziju ClassLibrary aseblija zato jer nismo buildali solution.
