

# 1. Wiederholen Sie aus der Grundschulzeit das schriftliche Rechnen mit den vier Grundrechenarten.

## Schriftliche Addition 
$$
\begin{array}{r}
  1024 \\
+  512 \\
\hline
  1536 \\
\end{array}
$$


## Schriftliche Subtraktion 
$$
\begin{array}{r}
  2048 \\
-  256 \\
\hline
  1792 \\
\end{array}
$$


## Schriftliche Multiplikation

$$
\begin{array}{r}
  128 \cdot 64 \\
\hline
  7680 \\
  + \quad 512 \\
\hline
8192
  
\end{array}
$$

## Schriftliche Division

$$
\begin{array}{r}
8192 \div 64 = 128 \quad \text{Rest} \; 0
\end{array}
$$

```plaintext
 8192 : 64 = 128  
 64
 ----  
 179  
 128
 ---- 
  512  
  512  
 ----
    0
```

---
# 2. Übersetzen Sie Zahlen von Dezimal- ins Dualsystem und umgekehrt.

>[!tip] Anleitung zur Umwandlung von Dezimal in Binär
> 
> - Beginne mit der Dezimalzahl, die du in das Binärsystem umwandeln möchtest. Nehmen wir zum Beispiel die Zahl `18`.
> - Teile die Zahl durch `2` und notiere den Rest (`0` oder `1`). Dieser Rest ist die Binärziffer 
> - Teile das Ergebnis der vorherigen Division erneut durch `2` und notiere wieder den Rest. Fahre so lange fort, bis das Ergebnis der Division `0` ist.
> - Die Binärzahl setzt sich aus den notierten Resten zusammen, wobei der erste Rest die niedrigste Ziffer (rechts) und der letzte Rest die höchste Ziffer (links) darstellt.
> - Beispiel für die Umwandlung von `18` in Binär:
> 
> | Division     | Ergebnis | Rest |
> |:-------------|:---------|:----:|
> | $18 \div 2$  | $9$      |  $0$ |
> | $9 \div 2$   | $4$      |  $1$ |
> | $4 \div 2$   | $2$      |  $0$ |
> | $2 \div 2$   | $1$      |  $0$ |
> | $1 \div 2$   | $0$      |  $1$ |
> 
> - Nun schreibe die Reste von unten nach oben, um die Binärzahl zu erhalten: `10010`.
> - Die Zahl `18` im Dezimalsystem entspricht also der Binärzahl `10010`.

## Dezimal in Binär 
### Zahl: 3
- **Binär:**
  $$
  \begin{aligned}
  3 \div 2 &= 1 \quad R \quad 1 \\
  1 \div 2 &= 0 \quad R \quad 1 \\
  \end{aligned}
  \quad\Bigg\uparrow
  $$
  $Binär: \ 11$

### Zahl: 4
- **Binär:**
  $$
  \begin{aligned}
  4 \div 2 &= 2 \quad R \quad 0 \\
  2 \div 2 &= 1 \quad R \quad 0 \\
  1 \div 2 &= 0 \quad R \quad 1 \\
  \end{aligned}
  \quad\Bigg\uparrow
  $$
  $Binär: \ 100$

### Zahl: 32
- **Binär:**
  $$
  \begin{aligned}
  32 \div 2 &= 16 \quad R \quad 0 \\
  16 \div 2 &= 8 \quad R \quad 0 \\
  8 \div 2 &= 4 \quad R \quad 0 \\
  4 \div 2 &= 2 \quad R \quad 0 \\
  2 \div 2 &= 1 \quad R \quad 0 \\
  1 \div 2 &= 0 \quad R \quad 1 \\
  \end{aligned}
  \quad\Bigg\uparrow
  $$
  $Binär: \ 100000$

### Zahl: 50
- **Binär:**
  $$
  \begin{aligned}
  50 \div 2 &= 25 \quad R \quad 0 \\
  25 \div 2 &= 12 \quad R \quad 1 \\
  12 \div 2 &= 6 \quad R \quad 0 \\
  6 \div 2 &= 3 \quad R \quad 0 \\
  3 \div 2 &= 1 \quad R \quad 1 \\
  1 \div 2 &= 0 \quad R \quad 1 \\
  \end{aligned}
  \quad\Bigg\uparrow
  $$
  $Binär: \ 110010$

