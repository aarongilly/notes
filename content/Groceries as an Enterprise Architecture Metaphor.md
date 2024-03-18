---
created: 2024-03-16
created:
tags:
  - business
aliases:
---
[[Enterprise Architecture]] is a vague and abstract thing. Walking through Dillons I came up with the following:

Your business not having an articulated Enterprise Architecture is like going to the grocery store without a meal plan, without knowing what's already in your pantry, and in the worst of cases not even knowing what equipment your kitchen has. 

Sure, *you might be able to stumble your way through* to groceries that result in meals for the week, but you will:
- spend more money than you needed to
- end up with more wasted ingredients - buying stuff you don't actually need or more of what you already have
- have a less lean fridge & pantry, which will make it hard for your spouse to even know what the ingredients are for
- end up with a weird and incoherent meal plan for the week
- might buy ingredients you don't even have the equipment to cook

It takes time to take stock of your kitchen and think about the kinds of foods you want to make, but this up-front investment will result a better utilization of resources at the store and less frustration throughout the week.
### [[Enterprise Architectural Layers]] in the metaphor
Maybe this works.
- **Business Layer** - the Meal Plan, it's what you're trying to *do*, ultimately
	- Example: Bake a cake
- **Data Layer** - the list of what's in your pantry and the list of what your recipes call for
	- Example: 
		- Inventory - flour, sugar, eggs
		- Recipe - butter, milk, eggs, sugar, flour
- **Application Layer** - is what you can do with the equipment in your kitchen
	- Example: 
		- Mixing
- **Technology Layer** - is *how* you can do those things
	- Example:
		- Hobart Mix-o-Tron 5000
		- A handheld mixer and a bowl
		- Bowls and whisks for hand-mixing
### Scaling Up the Kitchen
Thinking of the layers that way might help in understanding **what** they are, but doesn't make it clear **why** they are a good thing - for that you have to scale up the kitchen. 
A real business is much bigger than your kitchen[^1]. Imagine your kitchen is actually a world-class restaurant with dozens of chefs, cooks, waiters, and a manager. They have to communicate effectively and continually to keep the customers happy. You have multiple pieces of technology over overlapping capabilities. You make make multiple orders with grocers per week. If an oven goes down, you might have a grilltop that *also* has oven capabilities you could utilize for the day.  

Your job is to utilize your budget to improve the restaurant. Do you buy better ingredients? Do you upgrade the equipment? Do you expand the menu to offer new dishes? Do you hire more people? 

Can you buy back more resources (money, space, etc) by consolidating certain capabilities? You could stop making your own bread dough in house. This is the only thing the Mix-o-tron 5000 was for. So you can sell that, get some money, no longer have to maintain it, and regain counter space to be used for other more valuable technologies delivering more utilized capabilities. Perhaps you've been toasting your bread in the regular oven, which is taking up valuable oven time. You could buy a toaster with the Mix-o-tron resources. 

If you ask any one of the members of the kitchen, they will give you the best answers from their perspective, but their perspective represents a limited view of the overall problem. Enterprise Architecture modeling creates a common asset around which discussions can be held. It can be used to model "to be" states. Once you replace the mix-o-tron with a toaster, what new capabilities open up?

[^1]: and if it's not, enterprise architecture is probably not something you need be concern too much with
****
### Source
- self
### Related
- 