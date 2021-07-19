# Teszt

Név: Csányi Attila

## Kérdések:

1. Mit értünk egy `commit` alatt, mit tartalmaz?
A commit a repó egy adott pillanatban aktuális állapotát tartalmazza. A commit logikailag összetartozó változásokat tartalmaz, egyszerre több fájl módosítása is lehet benne, commit message is tartozik hozzá.

1. Mi a különbség a `fetch` es `pull` git parancsok között?
A fetch letölti a távoli repo állapotát és szinkronizálja a lokális repoval, de nem módisítja a working directory-t. A pull a fetch és a merge parancsot végzi el egymás után, jelzi, ha conflict van, és a conflict feloldása után módosítja a lokális repo-t.

1. Mi a három állapota file-oknak git szempontjából, milyen parancsokkal mozgatjuk ezek között?
modified: a korábban már tracked fájl szerkesztésével kerül modified állapotba
staged: a módosított fájl a git add paranccsal kerül staged állapotba
commited: a stage areából a git commit paranccsal kerül át a lokális repo-ba

1. Hogyan jutunk egy másolathoz egy repóról?
A git clone paranccsal.

1. Mi történik, ha valaki más is módosította a file-t amin dolgozunk és mit tudunk tenni ilyenkor?
A git pull paranccsal le tudjuk tölteni az aktuális állapotot. Ha azonos soron történt a módosítás, akkor merge conflict keletkezik, amit fel kell oldani. Utána lehet add-olni, commit-olni és push-olni.

1. Mi az a `HEAD` és mi a jelentősége?
A HEAD az aktuális branch utolsó commit-jére mutat.

1. Mi a célja a branch-elésnek?
A branch ('elágazás') lehetővé teszi, hogy azonos repóban, és akár azonos fájlokot többen dolgozzanak párhuzamosan. A különböző branch-eket a git merge paranccsal lehet egyesíteni, az esetleges conflictokat ekkor lehet feloldani.

1. Hogyan lehet összehasonlítani file-ok változásait, mire tudjuk még ezt a kimenetet használni?
A git diff paranccsal lehet file-ok változásait összehasonlítani.

1. Hogy lehet megnézni egy repo történetét, milyen eszközeink vannak ebben való keresésre?
A git log paranccsal lehet megnézni a repo történetét. A kimenetet kapcsolókkal lehet módosítani pl. git log --oneline --graph --all. A grep-pel tudunk szűrni a kimenetbent.
1. Melyik git parancsot használnád, hogy megtudd milyen állapotban van épp a repo?
git status
