---
Index: 11
---

``` csharp

// C# Naming Conventions Example 
// -----------------------------------------------
// General rule:
// - Classes, Properties, and Methods = PascalCase
// - Private fields and local variables = camelCase (sometime people use underscore in front of variables '_number')
// - Constants = ALL_CAPS (optional, less common)

// CLASS (PascalCase)
public class Animal
{
    // PRIVATE FIELD (camelCase, no underscore)
    private int energyLevel;

    // PROPERTY (PascalCase)
    public string Name { get; set; }

    // PROPERTY (PascalCase)
    public int Age { get; set; }

    // CONSTANT (PascalCase)  (sometimes ALL_CAPS in older styles or personal preference 'MAXAGE')
    public const int MaxAge = 20;   // PascalCase (recommended in C#)


    // METHOD (PascalCase)
    public void MakeSound()
    {
        // LOCAL VARIABLE (camelCase)
        string sound = "Generic sound";

        Console.WriteLine($"{Name} makes a {sound}!");
    }

    // METHOD (PascalCase) with parameter (camelCase)
    public void FeedAnimal(int foodAmount)
    {
        // LOCAL VARIABLE (camelCase)
        int gainedEnergy = foodAmount * 2;
        energyLevel += gainedEnergy;
    }
}

// -----------------------------------------------
// USING THE CLASS

// LOCAL VARIABLES (camelCase)
Animal cat = new Animal { Name = "Whiskers", Age = 3 };
Animal dog = new Animal { Name = "Buddy", Age = 5 };

// CALLING METHODS (PascalCase)
cat.MakeSound();
dog.FeedAnimal(10);
```