### Zahl: 128
- **Binär:**
  $$
  \begin{aligned}
  128 \div 2 &= 64 \quad R \quad 0 \\
  64 \div 2 &= 32 \quad R \quad 0 \\
  32 \div 2 &= 16 \quad R \quad 0 \\
  16 \div 2 &= 8 \quad R \quad 0 \\
  8 \div 2 &= 4 \quad R \quad 0 \\
  4 \div 2 &= 2 \quad R \quad 0 \\
  2 \div 2 &= 1 \quad R \quad 0 \\
  1 \div 2 &= 0 \quad R \quad 1 \\
  \end{aligned}
  \quad\Bigg\uparrow
  $$
  $Binär: \ 10000000$

### Zahl: 1024
- **Binär:**
  $$
  \begin{aligned}
  1024 \div 2 &= 512 \quad R \quad 0 \\
  512 \div 2 &= 256 \quad R \quad 0 \\
  256 \div 2 &= 128 \quad R \quad 0 \\
  128 \div 2 &= 64 \quad R \quad 0 \\
  64 \div 2 &= 32 \quad R \quad 0 \\
  32 \div 2 &= 16 \quad R \quad 0 \\
  16 \div 2 &= 8 \quad R \quad 0 \\
  8 \div 2 &= 4 \quad R \quad 0 \\
  4 \div 2 &= 2 \quad R \quad 0 \\
  2 \div 2 &= 1 \quad R \quad 0 \\
  1 \div 2 &= 0 \quad R \quad 1 \\
  \end{aligned}
  \quad\Bigg\uparrow
  $$
  $Binär: \ 10000000000$


## Binär in Dezimal

>[!tip] Anleitung zur Umwandlung von Binär in Dezimal
> - Schreibe die Binärzahl auf nehmen wir beispielsweise `10010`
> - Schreibe über jede Ziffer in der Binärzahl die dazugehörige Potzenz
> 	- Schreibe von der rechten Ziffer aus beginnend $2^0$, $2^1$, $2^2$, ... 
> 	- Mache das bis du bei der linkesten Ziffer angekommen bist
> - Nun solltest du etwas in dieser Form haben:
>
>| $2^4$ | $2^3$ | $2^2$ | $2^1$ | $2^0$ |
>|:-----:|:-----:|:-----:|:-----:|:-----:|
>|   1   |   0   |   0   |   1   |   0   |
>
> - Nehme nun alle Spalten die eine `1` haben und addiere diese 2er-Potenzen zusammen
> - In unserem Beispiel:
> 	- $2^4+2^1\quad=\quad16+2\quad =\quad18$

### Zahl: $11_2$
- **Berechnung:**
  $$
  1 \cdot 2^1 + 1 \cdot 2^0 = 2 + 1 = 3
  $$
- **Dezimal:**
  $$
  3_{10}
  $$

---

### Zahl: $100_2$
- **Berechnung:**
  $$
  1 \cdot 2^2 + 0 \cdot 2^1 + 0 \cdot 2^0 = 4 + 0 + 0 = 4
  $$
- **Dezimal:**
  $$
  4_{10}
  $$

---

#### Zahl: $100000_2$
- **Berechnung:**
  $$
  1 \cdot 2^5 + 0 \cdot 2^4 + 0 \cdot 2^3 + 0 \cdot 2^2 + 0 \cdot 2^1 + 0 \cdot 2^0 = 32 + 0 + 0 + 0 + 0 + 0 = 32
  $$
- **Dezimal:**
  $$
  32_{10}
  $$

---

### Zahl: $110010_2$
- **Berechnung:**
  $$
  1 \cdot 2^5 + 1 \cdot 2^4 + 0 \cdot 2^3 + 0 \cdot 2^2 + 1 \cdot 2^1 + 0 \cdot 2^0 = 32 + 16 + 0 + 0 + 2 + 0 = 50
  $$
- **Dezimal:**
  $$
  50_{10}
  $$

---

### Zahl:  $10000000_2$
- **Berechnung:**
  $$
  1 \cdot 2^7 + 0 \cdot 2^6 + 0 \cdot 2^5 + 0 \cdot 2^4 + 0 \cdot 2^3 + 0 \cdot 2^2 + 0 \cdot 2^1 + 0 \cdot 2^0 = 128 + 0 + 0 + 0 + 0 + 0 + 0 + 0 = 128
  $$
- **Dezimal:**
  $$
  128_{10}
  $$

---

