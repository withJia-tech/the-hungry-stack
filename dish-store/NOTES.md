# dish-store — Hibernate

## The metaphor
Hibernate is the **recipe book that talks to the fridge**. You describe what a dish looks like (name, origin, borrowed-by). Hibernate handles actually putting it in the database and getting it back out. You never write SQL. You just say "save this dish" and it figures out the table.

## The exercise — CRUD as a kitchen verb

Create a `Dish` class. It has:
- a `name` (e.g. `"laksa"`)
- a `language_of_origin` (e.g. `"contested"`)
- a `borrowed_by` list (e.g. `["Singaporean English", "Australian English"]`)

Then do these four things, in order:

1. **Cook** — `save(dish)` → put it in the fridge
2. **Reheat** — `findById(1)` → take it back out
3. **Re-season** — change the name, save again → leftovers, edited
4. **Throw out** — `delete(dish)` → empty plate

That's CRUD: **C**reate, **R**ead, **U**pdate, **D**elete. Four operations. The whole point of a database, experienced as cooking, saving, reheating, and throwing out leftovers.

## The lesson
You never wrote a single line of SQL. Hibernate looked at your `Dish` class and worked out the table for you. That's the magic — and it's also the trap. Later you'll want to know what SQL it actually ran, and you'll learn to read the logs.

## You'll know it works when
You can run the program twice. The second time, the dish you saved last time is still there.

## Reflection (fill in after)
What surprised me:
What confused me:
What I want to try next:
