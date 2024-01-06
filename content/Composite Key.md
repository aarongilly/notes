---
tags:
- data
---
**A candidate key made up of multiple fields**

In [[Relational Databases]], a Composite Key (sometimes called "Compound Key") is a [[Candidate Key]] that is comprised of more than 1 attribute.

## Example

Given a table with fields:

- `student_id`
- `first_name`
- `last_name`
- `is_enrolled`

There are two sets of Candidate Keys.

1. `student_id`
2. `first_name`, `last_name`

Since the Candidate Key `student_id` is comprised of only one attribute, it is NOT a composite key. Also, because `student_id` is  

Since the Candidate Key `first_name`, `last_name` is comprised of more than one attribute, it is a Composite Key.

---

## Source

[Database normalization - Wikipedia](https://en.wikipedia.org/wiki/Database_normalization)

### Related Notes
- [[Candidate Key]] 
- [[Relational Databases]]