---
created: 2023-07-08
aliases: 
tags:
  - coding
---
**Six good tips for coding with others**

1. **Finish your code before moving on.** Otherwise you’re going to have compounding technical debt.
2. **Enforce standards for formatting.** Use Linters. These expose low quality code faster and make rework much easier. [[Discipline = Freedom]].
3. **Document your patterns.** Use a [[Markdown]] file or a Wiki to document how you do things like access your database.
4. **Review new patterns early.** Publicize them to the team for feedback.
    
    e.g. - a new developer brings on their own access pattern to access a database, but doesn’t tell anyone about them using it. This pattern starts to show up around the code base, but it isn’t flexible enough to meet changing requirements.
    
5. **Never expose refactoring to customers.** That’s the developer’s job to handle. If the Customer is aware of it, they’ll try to control it. They’ll force you into bad situations.
6. Give yourself extra time for uncertainty. Give yourself extra time for documentation. Don’t fall prey to [[Unknown Unknowns]] and the [[Planning Fallacy]]. 

---

### Source
- [[How Senior Programers ACTUALLY write code]]

### Related
- [[Planning Fallacy]] 
- [[Markdown]] 
- [[Discipline = Freedom]] 
- [[Unknown Unknowns]]