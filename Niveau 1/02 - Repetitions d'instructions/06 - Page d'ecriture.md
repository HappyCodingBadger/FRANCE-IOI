# Page d'écriture

## Pseudo-Code

_Le pseudo-code est important, c'est l'étape qui permet de mettre à plat ses idées. Le mieux est de le faire sur papier et d'écrire le déroulement de l'algorithme, en français, comme si tu rédigeais une liste de choses à faire._

**Conseil France IOI :**

**Lisez bien les exemples ! Ils sont là pour vous aider, pour que vous compreniez bien quelles sont les données à lire et ce que doit calculer votre programme.**

**Les exemples du sujet sont d'excellents supports pour vous assurer que vous avez bien compris le problème posé. À chaque fois, essayez pour chaque exemple de calculer vous-même le résultat à partir des données d'entrée, et vérifiez que la sortie correspond. Si vous n'êtes pas d'accord avec l'exemple, vous aurez beaucoup de mal à résoudre l'exercice !**

Ici on voit la différence entre imprimer sur la même ligne et imprimer avec un retour à la ligne. La différence est subtile mais utile selon l'affichage qu'on voudra faire plus tard. Une fois que cette notion est compris, il ne s'agit rien de plus que de boucles et d'impression.

```
Je répète 30 fois sur la même ligne
  j'imprime a_
Je reviens à la ligne
Je répète 30 fois sur la même ligne
  j'imprime b_
Je reviens à la ligne
Je répète 30 fois sur la même ligne
  j'imprime b_
je reviens à la ligne
```

## Python

<details>
  <summary>Solution</summary>

```Python
for loop in range(30):
   print("a_", end = "")
print()
for loop in range(30):
   print("b_", end = "")
print()
for loop in range(30):
   print("c_", end = "")
print()
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
class Main {
   public static void main(String[] args) {
      for (int loop = 1; loop <= 30; loop = loop + 1) {
         System.out.print("a_");
      }
      System.out.println();
    
      for (int loop = 1; loop <= 30; loop = loop + 1) {
         System.out.print("b_");
      }
      System.out.println();
    
      for (int loop = 1; loop <= 30; loop = loop + 1) {
         System.out.print("c_");
      }
      System.out.println();
   }
}
```

</details>
