

# Java

```java
class Main{
  public static void main(String[] args){
    System.out.println("Hello world");
  }
}
```

Description de la fonction main

##Prototype d'une méthode

Une méthode est rendue unique et distincte grâce à son prototype : nom de la méthode, type de valeur de retour, liste et types des arguments)

##Types

##Classe

##Instance

##Constructeur

Les constructeurs permettent d'effectuer un certain traitement au moment de l'instanciation de l'objet lui même. Un constructeur est une méthode qui a la particularité de posséder le même nom que la classe à laquelle il appartient. Pour reprendre notre exemple, pour éviter d'invoquer les méthodes setNom() et setCouleur() juste après l'instanciation, on pourrait mettre ce traitement dans le constructeur de cette façon :

EXEMPLE ######

public class Chien extends Animal {
    public Chien(String nom, String couleur) {
        setNom(nom);
        setCouleur(couleur);
    }
    public String aboie() {
        return "OUAF OUAF";
    }
}

Et instancier le Chien comme suit :

Chien monChien = new Chien("Médor", "Noir");

Cependant, si on veut que tous les animaux bénéficient de ce constructeur bien pratique, il aurait fallu le mettre directement dans la classe Animal. Dans ce cas, il faut aussi créer un constructeur dans la classe Chien qui invoque le constructeur de sa surclasse. Le mot clé super sert à ça :

public class Animal {
    String nom, couleur;
    public Animal(String nom, String couleur) {
        this.nom = nom;
        this.couleur = couleur;
    }
    public getNom() {
        return nom;
    ...

public class Chien extends Animal {
    public Chien(String nom, String couleur) {
        super(nom, couleur);
    }
    public String aboie() {
        return "OUAF OUAF";
    }
}

#############

##Static

Usage du mot clé `static`

##Abstract

Usage du mot clé `abstract`

##Boucles

##Classes utilitaires

1.    ArrayList



##Interfaces

##Exceptions
1.  try... catch... finally

2. throw

3. throws

# Design Patterns

##Decorator

Permet d'agrémenter un objet de nouvelles methodes en l'encapsulant dans une classe Decorator.

##Singleton

Description du singleton

##Observer

![Pattern Observer](https://raw.githubusercontent.com/clm-a/java-notes/master/observer.png "Pattern Observer")

Description d'observer

##MVC

Description du pattern MVC

##Factory

Description du pattern Factory
