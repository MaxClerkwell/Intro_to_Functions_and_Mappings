# Einführung in Abbildungen

## 1. Einleitung
Abbildungen sind ein fundamentales Konzept in Mathematik und Informatik. Sie beschreiben die eindeutige Zuordnung von Elementen einer Menge zu Elementen einer anderen Menge. In der Informatik spielen sie eine zentrale Rolle bei der Datenverarbeitung, Verschlüsselung und Speicheradressierung.

## 2. Definition einer Abbildung
Eine Abbildung ist eine Vorschrift, die jedem Element einer Menge \( A \) genau ein Element einer Menge \( B \) zuordnet. Formal schreiben wir:

\[ f: A \to B, \quad f(a) = b \]

Dabei nennt man:
- \( A \) die **Definitionsmenge** \( D(f) \)
- \( B \) die **Wertemenge** \( W(f) \)
- \( f(A) \) die **Bildmenge**

## 3. Eigenschaften von Abbildungen
### 3.1 Injektivität
Eine Abbildung \( f: X \to Y \) ist **injektiv**, wenn unterschiedliche Eingaben unterschiedliche Ausgaben liefern:

\[ f(x_1) = f(x_2) \Rightarrow x_1 = x_2 \]

**Anwendung in der Informatik:** Speicheradressierung, bei der jede Adresse genau einem Speicherinhalt entspricht.

### 3.2 Surjektivität
Eine Abbildung \( f: X \to Y \) ist **surjektiv**, wenn jeder Wert in \( Y \) von mindestens einem Wert in \( X \) getroffen wird:

\[ \forall y \in Y, \exists x \in X: f(x) = y \]

**Anwendung in der Informatik:** Rundungsfunktionen, die mehreren Eingabewerten denselben Ausgabewert zuordnen.

### 3.3 Bijektivität
Eine Abbildung ist **bijektiv**, wenn sie sowohl injektiv als auch surjektiv ist. Das bedeutet, dass jedes Element aus \( Y \) genau einem Element aus \( X \) zugeordnet wird.

**Anwendung in der Informatik:** Kodierungen, bei denen eine 1:1-Entsprechung zwischen Original- und Kodierungswert besteht.

## 4. Umkehrbarkeit von Abbildungen
Eine Abbildung \( f: X \to Y \) ist **umkehrbar**, wenn es eine Funktion \( g: Y \to X \) gibt, sodass:

\[ g(f(x)) = x \quad \text{und} \quad f(g(y)) = y \]

**Beispiel für eine umkehrbare Funktion:**

\[ f(x) = x - 3, \quad f^{-1}(y) = y + 3 \]

**Wann ist eine Funktion nicht umkehrbar?**
- Wenn sie nicht injektiv ist.
- Beispiel: \( f(x) = x^2 \), da \( f(-2) = f(2) = 4 \) keine eindeutige Umkehrfunktion existiert.

**Anwendung in der Informatik:**
- Einwegfunktionen als Grundlage asymmetrischer Verschlüsselung.

## 5. Darstellung von Abbildungen
Abbildungen können auf verschiedene Weise dargestellt werden:

- **Funktionsgleichungen:** \( f(x) = x^2 \)
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