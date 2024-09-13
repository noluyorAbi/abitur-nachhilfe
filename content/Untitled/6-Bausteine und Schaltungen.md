


# Das wusste schon de Morgan

>[!note] Aufgabenstellung
>
>Die boolesche Operation $\text{And } (\land)$ kann unter Verwendung der booleschen Operation $\text{Not } (\neg)$ aus der booleschen Operation $\text{Or } (\lor)$ erzeugt werden. Und auch umgekehrt, $\text{Or } (\lor)$ kann aus $\text{And } (\land)$ unter Verwendung von $\text{Not } (!)$ erzeugt werden.
>
>Bauen Sie $\text{And}$ und $\text{Or}$. Entwickeln Sie zunächst die benötigen Formeln und entwerfen Sie dann die dazu entsprechenden Schaltungen.

## Grundlagen

|  A  |  B  | A $\land$ B | A $\lor$ B |
|:---:|:---:|:-----------:|:----------:|
|  0  |  0  |      0      |     0      |
|  0  |  1  |      0      |     1      |
|  1  |  0  |      0      |     1      |
|  1  |  1  |      1      |     1      |

### De Morganschen Gesetze

#### **NOT (A AND B) ist dasselbe wie (NOT A) OR (NOT B)**
$$
\begin{aligned}
\neg(A \land B) &= \neg A \lor \neg B
\end{aligned}
$$

|  A  |  B  | $\neg(A \land B)$ | $(\neg A) \lor (\neg B)$ |
|:---:|:---:|:-----------------:|:-----------------------:|
|  0  |  0  |        1          |           1             |
|  0  |  1  |        1          |           1             |
|  1  |  0  |        1          |           1             |
|  1  |  1  |        0          |           0             |

#### **NOT (A OR B) ist dasselbe wie (NOT A) AND (NOT B)**:

$$
\begin{aligned}
\neg(A \lor B) &= \neg A \land \neg B
\end{aligned}
$$

|  A  |  B  | $\neg(A \lor B)$ | $(\neg A) \land (\neg B)$ |
|:---:|:---:|:----------------:|:------------------------:|
|  0  |  0  |        1         |            1             |
|  0  |  1  |        0         |            0             |
|  1  |  0  |        0         |            0             |
|  1  |  1  |        0         |            0             |

#### Schaltplan zu De Morgan

![[Pasted image 20240826174802.png]]

### Aus den De Morganschen Gesetzen können wir nun AND und OR herleiten

#### AND

- Aus dem ersten De Morganschen Gesetz gilt

$$
\begin{aligned}
\neg(A \land B) &= \neg A \lor \neg B
\end{aligned}
$$
- Dies negieren wir nun nochmal um durch die Doppelte Negierung, die Negierung aufzuheben

$$
\begin{aligned}
\neg\neg(A \land B) &=\neg(\neg A \lor \neg B)\\
&=A \land B
\end{aligned}
$$

#### OR

- Aus dem zweiten De Morganschen Gesetz gilt

$$
\begin{aligned}
\neg(A \lor B) &= \neg A \land \neg B
\end{aligned}
$$

- Dies negieren wir nun nochmal um durch die Doppelte Negierung, die Negierung aufzuheben

$$
\begin{aligned}
\neg\neg(A \lor B) &=\neg(\neg A \land \neg B)\\
&=A \lor B
\end{aligned}
$$

# Zaun oder Gatter – das ist hier die Frage

Untersuchen Sie anhand von Wahrheitstafeln, ob

```
!a !b c + !a b !c + a !b !c + a b c
```

und

```
Xor( Xor(a,b), c)
```

identisch sind.


### Lösung

Um die beiden Ausdrücke $!a !b c + !a b !c + a !b !c + a b c$ und $Xor(Xor(a, b), c)$ anhand von Wahrheitstafeln zu vergleichen, erstellen wir zunächst die Wahrheitstafeln für beide Ausdrücke und prüfen dann, ob die Ergebnisse in allen Fällen übereinstimmen.

### Wahrheitstafel für $!a !b c + !a b !c + a !b !c + a b c$

| a | b | c | !a | !b | !a!bc | !ab!c | a!b!c | abc | !a!bc + !ab!c + a!b!c + abc |
|---|---|---|----|----|-------|-------|-------|-----|------------------------------|
| 0 | 0 | 0 |  1 |  1 |   0   |   0   |   0   |  0  |             0                |
| 0 | 0 | 1 |  1 |  1 |   1   |   0   |   0   |  0  |             1                |
| 0 | 1 | 0 |  1 |  0 |   0   |   1   |   0   |  0  |             1                |
| 0 | 1 | 1 |  1 |  0 |   0   |   0   |   0   |  0  |             0                |
| 1 | 0 | 0 |  0 |  1 |   0   |   0   |   1   |  0  |             1                |
| 1 | 0 | 1 |  0 |  1 |   0   |   0   |   0   |  1  |             1                |
| 1 | 1 | 0 |  0 |  0 |   0   |   0   |   0   |  0  |             0                |
| 1 | 1 | 1 |  0 |  0 |   0   |   0   |   0   |  1  |             1                |

### Wahrheitstafel für $Xor(Xor(a, b), c)$

1. Berechnen wir zunächst $Xor(a, b)$:
   $$
   a \oplus b = ab' + a'b
   $$

| a | b | a ⊕ b |
|---|---|-------|
| 0 | 0 |   0   |
| 0 | 1 |   1   |
| 1 | 0 |   1   |
| 1 | 1 |   0   |

2. Berechnen wir dann $Xor(Xor(a, b), c)$:
   $$
   (a \oplus b) \oplus c = (a \oplus b)c' + (a \oplus b)'c
   $$

| a | b | c | a ⊕ b | (a ⊕ b) ⊕ c |
|---|---|---|-------|--------------|
| 0 | 0 | 0 |   0   |      0       |
| 0 | 0 | 1 |   0   |      1       |
| 0 | 1 | 0 |   1   |      1       |
| 0 | 1 | 1 |   1   |      0       |
| 1 | 0 | 0 |   1   |      1       |
| 1 | 0 | 1 |   1   |      0       |
| 1 | 1 | 0 |   0   |      0       |
| 1 | 1 | 1 |   0   |      1       |

### Vergleich der Wahrheitstafeln

| a | b | c | !a!bc + !ab!c + a!b!c + abc | (a ⊕ b) ⊕ c |
|---|---|---|-----------------------------|-------------|
| 0 | 0 | 0 |             0               |      0      |
| 0 | 0 | 1 |             1               |      1      |
| 0 | 1 | 0 |             1               |      1      |
| 0 | 1 | 1 |             0               |      0      |
| 1 | 0 | 0 |             1               |      1      |
| 1 | 0 | 1 |             1               |      0      |
| 1 | 1 | 0 |             0               |      0      |
| 1 | 1 | 1 |             1               |      1      |

Wir sehen, dass die Ergebnisse in allen Fällen übereinstimmen. Daher sind die beiden Ausdrücke $!a !b c + !a b !c + a !b !c + a b c$ und $Xor(Xor(a, b), c)$ identisch.