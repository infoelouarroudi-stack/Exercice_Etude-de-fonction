# Limites et Études de Fonctions - Exercices Complets Terminale

---

## 📚 PARTIE 1 : CALCULS DE LIMITES

### 🔵 Niveau 1 — Faciles (techniques directes : terme dominant / division)

#### Exercice 1
$$\lim_{x\to+\infty}(4x^{3}-2x+1)$$

**Correction :**
* C'est un polynôme de degré 3 : le terme dominant est $4x^3$ qui tend vers $+\infty$ quand $x\to+\infty$.
* **Résultat :** $\boxed{+\infty}$

---

#### Exercice 2
$$\lim_{x\to+\infty}\frac{6x^{2}+3}{2x^{2}-1}$$

**Correction :**
* On divise numérateur et dénominateur par $x^{2}$ :
$$\frac{6+\tfrac{3}{x^{2}}}{2-\tfrac{1}{x^{2}}}\xrightarrow[x\to+\infty]{}\frac{6}{2} = 3$$
* **Résultat :** $\boxed{3}$

---

#### Exercice 3
$$\lim_{x\to -\infty}(-x^{3}+x)$$

**Correction :**
* Terme dominant : $-x^{3}$. Quand $x\to -\infty$, $x^{3}\to -\infty$ donc $-x^{3}\to +\infty$.
* **Résultat :** $\boxed{+\infty}$

---

#### Exercice 4
$$\lim_{x\to 0^{+}}\frac{1}{x}$$

