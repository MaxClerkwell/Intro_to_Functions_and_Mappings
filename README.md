# Einführung in Abbildungen

## 1. Einleitung
Abbildungen sind ein fundamentales Konzept in Mathematik und Informatik. Sie beschreiben die eindeutige Zuordnung von Elementen einer Menge zu Elementen einer anderen Menge. In der Informatik spielen sie eine zentrale Rolle bei der Datenverarbeitung, Verschlüsselung und Speicheradressierung.

## 2. Definition einer Abbildung
Eine Abbildung ist eine Vorschrift, die jedem Element einer Menge \( A \) genau ein Element einer Menge \( B \) zuordnet. Formal schreiben wir:

![Definition](https://latex.codecogs.com/png.latex?f%3A%20A%20%5Cto%20B%2C%20%5Cquad%20f%28a%29%20%3D%20b)

Dabei nennt man:
- \( A \) die **Definitionsmenge** \( D(f) \)
- \( B \) die **Wertemenge** \( W(f) \)
- \( f(A) \) die **Bildmenge**

## 3. Eigenschaften von Abbildungen
### 3.1 Injektivität
Eine Abbildung \( f: X \to Y \) ist **injektiv**, wenn unterschiedliche Eingaben unterschiedliche Ausgaben liefern:

![Injektivität](https://latex.codecogs.com/png.latex?f%28x_1%29%20%3D%20f%28x_2%29%20%5CRightarrow%20x_1%20%3D%20x_2)

**Anwendung in der Informatik:** Speicheradressierung, bei der jede Adresse genau einem Speicherinhalt entspricht.

### 3.2 Surjektivität
Eine Abbildung \( f: X \to Y \) ist **surjektiv**, wenn jeder Wert in \( Y \) von mindestens einem Wert in \( X \) getroffen wird:

![Surjektivität](https://latex.codecogs.com/png.latex?%5Cforall%20y%20%5Cin%20Y%2C%20%5Cexists%20x%20%5Cin%20X%3A%20f%28x%29%20%3D%20y)

**Anwendung in der Informatik:** Rundungsfunktionen, die mehreren Eingabewerten denselben Ausgabewert zuordnen.

### 3.3 Bijektivität
Eine Abbildung ist **bijektiv**, wenn sie sowohl injektiv als auch surjektiv ist. Das bedeutet, dass jedes Element aus \( Y \) genau einem Element aus \( X \) zugeordnet wird.

**Anwendung in der Informatik:** Kodierungen, bei denen eine 1:1-Entsprechung zwischen Original- und Kodierungswert besteht.

## 4. Umkehrbarkeit von Abbildungen
Eine Abbildung \( f: X \to Y \) ist **umkehrbar**, wenn es eine Funktion \( g: Y \to X \) gibt, sodass:

![Umkehrbarkeit](https://latex.codecogs.com/png.latex?g%28f%28x%29%29%20%3D%20x%20%5Cquad%20%5Ctext%7Bund%7D%20%5Cquad%20f%28g%28y%29%29%20%3D%20y)

**Beispiel für eine umkehrbare Funktion:**

![Beispiel](https://latex.codecogs.com/png.latex?f%28x%29%20%3D%20x%20-%203%2C%20%5Cquad%20f%5E%7B-1%7D%28y%29%20%3D%20y%20%2B%203)

**Wann ist eine Funktion nicht umkehrbar?**
- Wenn sie nicht injektiv ist.
- Beispiel: \( f(x) = x^2 \), da \( f(-2) = f(2) = 4 \) keine eindeutige Umkehrfunktion existiert.

**Anwendung in der Informatik:**
- Einwegfunktionen als Grundlage asymmetrischer Verschlüsselung.

## 5. Darstellung von Abbildungen
Abbildungen können auf verschiedene Weise dargestellt werden:

- **Funktionsgleichungen:** ![Funktionsgleichung](https://latex.codecogs.com/png.latex?f%28x%29%20%3D%20x%5E2)
- **Tabellen:** Wertepaare \( (x, f(x)) \)
- **Graphen:** Visualisierung einer Funktion
- **Code:** Implementierung als Programm

**Beispielhafte Implementierung einer Abbildung in Python:**

```python
def square(x):
    return x * x
```

## 6. Anwendungen in der Informatik
- **Hashfunktionen:** Abbildungen mit festgelegtem Wertebereich für sichere Datenspeicherung.
- **Verschlüsselung:** Einwegfunktionen als Basis asymmetrischer Kryptographie.
- **Maschinelles Lernen:** Abbildungen zwischen Eingangs- und Ausgangsdaten in neuronalen Netzen.

## 7. Take Home
- Abbildungen sind grundlegend für Mathematik und Informatik.
- Sie beschreiben die Zuordnung von Werten zwischen Mengen.
- Eigenschaften wie Injektivität, Surjektivität und Bijektivität beeinflussen ihre Umkehrbarkeit.
- In der Informatik sind Abbildungen für Adressierung, Kodierung und Verschlüsselung zentral.

## 8. Weiterführende Literatur
- Wikipedia: [Abbildung (Mathematik)](https://de.wikipedia.org/wiki/Abbildung_(Mathematik))
- Wolfram MathWorld: [Function](https://mathworld.wolfram.com/Function.html)
- Khan Academy: [Functions](https://www.khanacademy.org/math/algebra/x2f8bb11595b61c86:functions)
- StackExchange: [Anwendungen in der Informatik](https://cs.stackexchange.com/questions/17105/why-do-we-use-injective-surjective-and-bijective-functions-in-computer-science)
- MIT OpenCourseWare: [Single Variable Calculus](https://ocw.mit.edu/courses/mathematics/18-01-single-variable-calculus-fall-2006/)
- Arents: [Mathematik - Kapitel 1](https://link.springer.com/book/10.1007/978-3-662-64389-1)
