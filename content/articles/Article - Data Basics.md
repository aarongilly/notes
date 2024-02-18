---
created: 2022-07-22
tags:
  - data
  - article
aliases:
---
Upfront: “data” is the plural of “datum”. It is not a singular noun, it is plural. I will refer to it as such.

# What are Data?

Data are information encoded into a form suitable for storage, transmission, or processing. If you Google the definition of “data”, you get:

> facts and statistics collected together for reference or analysis. - Google’s main definition for “data”

## Facts are Not in Fact, Facts

Data, though, are not “facts” in the _traditional_ sense of the word. “Fact” means something else in dataspeak(tm).

Firstly, data “facts” can be outright wrong. Factual inaccuracy in data happens all the time. Open up the contacts app on your phone. Call every single number in there you’d find a fair few that are no longer factually accurate, yet these records are referred to as "facts". The record stored in your contacts app (probably in a SQLite database, under the hood), contains many “facts” that may not be _true._

Secondly, data can be fundamentally accurate, but incorrectly parsed. If I told you I have woke up today at ‘2021-05-10T11:45.000Z’, you may think me a lazy bum sleeping until almost noon - that’s an easy conclusion to jump to. If I told you that “T11:45.000Z” means 11:45AM according to the _Coordinated Universal Time_ (UTC) standard, and in my local time zone that is **5:45AM**, then you may have a different opinion. If I told you about some event that happened on “10/11/12”, you could assume I meant October 11th, 2012 (if you’re in America), or November 12th, 2010 (if you’re in China, Korea, or Japan), or November 10th, 2012 (if you’re in most of the rest of the world). Facts that are actually _factual_ require accurate parsing[^1].

