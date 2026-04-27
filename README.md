# AlgoStudio
AlgoStudio is a lightweight IDE designed for learning and writing algorithms with a custom syntax, auto-completion, and error detection.
# AlgoStudio 🖥️

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20Mac-lightgrey)
![License](https://img.shields.io/badge/License-MIT-green)
![Size](https://img.shields.io/github/repo-size/ZIANIAyyoub/AlgoStudio)
![Stars](https://img.shields.io/github/stars/ZIANIAyyoub/AlgoStudio?style=social)

> **Compilateur et interpréteur de pseudocode algorithmique en français.**  
> Application bureau complète — Python 3 + Tkinter, sans aucune dépendance externe.

Développé par **ZIANI Ayyoub**

---

## 📸 Aperçu


<img width="1916" height="1018" alt="image" src="https://github.com/user-attachments/assets/b3b838e9-a91e-4c9e-8bd4-21c268b7b16c" />
.
<img width="1495" height="783" alt="image" src="https://github.com/user-attachments/assets/90ad47b6-db19-49c1-9e30-eb0153cb3048" />
.
<img width="357" height="345" alt="image" src="https://github.com/user-attachments/assets/526c9bb9-4d6e-4c3e-b2e5-b195ec7d1310" />



---

## ✨ Fonctionnalités

| Fonctionnalité | Description |
|----------------|-------------|
| ▶️ **Exécution directe** | Interprète et exécute le pseudocode en temps réel |
| 💡 **Auto-complétion** | Suggestions intelligentes : mots-clés + vos variables |
| 📊 **Variables en direct** | Visualiseur live de toutes les variables pendant l'exécution |
| ⬆️ **Export C / Python** | Génère du code C ou Python à partir de votre algorithme |
| 📄 **Onglets multiples** | Travaillez sur plusieurs fichiers simultanément |
| 🔍 **Recherche avancée** | Chercher et remplacer avec surlignage |
| 🎨 **Thèmes** | Dark / Light — sauvegardés automatiquement |
| 💾 **Session persistante** | Vos fichiers ouverts sont restaurés au prochain lancement |
| 📖 **Exemples intégrés** | Bibliothèque d'exemples organisée par chapitre (Ch.1 à Ch.8) |

---

## 🚀 Installation et lancement

### Prérequis
- Python **3.8 ou supérieur**
- Tkinter (inclus par défaut avec Python)

### Lancement
```bash
# Cloner le dépôt
git clone https://github.com/zianiayyoub06-hub/AlgoStudio.git
cd AlgoStudio

# Lancer l'application
python main.py
```

> ✅ Aucune installation de bibliothèque requise.

---

## ⌨️ Raccourcis clavier

| Raccourci | Action |
|-----------|--------|
| `F5` | ▶ Exécuter l'algorithme |
| `F6` | ■ Arrêter l'exécution |
| `F7` | 📊 Visualiseur de variables (Live) |
| `Ctrl+T` | 📄 Nouvel onglet |
| `Ctrl+W` | ✕ Fermer l'onglet courant |
| `Ctrl+Espace` | 💡 Auto-complétion |
| `Ctrl+F` | 🔍 Chercher / Remplacer |
| `Ctrl+/` | 💬 Commenter / Décommenter la ligne |
| `Tab` | → Indenter / Valider une suggestion |
| `Échap` | ✕ Fermer la suggestion |

---

## 📝 Structure d'un algorithme

```
Algorithme <Nom>;

Type <NomType> = Enregistrement    // optionnel
    champ : Type;
Fin;

Var
    variable   : Entier;
    tab[N]     : Tableau De Entier;
    ptr        : ^Entier;          // pointeur

Debut
    <instructions>
Fin.
```

---

## 💡 Exemple rapide

```
Algorithme TableDeMultiplication;
Var
    n, i : Entier;
Debut
    Ecrire("Entrez un nombre :");
    Lire(n);
    Pour i <- 1 a 10 Faire
        Ecrire(n, "x", i, "=", n * i);
    FinPour;
Fin.
```

---

## 📁 Structure du projet

```
AlgoStudio/
├── main.py          ← Point d'entrée — lancer ici
├── app.py           ← Interface graphique (Tkinter)
├── lexer.py         ← Tokeniseur (Lexer)
├── ast_nodes.py     ← Nœuds AST
├── parser.py        ← Analyse syntaxique (Parser)
├── interpreter.py   ← Exécution (Interpréteur)
├── codegen.py       ← Export vers C et Python
├── themes.py        ← Thèmes de couleurs
└── examples.py      ← Exemples intégrés par chapitre
```

--
╔══════════════════════════════════════════════════════════════════╗
║  RÉFÉRENCE OFFICIELLE — AlgoStudio                         ║
║  ZIANI AYYOUB  —  PYTHON —  ENSEIGNEMENT                         ║
╚══════════════════════════════════════════════════════════════════╝

▶ 1. STRUCTURE GÉNÉRALE
══════════════════════════════════════════════════════════════════
Algorithme <Nom>;
    Const
        <Nom> = <Valeur>;
    Var
        <Nom> : <Type>;
    Debut
        <Instructions>;
    Fin.

▶ 2. TYPES DE DONNÉES
══════════════════════════════════════════════════════════════════
    Entier       Nombre entier            ex: 5, -3, 100
    Reel         Nombre réel              ex: 3.14, -2.5
    Caractere    Un caractère             ex: 'a', 'Z'
    Chaine       Chaîne de caractères     ex: "bonjour"
    Booleen      Booléen                  Vrai  ou  Faux

▶ 3. TABLEAUX
══════════════════════════════════════════════════════════════════
  // 1D  (syntaxe officielle : taille avant les deux-points)
    T[100] : Tableau De Entier;
    C[50]  : Tableau De Caractere;    // tableau de caractères

  // 2D (matrice)
    M[10][10] : Tableau De Reel;

  // Tableau d'enregistrements
    etuds[30] : Tableau De Etudiant;

  // Paramètre de fonction (sans taille)
    Procedure Tri(T : Tableau De Entier; n : Entier);

  // Accès
    T[i] <- valeur;       M[i][j] <- valeur;
    etuds[1].nom <- "Ali";

▶ 4. AFFECTATION
══════════════════════════════════════════════════════════════════
  variable <- <expression>;       // opérateur officiel
  variable := <expression>;       // accepté aussi

▶ 5. OPÉRATEURS
══════════════════════════════════════════════════════════════════
  Arithmétiques :  +  -  *  /  Div  Mod
    Comparaison   :  =  <>  <  >  <=  >=
    Logiques      :  Et  Ou  Non  (priorité : Non > Et > Ou)

▶ 6. ENTRÉE / SORTIE
══════════════════════════════════════════════════════════════════
    Lire(var1, var2, ...);
    Ecrire(expr1, expr2, ...);

▶ 7. CONDITIONS
══════════════════════════════════════════════════════════════════
    Si <condition> Alors
        <instructions>;
    FinSi;

    Si <condition> Alors ... Sinon ... FinSi;

▶ 8. BOUCLES
══════════════════════════════════════════════════════════════════
  // Pour — fermeture : FinPour
    Pour <compteur> <- <debut> a <fin> [Pas <pas>] Faire
        <instructions>;
    FinPour;

  // TantQue — fermeture : FinTantQue
    TantQue <condition> Faire
        <instructions>;
    FinTantQue;

  // Répéter — s'exécute au moins 1 fois
    Repeter
        <instructions>;
    JusquA <condition>;

  // Contrôle de boucle  ★ NOUVEAU
  Arreter;      // sortir immédiatement de la boucle (break)
  Continuer;    // passer à l'itération suivante (continue)

▶ 9. SELON / CAS  (Switch)
══════════════════════════════════════════════════════════════════
    Selon <expression> Faire
        Cas <valeur1>: <instructions>;
        Cas <valeur2>: <instructions>;
        Autrement: <instructions>;
    FinSelon;

▶ 10. FONCTIONS ET PROCÉDURES
══════════════════════════════════════════════════════════════════
  // Déclarées AVANT l'algorithme principal

    Fonction <Nom>(<Params>) : <TypeRetour>;
    Var <locales>;
    Debut
        ...
        Retourner(<expression>);
    Fin;

    Procedure <Nom>(<Params>);
    Var <locales>;
    Debut  ...  Fin;

  // Passage tableau en paramètre (sans taille)
    Procedure Remplir(T : Tableau De Entier; n : Entier);

▶ 11. ENREGISTREMENTS
══════════════════════════════════════════════════════════════════
  // Déclaré APRÈS l_en-tête Algorithme, AVANT Var
    Type NomType = Enregistrement
        champ1 : Type1;
        champ2 : Type2;
    Fin;

    Var e : NomType;
    e.champ1 <- valeur;
    Ecrire(e.champ2);

▶ 12. POINTEURS  ★ DEUX SYNTAXES ACCEPTÉES
══════════════════════════════════════════════════════════════════
  // Syntaxe classique
    p : Pointeur Vers <Type>;

  // Syntaxe C-like  (nouveau)
  p : ^<Type>;           // ex:  p : ^Ville    p : ^Entier

  // Allocation / Libération
  Nouveau(p);            // alloue un enregistrement
  Liberer(p);            // libère

  // Accès
  p^.champ <- val;       // notation ^ (caret)
  p->champ <- val;       // notation -> (flèche, la plus utilisée)

  // Valeur nulle
    p <- NIL;

▶ 13. FICHIERS
══════════════════════════════════════════════════════════════════
    Var f : Fichier;

    Ouvrir(f, "chemin/nom.dat", "lecture");
    Ouvrir(f, "chemin/nom.dat", "ecriture");
    Ouvrir(f, "chemin/nom.dat", "mise a jour");

    TantQue Non FinFichier(f) Faire
        Lire(f, enreg);
    FinTantQue;

    Ecrire(f, variable);
    Fermer(f);

▶ 14. PILES  (Ch9)
══════════════════════════════════════════════════════════════════
  Empiler(P, element);       // ajouter au sommet
  Depiler(P, &element);      // retirer du sommet
  x <- Sommet(P);            // consulter sans supprimer
  b <- PileVide(P);          // Vrai si vide

▶ 15. FILES  (Ch10)
══════════════════════════════════════════════════════════════════
  Enfiler(F, element);       // ajouter en queue
  Defiler(F, &element);      // retirer de la tête
  x <- Tete(F);              // consulter sans supprimer
  b <- FileVide(F);          // Vrai si vide

▶ 16. FONCTIONS PRÉDÉFINIES
══════════════════════════════════════════════════════════════════
  // Chaînes
    longueur(ch)                    → Entier
    concat(ch1, ch2)                → Chaine
    sous_chaine(ch, debut, fin)     → Chaine
    trouve(ch, motif)               → Entier  (-1 si absent)
    remplace(ch, ancien, nouveau)   → Chaine
    majuscule(ch) / minuscule(ch)   → Chaine
    trim(ch)                        → Chaine

  // Tableau De Caractere
    chaine_vers_tableau(s)          → Tableau De Caractere
    tableau_vers_chaine(tab)        → Chaine

  // Mathématiques
    abs(x)   sqrt(x)   pow(x,n)   arrondi(x,n)
    sin(x)   cos(x)    tan(x)     log(x)   log2(x)   log10(x)
    max(a,b) min(a,b)  entier(x)  reel(x)

  // Divers
    aleatoire()          → Reel   (0..1)
    aleatoire_entier(a,b)→ Entier
    ord(c) / chr(n)      → Entier / Caractere

▶ 17. EXPORT  ★ NOUVEAU
══════════════════════════════════════════════════════════════════
    Menu Outils → Exporter vers C        (.c)
    Menu Outils → Exporter vers Python   (.py)
    L'algorithme est converti en code exécutable.

▶ 18. RACCOURCIS CLAVIER
══════════════════════════════════════════════════════════════════
    F5              ▶  Exécuter
    F6              ■  Arrêter
    F7              📊 Live Variables (variables en temps réel)
    Ctrl+Espace     💡 Suggestions (mots-clés + vos variables)
    Ctrl+F          🔍 Chercher / Remplacer
    Ctrl+/          Commenter / Décommenter
    Tab             Indentation automatique / Valider suggestion
    Échap           Fermer la suggestion


---

## 📄 Licence

Ce projet est sous licence **MIT** — voir le fichier [LICENSE](LICENSE) pour plus de détails.

---




# 🚀 AlgoStudio

**AlgoStudio** هو بيئة تطوير (IDE) خفيفة وموجهة لتعلم وكتابة الخوارزميات بطريقة سهلة وبسيطة، مع دعم syntax مخصص وأدوات مساعدة للمبتدئين والمحترفين.

---

## ✨ المميزات

* 🧠 Syntax مخصص للخوارزميات
* ⚡ Auto-completion ذكي
* 🔍 كشف الأخطاء (Syntax checking)
* 🖥️ واجهة رسومية سهلة الاستعمال
* 📂 دعم الملفات (قراءة / كتابة)
* 🔄 إمكانية تطويره وتحويله للغات أخرى (Python / C)

---

## 📸 Screenshots

> أضف هنا صور من البرنامج

---

## ⚙️ التثبيت

### 🔹 نسخة جاهزة (exe)

1. حمل الملف من قسم **Releases**
2. شغل البرنامج مباشرة (لا يحتاج Python)

### 🔹 تشغيل من الكود

```bash
git clone https://github.com/zianiayyoub06-hub/AlgoStudio.git
cd AlgoStudio
pip install -r requirements.txt
python main.py
```

---

## 📁 هيكلة المشروع

```
AlgoStudio/
│
├── main.py
├── core/
├── ui/
├── assets/
├── examples/
├── README.md
└── requirements.txt
```

---

## 🛠️ التقنيات المستعملة

* Python
* Tkinter / PyQt (حسب مشروعك)
* Custom Parser (AST)

---


---

## 📄 الرخصة

هذا المشروع تحت رخصة MIT.

---

## 👨‍💻 المطور

Developed by **[ziani ayyoub]**

---

⭐ إذا عجبك المشروع، عطينا Star!



## 📬 Contact

**ZIANI Ayyoub** — zianiayyoub06@gmail.com

Si ce projet vous a été utile, laissez une ⭐ sur GitHub !