### Zahl: $10000000000_2$
- **Berechnung:**
  $$
  1 \cdot 2^{10} + 0 \cdot 2^9 + 0 \cdot 2^8 + 0 \cdot 2^7 + 0 \cdot 2^6 + 0 \cdot 2^5 + 0 \cdot 2^4 + 0 \cdot 2^3 + 0 \cdot 2^2 + 0 \cdot 2^1 + 0 \cdot 2^0 = 1024 + 0 + 0 + 0 + 0 + 0 + 0 + 0 + 0 + 0 + 0 = 1024
  $$
- **Dezimal:**
  $$
  1024_{10}
  $$


---

# 3. Verrechnen Sie zwei Zahlen parallel im Dezimal- und im Dualsystem und vergleichen sie die Ergebnisse.

>[!example] Beispiel: Addition im Dezimal- und Dualsystem
>
>### Dezimalsystem
>
>Wir nehmen die Zahlen `12` und `5` im Dezimalsystem und führen eine Addition durch:
>
>$$ 12 + 5 = 17 $$
>
>### Dualsystem
>
>Zunächst konvertieren wir die Dezimalzahlen `12` und `5` in das Dualsystem:
>
>- Die Zahl `12` wird im Dualsystem als `1100` dargestellt.
>- Die Zahl `5` wird im Dualsystem als `101` dargestellt (wir fügen für die Addition vorn Nullen hinzu, um sie auf dieselbe Länge zu bringen: `0101`).
>
>#### Wie funktioniert die Addition im Dualsystem?
>
>Die Addition im Dualsystem funktioniert ähnlich wie im Dezimalsystem, jedoch gibt es nur zwei Ziffern: `0` und `1`. Die Regeln sind einfach:
>- `0 + 0 = 0`
>- `1 + 0 = 1` oder `0 + 1 = 1`
>- `1 + 1 = 10` (dies entspricht `2` im Dezimalsystem, weshalb eine `1` in die nächste Stelle übertragen wird, wie ein Übertrag im Dezimalsystem)
>
>Diese Regeln sorgen dafür, dass bei der Addition von zwei `1`en ein Übertrag entsteht, der in die nächste Position geht.
>
>Führen wir die Addition im Dualsystem durch:
>
>$$
>\begin{aligned}
> & 1100_2 \\
> + & 0101_2 \\
>\hline
> & 10001_2 \\
>\end{aligned}
>$$
>
>Schritt für Schritt:
>1. **Rechte Spalte**: `0 + 1 = 1`
>2. **Nächste Spalte**: `0 + 0 = 0`
>3. **Nächste Spalte**: `1 + 1 = 10` (also `0` in dieser Spalte und `1` als Übertrag)
>4. **Nächste Spalte**: `1 + 0 + 1 (Übertrag) = 10` (also `0` in dieser Spalte und wieder `1` als Übertrag)
>5. **Letzte Spalte**: Der Übertrag wird in die nächste Spalte geschrieben, was zu einem zusätzlichen `1` führt.
>
>Das Endergebnis ist `10001_2`, was der Dezimalzahl `17` entspricht.
>
>### Vergleich der Ergebnisse
>
>- Das Ergebnis der Addition im Dezimalsystem ist `17`.
>- Das Ergebnis der Addition im Dualsystem `10001_2` entspricht ebenfalls der Dezimalzahl `17`.
>
>Fazit: Die Addition führt sowohl im Dezimal- als auch im Dualsystem zum selben Ergebnis. Die Regeln zur Addition im Dualsystem sind vergleichbar mit denen im Dezimalsystem, jedoch wird ein Übertrag immer dann erzeugt, wenn zwei `1`en addiert werden.


