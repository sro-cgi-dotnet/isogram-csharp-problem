# Isogram

**Objective:** Setup a solution with test cases to determine if a word or phrase is an isogram.

An isogram (also known as a "nonpattern word") is a word or phrase without a repeating letter, however spaces and hyphens are allowed to appear multiple times.

**Examples of isograms:**
  - lumberjacks
  - background
  - downstream
  - six-year-old

The word isograms, however, is not an isogram, because the s repeats.

## Test Scenarios

```csharp
 [Fact]
    - Should hold true for empty string
    - Should hold true for word `isogram` with lower case characters
    - Should hold false for word `eleven`
    - Should hold true for long reported english word like `subdermatoglyphic`
    - Should hold true for word with duplicated character in mixed case `Alphabet`
    - Should hold true for word with hyphen `thumbscrew-japingly`
    - 
    

    [Fact(Skip = "Remove to run test")]
    public void Isogram_with_duplicated_hyphen()
    {
        Assert.True(Isogram.IsIsogram("six-year-old"));
    }

    [Fact(Skip = "Remove to run test")]
    public void Made_up_name_that_is_an_isogram()
    {
        Assert.True(Isogram.IsIsogram("Emily Jung Schwartzkopf"));
    }

    [Fact(Skip = "Remove to run test")]
    public void Duplicated_character_in_the_middle()
    {
        Assert.False(Isogram.IsIsogram("accentor"));
    }
```

## Note:
- The name of the solution should exactly be `isogram-csharp-problem.sln`
- Don't change the content of files `.gitignore` and `.travis.yml`

## Issues:

Incase of problem raise an issue on https://github.com/nishant-jain-94/isogram-csharp-problem/issues

## Source

Wikipedia https://en.wikipedia.org/wiki/Isogram