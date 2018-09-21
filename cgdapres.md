# CGDA Presentations

Here are the presentations I have done for the Calgary Game Developers Association:
### September 2018 - Custom Unity Inspectors

Expanding on the presentation I did in 2016, here is some sample code of writing your own inspector. And there is a sample of an Editor window.

[**View Slides**](https://docs.google.com/presentation/d/1nHAmR-JZefxOezRR0lhRkhb0oin7ZDGW5BdllYIQs80/edit?usp=sharing)

Here are the code samples:




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
