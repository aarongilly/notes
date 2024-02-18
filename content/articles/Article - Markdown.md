---
created: 2020-09-13
tags:
  - notetaking
  - article
aliases:
---
Markdown is a text-based text styling language. In layman’s terms, it is a couple of additional characters you put in your writing that the computer uses to change how it looks. It allows you to do things like **bold**, _italicize_, and [hyperlink](https://en.wikipedia.org/wiki/Hyperlink) your text without taking your hands off the keyboard.

# Some History

Markdown was first codified into a standard in 2006 by a guy named John Gruber, whom I know nothing about, in collaboration with a guy named Aaron Swartz, whom I know enough about to say he died way too early and contributed more to the world of technology than I’ll ever accomplish.

# Why is it Popular?

Turns out people are both lazy and expressive. We want the ability to write with _some_ level of nuance, but developers don’t necessarily want to go through the trouble of building full richtext editors, complete with buttons and menus that allow you to make things **bold** or make hyperlinks. Also such richtext editors expand the size of a webpage that your computer needs to download, interpret, and display. Even if the size is miniscule, there’s no reason to take that hit when you’ve got an easy option that more and more people are learning.

More than that, Markdown serves a purpose of creating a simple text formatting language that can be interpreted by a large number of clients in different environments. If you export your Microsoft Word files and then try to open them with other applications, you’ll find that there aren’t a _ton_ of available options for you. Moreover, all the available options will come with some sort of interpretation errors. The core Markdown syntax notation is entirely portable, meaning you can copy your stylized text from one place and put it in another, and it will _probably_ look like what you’d expect. Better yet, Markdown was designed to be human-readable. So, even if you look at **plain text Markdown** you’ll not only be able to _read_ it, you’ll probably be able to read it almost as effectively as you would if it were stylized.

```
# Avengers Movies

Marvel’s "The Avengers" came out in 2012 and changed the landscape of cinema. It combined heroes from **five** different movies that came before it into one super team. At the time it seemed like an impossible feat - but they’d go on to not only *repeat* that success, but to **blow it out of the water**.

## Avengers at the Box Office

Box office numbers don’t lie; The Avengers are **huge**:
- Marvel’s The Avengers made $1.529B
- Avengers: Age of Ultron made $1.403B
- Captain America: Civil War made $1.153B
  - This definitely counts
- Avengers: Infinity War made $2.048B
- Avengers: Endgame made **$2.798B** and is currently the highest-grossing movie of all time

source: [Google](https://www.google.com/search?q=avengers+movies+box+office)
```

Compare that to html…

```
<h1 id="avengers-movies">Avengers Movies</h1>
<p>Marvel’s "The Avengers" came out in 2012 and changed the landscape of cinema. It combined heroes from <strong>five</strong> different movies that came before it into one super team. At the time it seemed like an impossible feat - but they’d go on to not only <em>repeat</em> that success, but to <strong>blow it out of the water</strong>.</p>
<h2 id="avengers-at-the-box-office">Avengers at the Box Office</h2>
<p>Box office numbers don’t lie; The Avengers are <strong>huge</strong>:</p>
<ul>
<li>Marvel’s The Avengers made $1.529B</li>
<li>Avengers: Age of Ultron made $1.403B</li>
<li>Captain America: Civil War made $1.153B<ul>
<li>This definitely counts</li>
</ul>
</li>
<li>Avengers: Infinity War made $2.048B</li>
<li>Avengers: Endgame made <strong>$2.798B</strong> and is currently the highest-grossing movie of all time</li>
</ul>
<p>source: <a href="https://www.google.com/search?q=avengers+movies+box+office">Google</a></p>

```

# Where can you use it?

The beauty of Markdown is that it _can_ be used **anywhere**. You can open notepad on your Windows computer and type out a note using Markdown syntax. You’ll be able to read it easily as you’re writing it. Markdown files typically end with “.md” (as opposed to “.txt”), but really it doesn’t matter what your file extension is. You can copy and paste Markdown text into these platforms (and 1000s more, I’m sure):

- Reddit
- GitHub
- Notion
- Dropbox Paper
- Bear
- Roam
- Obsidian
- Most coding README files

All these services (and hundreds more) will turn ‘**this**’ into ‘**this**’.

# How do you Markdown?

## The 80% of Stuff You’ll Use Often

### Basic Styling

The whole idea of Markdown is that you’re not taking your hands off the keyboard.

_Italic_ - surround the text to be italicized with single asterisks.

```
This text is not italic, other than *these two* words.
```

**Bold** - surround the text to be bolded with double asterisks.

```
You can write like **this** if you're feeling **particularly bold**.
```

Block quote - start each line to included in the block quote with a greater-than sign. If you don’t know what a block quote is…

> A Block Quote looks like this.

```
I heard this awesome tip:
> Block quotes are a good way to make something stand out.
```

Unordered List - start each line to be included in the unordered list with a hyphen (or asterisk), then a space.

```
Things Dwight enjoys:
- Bears
- Beats
- Battlestar Gallactica
```

Ordered Lists - start each line to be included in the ordered list with a number… weirdly you can use _any_ number, and it will automatically render with proper order.

```
Steps for making a sandwich:
1. Get bread
2. Get ingredients
3. Text your mom for help
```

### Other Things

Hyperlinks - in order to link text, put the text you want to display inside square brackets, and follow them with the hyperlink in parenthesis.

```
This is a [pretty okay website I guess](https://aarongilly.com)
```

Inline images - not _every_ place you can use markdown will support inline images, but those that do will use the same syntax as hyperlinks, but with an exclamation point in front.

```
This is a picture of a dog:
![this text will load if the link is broken](https://images.unsplash.com/photo-1561037404-61cd46aa615b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2700&q=80)
```

To do lists - this is also not accepted _everywhere_, but places like GitHub and Notion will recognize any line starting with an open and close square bracket as to-do items.

```
- [] this is an incomplete task
- [x] this is a completed task
```

## The 20% of Stuff You Won’t

### Tables

These are the biggest pain in the neck for markdown. There’s simply no way to manually type a table that looks good to people reading plaintext. There are various methods of making table in Markdown - but none of them are all that satisfying.

### Text coloring

Native markdown has no support for text color changing.

### Underlining

Weirdly there is no support for underlining in the standard Markdown syntax. I suspect it’s because the syntax was written with the expectation that underlined text would be reserved for links. Frankly I’m okay without underlined text. It’s my least favorite _attention_ **grabbing** stylization.l

### Highlighting

In [[Obsidian]]-flavored Markdown, the syntax for ==highlighting== looks like this:

```
One word of this sentence is ==highlighted==, the rest aren't.
```

# Other Resources

- [The Official Markdown Guide](https://www.markdownguide.org/)