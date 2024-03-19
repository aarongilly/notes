---
created: 2023-07-08
tags:
  - coding
aliases:
---
`Pkl` is a new programming language for writing **configuration** files. The language outputs to [[JSON]], [[YAML]], [[XML]], and other common formats used for configuration files. It builds on the typical experience (doing it by hand) through the inclusion of [[Intellisense]], loops and classes, Type Safety, and the ability to impose constraints on values... and the constraints syntax and capabilities both look like they rule.

Example Pkl code:

```plaintext
email: String = "example@example.com"
port: Int(this > 1000) = 90
```

Here `port` would throw an error for not fitting to its constraint.

****
### Source
- [https://pkl-lang.org](https://pkl-lang.org/)

### Related
- [[JSON]]
- [[YAML]]
- [[XML]]