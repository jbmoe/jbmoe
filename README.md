```csharp
namespace Github;

public class Profile
{
    public Profile()
    {
        Name = "Jeppe Bach Møller";
        MotherTongue = new CultureInfo("da");
        Location = new RegionInfo("DK");
        CurrentJob = "Software Developer at Novicell";
        LinkedIn = new Uri("https://www.linkedin.com/in/jeppebachmøller/");
    }

    public string Name { get; set; }
    public CultureInfo MotherTongue { get; set; }
    public RegionInfo Location { get; set; }
    public string CurrentJob { get; set; }
    public Uri LinkedIn { get; set; }

    public void DisplayGreeting()
    {
        Console.WriteLine($"Hello, I'm {Name}! I live in {Location} and work as a {CurrentJob}.");
        // Hello, I'm Jeppe Bach Møller! I live in DK and work as a Software Developer at Novicell.
    }

    public void DisplayThankYou()
    {
        Console.WriteLine("Thank you for visiting my GitHub profile!");
    }
}
```
