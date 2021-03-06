# Jeu de calcul mental

## Pseudo-Code

_Le pseudo-code est important, c'est l'étape qui permet de mettre à plat ses idées. Le mieux est de le faire sur papier et d'écrire le déroulement de l'algorithme, en français, comme si tu rédigeais une liste de choses à faire._

**Conseil France IOI :**

**Lisez bien les exemples ! Ils sont là pour vous aider, pour que vous compreniez bien quelles sont les données à lire et ce que doit calculer votre programme.**

**Les exemples du sujet sont d'excellents supports pour vous assurer que vous avez bien compris le problème posé. À chaque fois, essayez pour chaque exemple de calculer vous-même le résultat à partir des données d'entrée, et vérifiez que la sortie correspond. Si vous n'êtes pas d'accord avec l'exemple, vous aurez beaucoup de mal à résoudre l'exercice !**

Le nom à multiplier, dans cet exercice, est TOUJOURS 66. Ce qui change, c'est le nombre de fois où l'on enchaîne les opérations de calculs.

```
Je récupère l'entrée
J'initie mon résultat à 66
Je répète autant de fois que mon entrée
  J'assigne résultat = résultat * numéro de boucle
  J'affiche résultat
```

## Python

<details>
  <summary>Solution</summary>

```Python
nbNombres = int(input())
étape = 0
résultat = 66
for loop in range(nbNombres):
   étape = étape + 1
   résultat = résultat * étape
   print(résultat)
```

</details>

## Java

Code minimal Java

<details>
  <summary>Minimum fonctionnel</summary>

```Java
  class Main {
    public static void main(String[] args) {
      // ton code ici
    }
  }
```

</details>

</br>
Et avec les instructions :)
</br>
</br>

<details>
  <summary>Solution</summary>


```Java
import algorea.Scanner;
class Main {
   static Scanner entrée = new Scanner(System.in);
   public static void main(String[] args) {
      int nbNombres = entrée.nextInt();
      int résultat = 66;
      for (int facteur = 1; facteur <= nbNombres; facteur = facteur + 1) {
         résultat = résultat * facteur;
         System.out.println(résultat);
      }
   }
}
```

</details>
