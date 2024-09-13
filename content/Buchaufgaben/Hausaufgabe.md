
# Aufgabe - Q2 IF-LK - ComparableContent implementieren

>[!note] Aufgabenstellung
>Vollendet eure Implementation des ComparableContent-Interfaces, das wir für die binären Suchbäume benötigen. Das Interface findet ihr bei den Abiturklassen.
>
>Als Beispiel hatten wir abgesprochen die Klasse `Pferd` mit folgenden Attributen:
>
>- **farbe** (String)
>- **geschwindigkeit** (double)
>- **rasse** (String)
>- **geschlecht** (char)
>
>Denkt bei den Strings an die Standard-Java-Methode `compareTo` (siehe Google). `char`-s könnt ihr wie Zahlen vergleichen.

## Lösung

Hier ist eine vollständige Implementierung des `ComparableContent`-Interfaces und der Klasse `Pferd`. Die Klasse `Pferd` implementiert das Interface und definiert, wie die Vergleichslogik für Objekte dieser Klasse aussehen soll.

### 1. ComparableContent Interface

```java
public interface ComparableContent<T> {
    int compareTo(T other);
}
```

**Erklärung:**  
Das `ComparableContent`-Interface ist eine generische Schnittstelle, die eine Methode `compareTo` verlangt. Diese Methode wird implementiert, um zwei Objekte einer Klasse miteinander zu vergleichen. Der Rückgabewert dieser Methode ist ein `int` und folgt der Standard-Konvention:  
- Gibt `-1` zurück, wenn das aktuelle Objekt kleiner ist.  
- Gibt `1` zurück, wenn das aktuelle Objekt größer ist.  
- Gibt `0` zurück, wenn beide Objekte gleich sind.

Dies ist besonders wichtig, um Objekte korrekt in binären Suchbäumen sortieren zu können, da der Baum seine Struktur basierend auf dem Ergebnis der Vergleiche bildet.

---

### 2. Pferd Klasse

```java
public class Pferd implements ComparableContent<Pferd> {
    private String farbe;
    private double geschwindigkeit;
    private String rasse;
    private char geschlecht;

    // Constructor
    public Pferd(String farbe, double geschwindigkeit, String rasse, char geschlecht) {
        this.farbe = farbe;
        this.geschwindigkeit = geschwindigkeit;
        this.rasse = rasse;
        this.geschlecht = geschlecht;
    }

    // Getters
    public String getFarbe() {
        return farbe;
    }

    public double getGeschwindigkeit() {
        return geschwindigkeit;
    }

    public String getRasse() {
        return rasse;
    }

    public char getGeschlecht() {
        return geschlecht;
    }

    // compareTo method to compare two Pferd objects
    @Override
    public int compareTo(Pferd other) {
        // Compare based on geschwindigkeit (speed) first
        if (this.geschwindigkeit < other.geschwindigkeit) {
            return -1;
        } else if (this.geschwindigkeit > other.geschwindigkeit) {
            return 1;
        }

        // If geschwindigkeit is equal, compare based on farbe
        int farbeComparison = this.farbe.compareTo(other.farbe);
        if (farbeComparison != 0) {
            return farbeComparison;
        }

        // If farbe is also equal, compare based on rasse
        int rasseComparison = this.rasse.compareTo(other.rasse);
        if (rasseComparison != 0) {
            return rasseComparison;
        }

        // If rasse is also equal, compare based on geschlecht
        return Character.compare(this.geschlecht, other.geschlecht);
    }

    @Override
    public String toString() {
        return "Pferd [Farbe=" + farbe + ", Geschwindigkeit=" + geschwindigkeit + ", Rasse=" + rasse + ", Geschlecht=" + geschlecht + "]";
    }
}
```

**Erklärung:**  
Die Klasse `Pferd` enthält vier Attribute, die im Vergleich eine Rolle spielen:

1. **geschwindigkeit** (double): Die Geschwindigkeit eines Pferdes. Pferde mit höherer Geschwindigkeit werden als "größer" betrachtet.
2. **farbe** (String): Wenn die Geschwindigkeit gleich ist, wird die Farbe der Pferde alphabetisch verglichen (basierend auf der `compareTo`-Methode für Strings).
3. **rasse** (String): Wenn auch die Farben gleich sind, erfolgt ein weiterer Vergleich nach der Rasse des Pferdes.
4. **geschlecht** (char): Zuletzt wird das Geschlecht verglichen. Da `char` als numerischer Datentyp behandelt werden kann, erfolgt dieser Vergleich wie bei Zahlen.

Die `compareTo`-Methode folgt dieser Hierarchie, um die `Pferd`-Objekte zu sortieren oder zu vergleichen. Dies ist wichtig für binäre Suchbäume, wo die Struktur auf Vergleichen basiert.  
Die `toString`-Methode sorgt dafür, dass Objekte von `Pferd` in einer lesbaren Form ausgegeben werden, was beim Debugging hilfreich ist.

---

### 3. Beispiel zur Nutzung

```java
public class Main {
    public static void main(String[] args) {
        Pferd pferd1 = new Pferd("Braun", 45.6, "Arabian", 'M');
        Pferd pferd2 = new Pferd("Weiß", 47.3, "Thoroughbred", 'F');

        // Compare two Pferd objects
        int result = pferd1.compareTo(pferd2);

        if (result < 0) {
            System.out.println(pferd1 + " ist langsamer als " + pferd2);
        } else if (result > 0) {
            System.out.println(pferd1 + " ist schneller als " + pferd2);
        } else {
            System.out.println(pferd1 + " ist gleich zu " + pferd2);
        }
    }
}
```

**Erklärung:**  
In diesem Beispiel wird der Vergleich zwischen zwei `Pferd`-Objekten getestet. Die `compareTo`-Methode wird aufgerufen, um zu bestimmen, ob das erste Pferd langsamer, schneller oder gleich schnell ist wie das zweite. Basierend auf den Vergleichsoperationen (`geschwindigkeit`, `farbe`, `rasse` und `geschlecht`) wird ein Ergebnis zurückgegeben und entsprechend in der Konsole ausgegeben:

- Wenn das erste Pferd schneller ist, gibt es eine positive Zahl (`1`) zurück.
- Wenn es langsamer ist, gibt es eine negative Zahl (`-1`) zurück.
- Wenn sie gleich sind, wird `0` zurückgegeben.

Das Beispiel verdeutlicht, wie die Implementierung des `ComparableContent`-Interfaces es ermöglicht, `Pferd`-Objekte in einem binären Suchbaum korrekt zu vergleichen und zu sortieren.
