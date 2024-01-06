---
tags:
- data
---
**Fields in a table that could be part of its key.**

In [[Relational Databases]], any field that could be a component of a [[Candidate Key]] is called a "**Prime Attribute**". If a field could not be a part of a candidate key, that's considered a "non-prime attribute". 

Illustrative Example:

Given a table had the following columns:

- person ID
- first name
- last name
- phone number
- email
- height
- weight
- age
- gender

You could feasibly see 4 sets of [[Candidate Key]]s like the following:

- A - person ID
    - an example of [[Surrogate Keys]], by convention forced to be unique (if otherwise meaningless)
- B - phone number
    - usually unique to the individual, but sometimes shared
- C - email address
    - usually unique to the individual, but sometimes shared
- D - first name + last name
    - naming collisions happen in large enough datasets

Thus, the Prime and non-Prime attributes are as follows:

- PRIME - person ID
- PRIME - first name
- PRIME - last name
- PRIME - phone number
- PRIME - email
- NON-PRIME - height
- NON-PRIME - weight
- NON-PRIME - age
- NON-PRIME - gender

---

## Source

[https://en.wikipedia.org/wiki/Candidate_key](https://en.wikipedia.org/wiki/Candidate_key)

### Related Notes
- [[Relational Databases]] 
- [[Candidate Key]]