>[!example] Beispiel: Subtraktion im Dezimal- und Dualsystem
>
>### Dezimalsystem
>
>Wir beginnen mit den Dezimalzahlen `25` und `10` und führen eine Subtraktion durch:
>
>$$ 25 - 10 = 15 $$
>
>### Dualsystem
>
>Zunächst konvertieren wir die Dezimalzahlen `25` und `10` in das Dualsystem:
>
>- Die Zahl `25` wird im Dualsystem als `11001` dargestellt.
>- Die Zahl `10` wird im Dualsystem als `1010` dargestellt (wir fügen vorn eine Null hinzu, damit beide Zahlen dieselbe Länge haben: `01010`).
>
>#### Wie funktioniert die Subtraktion im Dualsystem?
>
>Die Subtraktion im Dualsystem ähnelt der Subtraktion im Dezimalsystem, folgt jedoch den Regeln der binären Mathematik:
>
>- `0 - 0 = 0`
>- `1 - 0 = 1`
>- `1 - 1 = 0`
>- Wenn wir `0 - 1` subtrahieren müssen, "leihen" wir uns eine `1` von der nächsthöheren Stelle, genau wie im Dezimalsystem.
>
>Führen wir die Subtraktion im Dualsystem Schritt für Schritt durch:
>
>$$
>\begin{aligned}
>& 11001_2 \\
>- & 01010_2 \\
>\hline
>& 01111_2 \\
>\end{aligned}
>$$
>
>Schrittweise:
>1. **Rechte Spalte**: `1 - 0 = 1`
>2. **Nächste Spalte**: `0 - 1 = 1` (wir "leihen" uns eine `1` von der nächsthöheren Stelle, was aus der linken `1` eine `0` macht)
>3. **Nächste Spalte**: `0 - 0 = 0`
>4. **Nächste Spalte**: `1 - 1 = 0`
>5. **Letzte Spalte**: `1 - 0 = 1`
>
>Das Ergebnis der Subtraktion ist `01111_2`, was der Dezimalzahl `15` entspricht.
>
>### Vergleich der Ergebnisse
>
>- Das Ergebnis der Subtraktion im Dezimalsystem ist `15`.
>- Das Ergebnis der Subtraktion im Dualsystem `01111_2` entspricht ebenfalls der Dezimalzahl `15`.
>
>Fazit: Die Subtraktion liefert sowohl im Dezimal- als auch im Dualsystem dasselbe Ergebnis. Die Regeln der Subtraktion bleiben in beiden Zahlensystemen ähnlich, obwohl die Handhabung der Ziffern aufgrund der binären Natur des Dualsystems leicht anders ist.


>[!example] Beispiel: Multiplikation im Dezimal- und Dualsystem
>
>### Dezimalsystem
>
>Nehmen wir die Zahlen `25` und `10` im Dezimalsystem und führen eine Multiplikation durch:
>
>$$ 25 \times 10 = 250 $$
>
>### Dualsystem
>
>Nun konvertieren wir die Dezimalzahlen `25` und `10` in das Dualsystem:
>
>- Die Zahl `25` im Dualsystem ist `11001`
>- Die Zahl `10` im Dualsystem ist `1010`
>
>- Zur Multiplikation beginnen wir bei der unteren Binärzahl an der rechtesten Stelle und schauen ob diese `1` oder `0` ist
>- Wenn diese `1` ist schreiben wir den 1. Faktoren so ab wie er ist falls die hinterste Zahl des 2.Faktoren `0` ist schreiben wir nur `0`-er hin, da `0 mal eine Zahl = 0`
>- Dies führen für wie zuvor genannt von der hintersten Zahl vom 2. Faktor bis zur vordersten Zahl durch, während wir bei den Ergebnissen die Stellen die wir schon abgearbeitet haben mit einem `x` auffüllen. (siehe unten)
>- Am Ende addieren wir dieses Zwischenergebniss welches wir durch verschieben bekommen haben
>
>Führen wir die Multiplikation im Dualsystem durch:
>
>$$
>\begin{aligned}
> 11001& \\
>\times \quad  01010& \\
>\hline
>\hline
>00000& \\
>11001\text{x}& \\
>00000\text{xx}& \\
>+\quad 11001\text{xxx}& \\
>\hline
>11111010
>\end{aligned}
>$$
>
>### Vergleich der Ergebnisse
>
>- Das Ergebnis der Multiplikation im Dezimalsystem ist `250`.
>- Das Ergebnis der Multiplikation im Dualsystem `1111101000_2` entspricht ebenfalls der Dezimalzahl `250`.
>
>Fazit: Auch hier stimmen die Ergebnisse im Dezimal- und Dualsystem überein.

## Division

### Erstes Beispiel

$$
10011100 \div 110 =011010 \quad R \quad00
$$

### Zweites Beispiel

$$
1100101 \div 111 =01110 \quad R \quad11
$$

---

# 4. Stellen Sie die Zahl -15 mit Hilfe des Zweierkomplements im Dualsystem dar.