**Correction :**
* Pour $x>0$ très petit, $1/x$ devient très grand positif.
* **Résultat :** $\boxed{+\infty}$ (et la limite bilatérale $x\to0$ n'existe pas)

---

### 🟡 Niveau 2 — Intermédiaires (conjugaison, racines, trigonométrie de base)

#### Exercice 5
$$\lim_{x\to+\infty}\frac{\sqrt{x^{2}+4}}{x}$$

**Correction :**
* Pour $x>0$, $\dfrac{\sqrt{x^{2}+4}}{x}=\sqrt{1+\dfrac{4}{x^{2}}}$.
* Quand $x\to+\infty$, $\tfrac{4}{x^{2}}\to0$ donc la racine tend vers $\sqrt{1}=1$.
* **Résultat :** $\boxed{1}$

---

#### Exercice 6
$$\lim_{x\to+\infty}\big(\sqrt{x^{2}+5x}-x\big)$$

**Correction :**
* Conjugaison :
$$\sqrt{x^{2}+5x}-x=\frac{(\sqrt{x^{2}+5x}-x)(\sqrt{x^{2}+5x}+x)}{\sqrt{x^{2}+5x}+x} =\frac{5x}{\sqrt{x^{2}+5x}+x}$$
* Diviser numérateur et dénominateur par $x$ (pour $x>0$) :
$$=\frac{5}{\sqrt{1+\tfrac{5}{x}}+1}\xrightarrow[x\to+\infty]{}\frac{5}{1+1}=\frac{5}{2}$$
* **Résultat :** $\boxed{\tfrac{5}{2}}$

---

#### Exercice 7
$$\lim_{x\to0}\frac{\sin x}{x}$$

**Correction :**
* Limite fondamentale (échelle angulaire en radians)
* **Résultat :** $\boxed{1}$

---

#### Exercice 8
$$\lim_{x\to0}\frac{1-\cos x}{x^{2}}$$

**Correction :**
* Développement limité : $1-\cos x \sim \dfrac{x^{2}}{2}$.
* Donc $\dfrac{1-\cos x}{x^{2}}\to \dfrac{1}{2}$.
* **Résultat :** $\boxed{\tfrac{1}{2}}$

---

### 🔴 Niveau 3 — Difficiles (DL, équivalents, formes indéterminées, exponentielle)

#### Exercice 9
$$\lim_{x\to0}\frac{\sin x - x}{x^{3}}$$

**Correction :**
* DL : $\sin x = x - \dfrac{x^{3}}{6} + o(x^{3})$.
* Donc $\sin x - x = -\dfrac{x^{3}}{6} + o(x^{3})$.
* Diviser par $x^{3}$ : limite $-\dfrac{1}{6}$.
* **Résultat :** $\boxed{-\tfrac{1}{6}}$

---

#### Exercice 10
$$\lim_{x\to0}\frac{\tan x - x}{x^{3}}$$

**Correction :**
* DL : $\tan x = x + \dfrac{x^{3}}{3} + o(x^{3})$.
* Donc $\tan x - x = \dfrac{x^{3}}{3} + o(x^{3})$.
* Diviser par $x^{3}$ : limite $\dfrac{1}{3}$.
* **Résultat :** $\boxed{\tfrac{1}{3}}$

---

#### Exercice 11
$$\lim_{x\to+\infty}x\big(\sqrt{x^{2}+2}-x\big)$$

**Correction :**
* Conjugaison / simplification :
$$x(\sqrt{x^{2}+2}-x)=\frac{2x}{\sqrt{x^{2}+2}+x}$$
* Diviser num. et dénom. par $x$ :
$$=\frac{2}{\sqrt{1+\tfrac{2}{x^{2}}}+1}\xrightarrow[x\to+\infty]{}\frac{2}{1+1}=1$$
* **Résultat :** $\boxed{1}$

---

#### Exercice 12
$$\lim_{x\to+\infty}\left(1+\frac{2}{x}\right)^{x}$$

**Correction :**
* On reconnait la forme classique $(1+\tfrac{a}{x})^{x}\to e^{a}$ (ici $a=2$).
* Méthode : écrire $\exp\big(x\ln(1+2/x)\big)$, développer $\ln(1+2/x)\sim 2/x$ puis $x\cdot 2/x\to2$.
* **Résultat :** $\boxed{e^{2}}$

---

## 📊 PARTIE 2 : ÉTUDES COMPLÈTES DE FONCTIONS

### 🟠 Exercice 1 : Fonction rationnelle simple

$$f(x) = \frac{x^2 - 4}{x - 1}$$

#### 1️⃣ Domaine de définition
$x \neq 1$ 👉 donc $D_f = \mathbb{R} \setminus \{1\}$

#### 2️⃣ Limites
* $\lim_{x\to 1^-} f(x) = -\infty$
* $\lim_{x\to 1^+} f(x) = +\infty$
* $\lim_{x\to +\infty} f(x) = +\infty$

#### 3️⃣ Dérivée
$$f'(x)=\frac{(2x)(x-1)-(x^2-4)(1)}{(x-1)^2}=\frac{x^2-2x+4}{(x-1)^2}$$

Le numérateur $x^2-2x+4>0$ pour tout $x$. 👉 donc $f'(x)>0$, la fonction est **strictement croissante** sur chaque intervalle de son domaine.

#### 4️⃣ Tableau de variation

| Intervalle | Sens de variation | Limites |
|------------|-------------------|---------|
| $(-\infty, 1)$ | ↗️ | $-\infty \to +\infty$ |
| $(1, +\infty)$ | ↗️ | $-\infty \to +\infty$ |

#### 5️⃣ Interprétation graphique
* **Asymptote verticale :** $x=1$
* **Pas d'asymptote horizontale**
* Courbe croissante des deux côtés

---

### 🟠 Exercice 2 : Fonction avec racine

$$f(x) = \sqrt{x+1} - x$$

#### 1️⃣ Domaine
$x \ge -1$

#### 2️⃣ Limites
* $\lim_{x\to -1^+} f(x)=1$
* $\lim_{x\to +\infty} f(x) = -\infty$

#### 3️⃣ Dérivée
$$f'(x)=\frac{1}{2\sqrt{x+1}} - 1$$

**Signe :**
* $f'(x)>0$ si $x<-\frac{3}{4}$
* $f'(x)<0$ si $x>-\frac{3}{4}$

#### 4️⃣ Tableau de variation

| Intervalle | Signe de f'(x) | Variation |
|------------|----------------|-----------|
| $[-1, -\frac{3}{4}]$ | + | ↗️ |
| $[-\frac{3}{4}, +\infty)$ | - | ↘️ |

#### 5️⃣ Interprétation
* **Maximum en** $x = -\frac{3}{4}$
* Courbe décroissante ensuite

---

### 🟠 Exercice 3 : Fonction polynomiale

$$f(x) = x^3 - 3x^2 + 2$$

#### 1️⃣ Domaine
$\mathbb{R}$

#### 2️⃣ Limites
$\lim_{x\to+\infty}f(x)=+\infty$, $\lim_{x\to-\infty}f(x)=-\infty$

#### 3️⃣ Dérivée
$$f'(x) = 3x^2 - 6x = 3x(x-2)$$

#### 4️⃣ Tableau de signe

| x | $-\infty$ | 0 | 2 | $+\infty$ |
|---|-----------|---|---|-----------|
| f'(x) | + | 0 | - | 0 | + |

#### 5️⃣ Variations
* **Croissante** sur $(-\infty, 0)$
* **Décroissante** sur $(0, 2)$
* **Croissante** sur $(2, +\infty)$

#### 6️⃣ Interprétation
* **Maximum local** en $x=0$
* **Minimum local** en $x=2$

---

### 🟠 Exercice 4 : Fonction rationnelle avec asymptotes

$$f(x) = \frac{2x+3}{x-1}$$

#### 1️⃣ Domaine
$x \neq 1$

#### 2️⃣ Limites
* $\lim_{x\to1^-}f(x)=-\infty$
* $\lim_{x\to1^+}f(x)=+\infty$
* $\lim_{x\to\pm\infty}f(x)=2$

#### 3️⃣ Asymptotes
* **Verticale :** $x=1$
* **Horizontale :** $y=2$

#### 4️⃣ Dérivée
$$f'(x)=\frac{2(x-1)-(2x+3)}{(x-1)^2}=\frac{-5}{(x-1)^2}<0$$

Donc $f$ **strictement décroissante** sur ses deux intervalles.

---

### 🟠 Exercice 5 : Fonction exponentielle

$$f(x) = x e^{-x}$$

#### 1️⃣ Domaine
$\mathbb{R}$

#### 2️⃣ Limites
* $\lim_{x\to-\infty} f(x)=0$
* $\lim_{x\to+\infty} f(x)=0$

#### 3️⃣ Dérivée
$$f'(x) = e^{-x}(1-x)$$

**Signe :**
* $f'(x)>0$ si $x<1$
* $f'(x)<0$ si $x>1$

#### 4️⃣ Variations

| Intervalle | Variation |
|------------|-----------|
| $(-\infty,1)$ | ↗️ |
| $(1,+\infty)$ | ↘️ |

**Maximum** en $x=1$ de valeur $f(1)=\frac{1}{e}$.

#### 5️⃣ Interprétation
Courbe en forme de cloche : monte jusqu'à $x=1$, puis décroît vers 0.

---

## 💡 Conseils pour la séance

### Pour les limites :
* Donne les 4 fonctions du **niveau 1** comme échauffement (contrôle du vocabulaire : terme dominant, degré)
* Enchaîne avec les **n°5–8** (racines, conjugaison, trigonométrie de base) pour travailler les techniques
* Termine par 9–12 (DL, équivalents, exponentielle) pour voir si l'élève maîtrise les développements limités et la manipulation des formes indéterminées

### Pour les études de fonctions :
* Commencer par l'exercice 1 (rationnelle simple)
* Progresser vers l'exercice 2 (racine) et 3 (polynôme)
* Terminer par les exercices 4 et 5 pour les asymptotes et l'exponentielle
