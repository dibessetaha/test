### Exemple Illustratif:

Prenons un exemple simple avec \(k = 2\) et \(n = 3\).

#### Matrice génératrice \(G\):
Supposons que la matrice génératrice \(G\) soit:
\[ G = \begin{pmatrix}
1 & 0 \\
0 & 1 \\
1 & 1
\end{pmatrix} \]

#### Encodage d'un vecteur message \(m\):
Pour un vecteur message \(m = \begin{pmatrix} m_1 \\ m_2 \end{pmatrix}\), le vecteur code est obtenu en multipliant \(G\) par \(m\):
\[ \phi(m) = G \times m = \begin{pmatrix}
1 & 0 \\
0 & 1 \\
1 & 1
\end{pmatrix} \times \begin{pmatrix}
m_1 \\
m_2
\end{pmatrix} = \begin{pmatrix}
m_1 \\
m_2 \\
m_1 + m_2
\end{pmatrix} \]

#### Exemples de vecteurs messages:
1. Si \(m = \begin{pmatrix} 1 \\ 0 \end{pmatrix}\), alors:
\[ \phi(m) = \begin{pmatrix} 1 \\ 0 \\ 1 \end{pmatrix} \]

2. Si \(m = \begin{pmatrix} 0 \\ 1 \end{pmatrix}\), alors:
\[ \phi(m) = \begin{pmatrix} 0 \\ 1 \\ 1 \end{pmatrix} \]

3. Si \(m = \begin{pmatrix} 1 \\ 1 \end{pmatrix}\), alors:
\[ \phi(m) = \begin{pmatrix} 1 \\ 1 \\ 0 \end{pmatrix} \]

4. Si \(m = \begin{pmatrix} 0 \\ 0 \end{pmatrix}\), alors:
\[ \phi(m) = \begin{pmatrix} 0 \\ 0 \\ 0 \end{pmatrix} \]

### Interprétation:
- Chaque vecteur code \(\phi(m)\) est un vecteur de longueur \(n = 3\) obtenu en multipliant la matrice génératrice \(G\) par le vecteur message \(m\).
- Les premiers \(k = 2\) bits du vecteur code sont les bits du message original.
- Le dernier bit est un bit de parité calculé comme la somme binaire des bits du message.

### Conclusion:
Cet exemple illustre comment un code linéaire utilise une matrice génératrice pour encoder des messages. En particulier, il montre comment les bits du message original et des bits de parité sont combinés pour former le vecteur code.
