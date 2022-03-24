# The Gilded Rose

![The Gilded Rose in World of Warcraft](img/the-gilded-rose.jpg)

Originally created by [@TerryHughes](https://twitter.com/TerryHughes). [@NotMyself](https://twitter.com/NotMyself) took it and ran with it, creating a .NET starter project on GitHub [here](https://github.com/NotMyself/GildedRose).

[Emily Bache](https://github.com/emilybache) and [friends](https://github.com/emilybache/GildedRose-Refactoring-Kata/graphs/contributors) have created [an amazing collection of starting points in a wide array of languages][bache-repo].

This is an _excellent_ kata - one I recommend repeating often, with different people and trying different ideas.

We almost all live in a world where we're having to improve _existing_ systems. These systems are running and creating value - they pay the salaries and _"can't"_ break.

 These systems were likely created by someone else. Given many people in our industry move jobs every 1-2 years - they're often not available to help. We also all know what it's like going back to code _you_ wrote 12+ months ago 🙈😊 `#alwaysimproving`.

---

## First Time? Start here!

1. Start a new project in your IDE of choice (or clone a starter kit from the [README](/README.md))
1. Copy-and-paste the existing code from [Emily Bache's repository][bache-repo] for your language of choice. ⚠ **Do not clone the entire repository!** Common languages:
    * C# (on .NET Core) - [`GildedRose.cs`](https://raw.githubusercontent.com/emilybache/GildedRose-Refactoring-Kata/main/csharpcore/GildedRose/GildedRose.cs) and [`Item.cs`](https://raw.githubusercontent.com/emilybache/GildedRose-Refactoring-Kata/main/csharpcore/GildedRose/Item.cs)
    * TypeScript - [`gilded-rose.ts`](https://raw.githubusercontent.com/emilybache/GildedRose-Refactoring-Kata/main/TypeScript/app/gilded-rose.ts)
1. Start adding tests as you sit fit. Be conscious of:
    * Speed of adding new tests.
    * Naming of the tests - is it clear what's broken if they fail?
    * Tracking completedness of the suite.

---

## Outline

* The focus of this Kata is **refactoring** - changing the design of the code, but _without_ changing it's external behaviour. This generally means either keeping - or adding - features - without breaking existing ones.
* Be sure to read the specification - and it's constraints - _thoroughly_ before starting!
* **Practice requirements:**
  * [Test-Driven Development](https://en.wikipedia.org/wiki/Test-driven_development) - this is how we ensure we don't break existing functionality.
  * [Pair Programming](https://en.wikipedia.org/wiki/Pair_programming) - this is how we best create code that is easy to understand and maintain. You can also consider [Mobbing](https://en.wikipedia.org/wiki/Mob_programming).

> ℹ Remember, **code is for people** - readability, testability and maintainability are key.

[bache-repo]:https://github.com/emilybache/GildedRose-Refactoring-Kata