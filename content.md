layout: true
  
<div class="my-header"></div>

<div class="my-footer">
  <table>
    <tr>
      <td style="text-align:right">Sächsische Landesbibliothek – Staats- und Universitätsbibliothek</td>
      <td>27. Februar 2024</td>
      <td style="text-align:right"><a href="https://www.slub-dresden.de/">www.slub-dresden.de</a></td>
    </tr>
    <tr>
      <td style="text-align:right"></td>
      <td />
    </tr>
  </table>
</div>

<div class="my-title-footer">
  <table>
    <tr>
      <td style="text-align:left"><b>Robert Sachunsky, Markus Weigelt</b></td>
      <td style="text-align:left"><b></b></td>
      <td style="text-align:left"><b>Kay-Michael Würzner</b></td>
    </tr>
    <tr>
      <td style="text-align:left">Abteilung Informationstechnologie</td>
      <td style="text-align:left"></td>
      <td style="text-align:left">Abteilung Benutzung und Information</td>
    </tr>
    <tr>
      <td style="font-size:8pt"><b>27. Februar 2024</b></td>
    </tr>
    <tr>
      <td style="font-size:8pt">DHd 2024</td>
    </tr>
  </table>
</div>

---

class: title-slide
count: false

# Edierst Du noch oder trainierst Du schon?
## Datenmanagement für Trainingsdaten für die automatische Texterkennung

---

# Overview

- Prinzipien der automatischen Texterkennung
- Wege zur *Ground Truth*
- **Datenmangement für Trainingsdaten** (praktischer Teil)
- Trainingseffekte
- Diskussion, Ausblick und ein Wort zu Transkribus

---

class: part-slide
count: false

# Prinzipien der automatischen Texterkennung

---

# Prinzipien der automatischen Texterkennung

.cols[
.sixty[
- Bilderfassung ≠ Texterfassung
- **O**ptical **C**haracter **R**ecognition: Automatische Erfassung von Text in Bildern
- ursprünglich begrenzt auf Zeichenerkennung
- heute häufig Synonym für den gesamten Texterfassungsprozess
  + Bildvorverarbeitung
  + Layoutanalyse (OLR)
  + Zeilenerkennung
  + ...
]
.fourty[
<center><img src="https://upload.wikimedia.org/wikipedia/commons/9/9f/Codex_Manesse_127r.jpg" /></center>
]
]

---

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_raw.svg" />
</p>
]
]

---

count: false

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
- Bildvorverarbeitung
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_raw.svg" />
</p>
]
]

---

count: false

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
- Bildvorverarbeitung
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_opt.svg" />
</p>
]
]

---

count: false

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_opt.svg" />
</p>
]
]

---

count: false

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_struct.svg" />
</p>
]
]

---

count: false

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
    * **strukturierende** Elemente
        + Absätze
        + Überschriften
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_struct.svg" />
</p>
]
]

---

count: false

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
    * **strukturierende** Elemente
        + Absätze
        + Überschriften
    * **textflussunterbrechende** Elemente
        + Seitenzahlen
        + Kolumnentitel
        + Abbildungsunterschriften
        + Marginalien etc.
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_struct.svg" />
</p>
]
]

---

count: false

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
    * **strukturierende** Elemente
        + Absätze
        + Überschriften
    * **textflussunterbrechende** Elemente
        + Seitenzahlen
        + Kolumnentitel
        + Abbildungsunterschriften
        + Marginalien etc.
    * **nichttextuelle** Elemente
        + Abbildungen
        + Tabellen etc.
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_struct.svg" />
</p>
]
]

---

count: false

# Prinzipien der automatischen Texterkennung

.cols[
.fifty[
- Bildvorverarbeitung
- Layoutanalyse
    * **strukturierende** Elemente
        + Absätze
        + Überschriften
    * **textflussunterbrechende** Elemente
        + Seitenzahlen
        + Kolumnentitel
        + Abbildungsunterschriften
        + Marginalien etc.
    * **nichttextuelle** Elemente
        + Abbildungen
        + Tabellen etc.
- Texterkennung
]
.fourty[
<p style="margin-top:-80px">
<img src="img/grenzboten_text.svg" />
</p>
]
]
---

class: part-slide

# Vielen Dank für Ihre Aufmerksamkeit!

<center>
<a href="https://wrznr.github.io/gt-management-dhd-2024/">wrznr.github.io/gt-management-dhd-2024</a>
</center>