Thirdly, data can (and often are) selectively represented in such a way to suit the agenda of the person presenting those data. There are a whole host of tricks marketers can use to represent technically accurate information in completely misleading ways. One such example is the aptly named _“lie factor”_. See [this Wikipedia Article](https://en.wikipedia.org/wiki/Misleading_graph) for tons of great examples I'm too lazy to reproduce here.

# Data Types

Data can refer to many different things, and come in many different forms. I am working on another article about information encoding and data parsing, but for now it’s enough to say that some data are simple, some are less so.

Just like there is no universally agreed to definition of what all it means to be ‘fit’, there isn’t a global, all-encompassing definition set of what _types_ of data exist. Different programming languages (or Database technologies) contain different sets of data types. Here are some of the more common ones.

## Booleans

Boolean data are either true or false. Zero or one. Yes or no.[^2]

Wholly contained set of examples:
- true
- false

The end.

## Integers

Integers are numbers without decimals. This is the meaning of the word “integer” mathematically, and it happens to be the meaning of the word in dataspeak, too. Integers in computers are typically limited to being small-to-large numbers. Once you get into huge-number territory, integers may not be possible.

Examples:

- 1
- -4
- 7472

## Floating Point Numbers

Floating point numbers are numbers that allow for decimals and really huge numbers. If we were to use math terms, this would include all rational and irrational numbers. These are separate from integers because of how they are represented in binary and thus how the computer stores them and processes them. Floating points numbers may be stored as approximations of the numbers they really represent. There is no closed-form way to store **_π_**, for example. But numbers don’t need to be irrational to be stored as approximations in the computer. For an example of the effects of this approximation, see [this Google result](https://www.google.com/search?q=399999999999999-399999999999998&client=safari&hl=en-us&sxsrf=ALiCzsaE_A3N12davQeN_6X1_F_OJojfJQ%3A1658342636393&ei=7EzYYpbGF5KuptQPxJa_6Aw&ved=0ahUKEwiW7Ifej4j5AhUSl4kEHUTLD80Q4dUDCA0&uact=5&oq=399999999999999-399999999999998&gs_lcp=Cgdnd3Mtd2l6EAM6BwgAEEcQsAM6BwgjEOoCECdKBAhBGABKBAhGGABQmSFYmSFghipoBHAAeACAAWqIAWqSAQMwLjGYAQCgAQGgAQKwAQrIAQjAAQE&sclient=gws-wiz).

Examples:

- 1.5
- 3.14159265358979323846264338
- 399,999,999,999,999

## Strings

“Strings” are just text. They call them “strings” because some languages (such as “C++”) don’t natively let you work with text. Instead you have to work with individual **characters…** that gave rise to the need for libraries of code that helped you ‘string together’ those characters and work with the resulting text. The name stuck. Modern programming languages have native support for strings.

Examples:

- Hello, world!
- How much would could a woodchuck chuck if a woodchuck could chuck wood?

## Dates & Times

Not every language contains constructs for dates and times. Many databases force you to just handle your own encoding and decoding of dates & times. However, they’re so common in application development and record keeping that they’re a standard feature of any modern programming language. Depending on the language, you may also have support for _durations_.

Examples:

- 2022-07-20
- 1955-04-24

## Enumerations (or “Enums”)

Enumerations are a good concept that should be more well known by normies. An enumeration is just a thing that has a certain, finite, pre-determined set of values it can have. You have to be able to _[enumerate](https://www.google.com/search?q=enumerate&ie=UTF-8&oe=UTF-8&hl=en-us&client=safari)_ those values. This lets you maintain control over inputs and define behaviors on a case-by-case basis more easily.

Examples:

- Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday
- ⭐️, ⭐️⭐️, ⭐️⭐️⭐️, ⭐️⭐️⭐️⭐️, ⭐️⭐️⭐️⭐️⭐️

## Objects

The last type of data is a catch-all for “anything more complex”. Some of the data types I’ve listed above are actually _objects_ behind the scenes. Objects can hold arbitrary amounts of data of whatever format you like. They are an incredibly powerful concept and thus are the basis of what many coding languages were developed around. You can’t really represent an object without resorting to some sort of conventional notation. Arguably the most widely-used notion is the JavaScript Object Notation (aka “JSON”).

Example:

```
{
	"name" : "Aaron Gillespie",
	"website" : "https://www.aarongilly.com",
	"owned_vehicle" : {
								"make" : "Ford",
								"model" : "Escape",
							},
	"languages_spoken" : ["English", "TypeScript"]
	"sibling_count" : 2,
	"writer" : true
}
```

# Digital and Analog Data

## Digital Data

See [my previous article](https://aarongilly.com/gillespedia/analog-vs-digital/) on the difference between analog and digital. All digital data can be thought of as a long long long string of zeroes and ones. Doesn’t matter if you’re looking at a picture, listening to a song, reading an email, or crunching numbers in Excel - if you’re doing it on a computer, you’re interacting with ones and zeroes.

We have special names for different quantities of zeros and ones:

![a table of zeros and ones](https://lh3.googleusercontent.com/pw/AM-JKLV5jkihBxr4Wgtoc7xyfJvfrCGf_PL3D0uQT5eTS1hswW7pbJI1ckoY2LXtTjEgSahY9PdIY5Jk6VD2WWF9oIIPpTDsvPrEE6C2y2jqWaOeotHGptkM0Bj8d1md7ttPsdPzLljtj9uiyCtxTjJIo9zKYA=w600)

There are a number of ways in which you can turn zeroes and ones into meaningful information. The translation of data into information is dependent on _context_ and _convention_.

Let’s consider the sequence “`01010101`”.

- A human would look at that number and say it’s **`one million ten thousand one hundred one`**, and perhaps comment on the strange leading zero
- A computer or binary-knowing human would say it’s that, or it could be the number **`85`**
- A computer, given the context it’s an ASCII character, would use the ASCII convention to say it’s the character `U`
- A computer, given the context it’s a tiny floating point number, would use a floating-point convention to say it’s the number **`832`**
- A human without glasses on might say it’s the letters `OlOlOlOl`

There are numerous other possible meanings of `01010101`, I’m not smart enough to look up what operations it might mean in machine code or other such possible interpretations.

Turning data into information is the process called “**parsing**”. I plan to write another post about data parsing in the future. Maybe I’ll remember to update this paragraph to include a link to it.

## Analog Data

This section included mostly for completeness. Not all data are digital. You can just write things out. A vinyl record is a form of fully analog data. A poloroid photograph is a purely analog form of data.

My favorite example of analog data I can’t find a picture of - when a wall has a small light or something jutting out the side of it and it rains you can interpret the direction of the rainfall from the dry streak under the wall protrusion. Something about that is really satisfying to me.

Pure analog data are less common than analog stores of digital data. You could probably just forget you read this bottom section and be just fine.

[^1]: Technically this isn’t fully true. You could get lucky with your incorrect parsing algorithm and still wind up with accurate facts. If you parse the date text “10/10/10” then it doesn’t matter what country you’re in, it’s October 10th, 2010. [↩](https://aarongilly.com/gillespedia/data-basics/#fnref:1)
    
[^2] In some cases Booleans include a 3rd “neither yes nor no” state, such as NULL. I prefer the use of Enums for that. [↩](https://aarongilly.com/gillespedia/data-basics/#fnref:2)