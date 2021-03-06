# Impression d'étiquette

## Pseudo-Code

_Le pseudo-code est important, c'est l'étape qui permet de mettre à plat ses idées. Le mieux est de le faire sur papier et d'écrire le déroulement de l'algorithme, en français, comme si tu rédigeais une liste de choses à faire._

**Conseil France IOI :**

**Lisez bien les exemples ! Ils sont là pour vous aider, pour que vous compreniez bien quelles sont les données à lire et ce que doit calculer votre programme.**

**Les exemples du sujet sont d'excellents supports pour vous assurer que vous avez bien compris le problème posé. À chaque fois, essayez pour chaque exemple de calculer vous-même le résultat à partir des données d'entrée, et vérifiez que la sortie correspond. Si vous n'êtes pas d'accord avec l'exemple, vous aurez beaucoup de mal à résoudre l'exercice !**

On commence par lire l’ensemble de la ligne de texte, puis on affiche chacun des caractères, sur sa propre ligne. 

```

```

## Python

<details>
  <summary>Solution</summary>

```Python
texte = input()
for idCaractere in range(len(texte)):
   print(texte[idCaractere])
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
      Scanner input = new Scanner(System.in);
      
      String ligne = input.nextLine();
      for (int iCar = 0; iCar < ligne.length(); iCar = iCar + 1)
      {
         System.out.println(ligne.charAt(iCar));
      }
   }
}
```

</details>
