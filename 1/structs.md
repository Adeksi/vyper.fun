# Chapter 4: Structs

Sometimes you need a more complex data type. For this, Vyper provides `structs`:

```vyper
struct Person:
    age: uint256
    name: String[64]
```

Structs allow you to create more complicated data types that have multiple properties.

> Note that we just introduced a new type, String. Fixed-size Strings can hold strings with equal or fewer characters than the maximum length of the string.
>
> ```vyper
> testString: String[100] = "Hello World!"
> ```
>
> The above `testString` can hold upto 100 characters. We have only used 12 characters in `"Hello World!"`

## Put it to the test

In our app, we're going to want to create some Pokemons! And Pokemons will have multiple properties, so this is a perfect use case for a struct.

1. Create a `struct` named `Pokemon`.

2. Our Pokemon struct will have 5 properties:
   - `name` (`String[32]`)
   - `dna` (`uint256`)
   - `HP` (`uint256`)
   - `matches` (`uint256`)
   - `wins` (`uint256`)

<!-- tabs:start -->

#### ** Template **

[embedded-code](../assets/1/1.4-template-code.vy ':include :type=code embed-template')

#### ** Solution **

[embedded-code-final](../assets/1/1.4-finished-code.vy ':include :type=code embed-final')

#### ** Previous Chapter Solution **

[embedded-code-previous](../assets/1/1.3-finished-code.vy ':include :type=code embed-previous')

<!-- tabs:end -->