>[!important] **Wichtiges Know-How zum Zweierkomplement**
>
>- **Definition**: Das Zweierkomplement ist eine Methode zur Darstellung negativer Zahlen im Binärsystem. Es ist besonders nützlich, weil damit Addition und Subtraktion von Vorzeichen behafteten Zahlen einfacher werden.
>
>- **Berechnung**:
>  1. **Binärzahl invertieren** (alle Bits umkehren, `1` wird zu `0` und `0` wird zu `1`).
>  2. **1 addieren** zum invertierten Wert.
>  
>- **Beispiel**: Um das Zweierkomplement von `0101` (5 im Dezimalsystem) zu berechnen:
>  1. **Invertieren**: `1010`
>  2. **1 addieren**: `1010 + 1 = 1011` (Zweierkomplement von `0101` ist `1011`, was `-5` darstellt).
>
>- **Vorteil**: Der Hauptvorteil des Zweierkomplements ist, dass es eine einheitliche Methode für die Darstellung negativer Zahlen bietet und keine speziellen Regeln für Subtraktion oder Addition erfordert. Rechner können so direkt mit Vorzeichen-behafteten Zahlen rechnen, ohne auf unterschiedliche Rechenverfahren zurückgreifen zu müssen.
>
>- **Grenzen der Bits**: Im Zweierkomplement hängt der darstellbare Wertebereich von der Anzahl der Bits ab:
>  - Für **n Bits** kann der Wertebereich dargestellt werden als:
>    - **Minimale Zahl**: $-2^{n-1}$
>    - **Maximale Zahl**: $2^{n-1} - 1$
>  - **Beispiel** für ein 8-Bit-System:
>    - Minimal darstellbare Zahl: $-128$
>    - Maximal darstellbare Zahl: $127$
>  - **Beispiel** für ein 16-Bit-System:
>    - Minimal darstellbare Zahl: $-32,768$
>    - Maximal darstellbare Zahl: $32,767$
  
### Anleitung:

- Da wir `-15` im Zweierkomplement darstellen wollen, müssen wir zunächst `15` in Binär darstellen, invertieren und dann 1 dazu addieren

$$
15 \text{ in Binär} = 1111
$$

>[!warning] Beachte, dass wir mindestens 5 Bit brauchen um es im Zweierkomplement darzustellen, da $-2^{n-1}$ die minimale Zahl für $n$ Bit angibt

$$
15 \text{ in Binär in 5 Bit} = 01111
$$

- Dies muss nun invertiert werden 



$$
15 \text{ in Binär und invertiert} = 10000
$$

- jetzt muss `1` draufaddiert werden 

$$
15 \text{ in Binär, invertiert und addiert} = 10001
$$
Das Ergebnis lautet also

$$
(-15)_{10} = 10001_2
$$

### Anleitung: Rückführung von Binärdarstellung zur Dezimaldarstellung (Zweierkomplement)

1. **Prüfen:**  
   - Höchstwertiges Bit (`1`) = negative Zahl im Zweierkomplement.

2. **Invertieren:**  
   - Invertiere alle Bits.

3. **Addieren:**  
   - Addiere `1` zur invertierten Zahl.

4. **Umwandeln:**  
   - Berechne den Dezimalwert der positiven Binärzahl.

5. **Vorzeichen:**  
   - Setze das negative Vorzeichen.

Beispiel:  
- `10001_2` → invertieren → `01110` → `+1` → `01111` → Dezimal: `15` → Ergebnis: `-15`.



>[!info] **Zweierkomplement vs. Einerkomplement: Einfach erklärt**
>
>- **Einerkomplement**:
>  - **Was es macht**: Wenn du eine negative Zahl darstellen willst, drehst du einfach alle 1en und 0en der positiven Zahl um. 
>    - Beispiel: Für `15` schreibst du `01111` und drehst es um zu `10000`, um `-15` darzustellen.
>  - **Problem**: Es gibt zwei verschiedene Möglichkeiten, `0` darzustellen: einmal als `00000` (positive Null) und einmal als `11111` (negative Null). Das kann zu Verwirrung führen und macht die Berechnung schwieriger.
>  - **Warum es nicht mehr benutzt wird**: Wegen der doppelten `0` ist es unpraktisch, und daher wird es kaum noch verwendet.
>
>- **Zweierkomplement**:
>  - **Was es macht**: Du drehst wieder alle 1en und 0en der positiven Zahl um, aber dann addierst du noch `1`, um die negative Zahl zu bekommen.
>    - Beispiel: Für `15` drehst du `01111` um zu `10000` und fügst `1` hinzu, was `10001` ergibt, um `-15` darzustellen.
>  - **Warum es besser ist**: Es gibt nur eine Art, `0` darzustellen, und es macht das Rechnen mit positiven und negativen Zahlen viel einfacher.
>  - **Warum es überall verwendet wird**: Es ist effizient und sorgt dafür, dass Computer leicht mit negativen Zahlen rechnen können, ohne dass es zu Problemen kommt.

