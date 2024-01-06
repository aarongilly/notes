---
tags:
- modeling
---
**Different ways in which things can be related.**

Things exist (citation needed). 

Things are either entities (’objects’) or behaviors (’processes’). Things can relate to one another. Things can relate to one-another in infinitely many ways. However there are multiple takes on categorizing and enumerating the ways in which things can relate to one-another, particularly in the realm of [[MBSE]]. Here are some categories that have been used in [[SysML]], [[OPM]], and [[IDEF]]  to bucket the way things can relate.

Note: OPM contains a graphical representation “OPD”, and a textual one “OPL”

# Relationship Categories

## Composition:  A —composed of→ B

An object is made up of smaller objects. Or a a process is made up of smaller processes. 

| In | Validity | Related Properties |
| --- | --- | --- |
| SysML
OPM
IDEF | Object-to-Object
Process-to-Process | Source & Destination Multiplicity |

**Representation:**

OPD/OPL

![Untitled](Untitled%2068.png)

SysML

![Untitled](Untitled%2069.png)

IDEF

![Untitled](Untitled%2070.png)

## Exhibition: A —exhibits property→ B

An object has an attribute. A process has an attribute. 

| In | Validity | Related Properties |
| --- | --- | --- |
| SysML
OPM | Any-to-Any | Unit |

**Representation:**

OPD/OPL

![Untitled](Untitled%2071.png)

SysML

![Untitled](Untitled%2072.png)

No graphical notation, instead properties are included

## Generalization: A —is a→ B

An thing is a more specific version of another thing.

| In | Validity | Related Properties |
| --- | --- | --- |
| SysML
OPM
IDEF | Object-to-Object
Process-to-Process |  |

**Representation:**

OPD/OPL

![Untitled](Untitled%2073.png)

SysML

![Untitled](Untitled%2074.png)

IDEF

![Untitled](Untitled%2075.png)

## Aggregation: A —is a group of→ B

Aggregation is a weaker form of Composition. Composition typically means that the child instance cannot be child to multiple parents via a composite relationship, but it can be a part of multiple parent class instances via an aggregation relationship.

An engine is only in 1 car. It is a composition.

A basketball player may play on several teams, so that relationship would be an aggregation. 

I've also seen aggregation disambiguated from composition by saying that when the parent class insurance is destroyed, a composition-linked child would also be destroyed, whereas an aggregation-linked child would not be destroyed. 

## Instantiation: A —is an instance of→ B

An thing is an individual instance of a kind of thing.

| In | Validity | Related Properties |
| --- | --- | --- |
| SysML
OPM
IDEF | Object-to-Object
Process-to-Process |  |

**Representation:**

OPD/OPL

![Untitled](Untitled%2076.png)

SysML

![Untitled](Untitled%2077.png)

No graphical link notation, instead instances are labeled with the Blocks they instantiate.

IDEF

![Untitled](Untitled%2078.png)

## Agency: A —handles→ B

An agent of some kind executes the activity B.

| In | Validity | Related Properties |
| --- | --- | ---

## Source
- [[SysML Distilled]]
- [[Wikipedia]] |
| SysML
OPM | Object-to-Process |  |

**Representation:**

OPD/OPL

![Untitled](Untitled%2079.png)

SysML

There isn't just 1 way to denote this is SysML. Nor UML.

## Yields: A —yields→ B

A process of some kind results in B

...

## Triggers: A —triggers→ B

An event of some kind triggers a process.

In [[UML]] AND [[OPM]]. Also maybe [[SysML]] in [[Activity Diagrams]]?

...

## Supports: A —supports→ B

An object or agent supports a process, but is not modified by it. Instruments in OPM. Mechanisms in IDEF.

...

## Constrains: A —constrains→ B

A characteristic of a thing (or a requirement) constrains another characteristic of a thing (possibly the same thing, possibly different).

# Other Sources

[Use case diagram - Wikipedia](https://en.wikipedia.org/wiki/Use_case_diagram#/media/File:Use_case_restaurant_model.svg)

### Related Notes
- [[OPM]] 
- [[SysML]] 
- [[IDEF]] 
- [[UML]]