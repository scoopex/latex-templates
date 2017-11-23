
Hintergrund
===========

Ein Framework um Folien mit weniger Schmerz als Libreoffice Impress bzw. Microsoft Powerpoint zu erzeugen.
Verbessserungs-, Erweiterungsbeiträge nehme ich gerne an, Pull Requests sind sehr willkommen.

Entwickeln
===========

 * Latex installieren
   ```
   apt-get install texlive-fonts-extra texlive-fonts-recommended texlive-base texlive-binaries texlive-extra-utils \
    texlive-font-utils texlive-fonts-recommended texlive-fonts-recommended-doc texlive-generic-recommended \
    texlive-lang-german texlive-latex-base texlive-latex-base-doc texlive-latex-recommended texlive-latex-recommended-doc \
    texlive-pictures texlive-pictures-doc texlive-pstricks texlive-pstricks-doc texlive-latex-extra
   ```
 * Editieren und kompilieren
   ```
   # Editieren und Ausführen
   vim -p src/parts/*
   ./process dev

   # Geöffnet lassen, aktualisiert sich automatisch
   evince tmp/vortrag.pdf &

   # Editieren und Ausführen
   ./process dev
   ```
 * Finale Version erstellen
   ```
   ./process final
   ./process clean
   git commit -m "<Kommentar>" -a
   ```

