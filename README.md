# randomStringGenerator
Random string generator for c# using LINQ

```cs
//To generate a random alphanumeric string of a specified length
 public static string RandomString(int length)
  {
    const string chars = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789";
    var random = new Random();
    return new string(Enumerable.Repeat(chars, length).Select(s => s[random.Next(s.Length)]).ToArray());
  }
```
