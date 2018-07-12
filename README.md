# Posts:

[**Ludum Dare 41**](ld41)

[**Global Game Jam 2018**](ggj2018)

[**S.A.C. RPG Prototyve**](sacrpg)

[**Ludum Dare 39**](ld39)

[**Ludum Dare 38**](ld38)

[**ShaderForge - 2D Sprite Outline**](spriteoutline)

[**Global Game Jam 2017**](ggj2017)

[**Older Game Jams**](oldjams)


# Presentations:

Here are the presentations I have done for the Calgary Game Developers Association:

### September 2017 - Game Genie presentation

How did these cheating devices work? And why are they uncommon now? How do you protect against them?

[**View Slides**](https://docs.google.com/presentation/d/1n1DXBCkOoAsyz6Ov7Trrt5_AiiNDuMzD4TH8SJX1TlU/edit?usp=sharing)

Here is the example I showed of obfuscating variables to make them harder to find.

```C#
//more secure float
public struct sfloat
{
    private float value;
    private float offset;
    public sfloat(float firstValue = 0f)
    {
        set(firstValue);
    }
    public void set(float newValue)
    {
        offset = Random.Range(-1000, 1000);
        value = newValue - offset;
    }
    public float get()
    {
        return value + offset;
    }
    static public implicit operator float(sfloat secureFloat)
    {//implicit conversion to float
        return secureFloat.get()
    }
}
```

### January 2016 - Unity inspector tricks

Some neat tricks you can use to make using the inspector in Unity more pleasant.

[View Slides](https://docs.google.com/presentation/d/1Q2jKwT85nTVqV1zcmusctR1bkySkPw5-TAwqZo7yd7Y/edit?usp=sharing)


# Ryan Dallaire

A Director of the [Calgary Game Developers Association](http://www.calgarygamedevelopers.com/)

Hobbyist Game Developer

C# Programmer


Email: Ryan.W.Dallaire@gmail.com

Email: Ryan@CalgaryGameDevelopers.com

Twitter: @RyanWDallaire  _I don't use it_

PGP: https://keybase.io/freedomdown
