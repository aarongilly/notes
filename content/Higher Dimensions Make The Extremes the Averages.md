---
created: 2023-08-23T21:59-05:00
updated: 2023-08-24T08:49-05:00
---
**As you go up in number of factors considered in problem solving, it becomes increasingly likely that the optimal approach will haveat least one of them will be at an extreme.*

It's just math and probability. If you have dimensions of trade space, as you add more dimensions the "optimal" solution becomes increasingly likely to be at an extreme of one or more dimensions. 

## Discrete Dimension Example
Assuming the "optimal" approach is a random point...

XOOOOOOOOX <- 20% chance it's at the extreme 10% end of a 1D situation.

XXXXXXXXXX
XOOOOOOOOX
XOOOOOOOOX
XOOOOOOOOX
XOOOOOOOOX
XOOOOOOOOX
XOOOOOOOOX
XOOOOOOOOX
XOOOOOOOOX
XXXXXXXXXX <- 36% chance it's at at least one extreme of a 2D situation. 

For 3D, it's 100+100+ 36*(8)/1000 = 48.8%

4D would continue this trend. 
{a,b,c,d} => 1 - 0.8^4 = 59%

---
### Source
- [[Ultralearning]]

### Related
- [[Lies, Damn Lies, and Statistics]]

#### Tags
#math 