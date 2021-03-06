# TITRE DE L'EXERCICE

## Pseudo-Code

_Le pseudo-code est important, c'est l'étape qui permet de mettre à plat ses idées. Le mieux est de le faire sur papier et d'écrire le déroulement de l'algorithme, en français, comme si tu rédigeais une liste de choses à faire._

**Conseil France IOI :**

**Lisez bien les exemples ! Ils sont là pour vous aider, pour que vous compreniez bien quelles sont les données à lire et ce que doit calculer votre programme.**

**Les exemples du sujet sont d'excellents supports pour vous assurer que vous avez bien compris le problème posé. À chaque fois, essayez pour chaque exemple de calculer vous-même le résultat à partir des données d'entrée, et vérifiez que la sortie correspond. Si vous n'êtes pas d'accord avec l'exemple, vous aurez beaucoup de mal à résoudre l'exercice !**

On utilise une boucle « tant que » pour répéter des instructions tant que le nombre n'a pas été trouvé. Au sein de cette boucle, on va donc tester si la proposition de l'enfant est trop grande ou trop petite. On sait qu'on a un proposition != àDeviner dans la boucle, donc il faut que la variable proposition soit déjà définie à ce moment là. On peut donc commencer par lire un premier nombre avant de rentrer dans la boucle. On sait en effet que l'enfant finira par donner la même valeur donc on aura au moins une proposition à lire. 

```
àDeviner <- lireEntier()
proposition <- lireEntier()
nbEssais <- 1
Tant que proposition != àDeviner
   Si proposition < àDeviner
      Afficher "c'est plus"
   Si proposition > àDeviner
      Afficher "c'est moins"
   proposition <- lireEntier()
   nbEssais <- nbEssais + 1
Afficher "Nombre d'essais nécessaires :", nbEssais
```

## Python

<details>
  <summary>Solution</summary>

```Python
aDeviner = int(input())
proposition = int(input())
nbEssais = 1
while proposition != aDeviner:
   if proposition < aDeviner:
      print("c'est plus")
   if proposition > aDeviner:
      print("c'est moins")
   proposition = int(input())
   nbEssais = nbEssais + 1
print("Nombre d'essais nécessaires : ")
print(nbEssais)
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
class Main
{
   public static void main(String[] args)
   {
      Scanner entrée = new Scanner(System.in);
      int àDeviner = entrée.nextInt();
      int proposition = àDeviner + 1;
      int nbEssais = 0;
      while (proposition != àDeviner)
      {
         proposition = entrée.nextInt();
         if (proposition < àDeviner)
         {
            System.out.println("c'est plus");
         }
         if (proposition > àDeviner)
         {
            System.out.println("c'est moins");
         }
         nbEssais = nbEssais + 1;
      }
      System.out.println("Nombre d'essais nécessaires : ");
      System.out.println(nbEssais);
   }
}
```

</details>
