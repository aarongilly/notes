---
tags:
  - modeling
  - data
  - business
summary: Tooling. Conditionals. Logical Operators. Arrow Relations.
---
**`= this.summary`** 

[[IDEF0]]'s big killer feature is its simplicity... but *sometimes* it's possible to create complexity in the name of "keeping it simple".

## Tooling
The lack of good [[IDEF0 Tools]] sucks. IDEF0 was designed to work with pen & paper, but paper is easily outmoded by digital methods that enforce [[Referential Integrity]] and allow for hyperlinks via [[URI]]s to drill into. You *could* represent everything there is to say in an IDEF0 model in a relatively simple [[OPM|OPL]]-like language. This would be useful and is easily technically possible... but ([almost](https://github.com/jimmyjazz/IDEF0-SVG/tree/master/lib/idef0)) no tools exist for this.

## Conditionals
Conditional statements are *probably* why IDEF0 claims itself to be a "functional" modeling language and *not* a "process" modeling language. They are, however, ridiculously common. People **will** break conventions to insert conditionals. 

I think that conditionals are also where you start to get "too much rope" and hang yourself with model [[System Complexity|complexity]].

## Logical Operators
When one function box has outputs that go to multiple "next" function blocks, there's no mechanism in place to say if the function completion "activates" both, either, or exactly one of the next functions. To me this is a massive gap in [[IDEF0]] in the service of functional modeling. This, too, is perhaps more "process" than "function" - but I'd argue IDEF0 as a language is harmed by the lack of "&"/"or".

Note: these **are** featured in [[IDEF3]].

## Arrow Relations 
This is where you really start to get into the weeds, but it would be nice to be able to relate or expand upon the relationship between the arrows themselves. If an arrow forks into multiple arrows, this implies a "Composed of" relationship (or something like it), but it would be nice to have and affordance for specifying the relations between the arrows. 

I can't imagine this being done *within* the IDEF0 diagram framework, but it would be a good (/necessary) thing to do in a full system model using [[IDEF]]. This is probably what [[IDEF3]] is meant to cover.

## Small Example
Small example I whipped up to illustrate some deficiencies.
![[What's Missing from IDEF0 2023-12-08 10.13.31.excalidraw|800px]]
### Example Issues:
1. Tooling didn't force me to put function numbers in my boxes, or tunnel the recipe/ingredients
2. What does "Food choice" entail? Is that a digital dataset? 
3. Are the Sous Chef and Chef *necessarily* different people?
4. The output of "Get ingredients" is split by whether or not the ingredients for the recipe chosen are available, but that important and simple distinction is hidden due to a lack of a mechanism for conditionals
---
### Source
- Personal usage & analysis of others
- [This dude's IDEF0 tool](https://github.com/jimmyjazz/IDEF0-SVG/tree/master/lib/idef0)

### Related
- [[IDEF0]]
- [[IDEF0 Tools]]
- [[IDEF]]
- [[IDEF3]]
- [[More is Unnecessary, Less is Impossible.|Perfect Tool]]