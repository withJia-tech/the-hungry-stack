# the-hungry-stack

A learning log. One tool a day, one folder a day, one tiny exercise that fits in a primary school brain. The dishes in `data/dishes.json` are the ingredients — each tool is a different way of moving them around a kitchen.

The point is not to build a restaurant. The point is to understand the stack so well that you could reinvent the recipes with it.

## The exercises

Each one is small enough to finish before lunch/recess time. :) Hopefully. You can time yourself.

**Spring Boot — `menu-api/`**
Build a `/menu` endpoint. Hit it in your browser, it returns the 5 dishes from `data/dishes.json` as JSON. That's it. _Your first API._

**Redis — `daily-special/`**
Store today's "dish of the day" in Redis. Retrieve it. Change it. Watch it disappear when it expires. _Expiry is the lesson._

**RabbitMQ — `order-queue/`**
One service shouts an order ("laksa, table 4"). Another service listens and prints "order received." Two _separate_ programs _talking through a queue_. Echoing the instruction. 

**Cucumber — `kitchen-tests/`**
Write a test in plain English: "Given the menu exists, when I ask for laksa, then I should get a price." Then make it _pass._ If you want to up the difficulty level, write a test where the different variations exist e.g. with or without curry leaves, with or without sea hums. 

**Docker**
Put your Spring Boot menu API in a lunchbox. Run it on your machine without installing Java globally. The lunchbox contains everything.

**SonarQube**
Point it at your code. Read what it complains about. Fix one thing. That's the whole exercise.

**Guava**
Use its `Multimap` to store one dish mapped to multiple cuisines. Print it. Feel how much less code that was.

**Hibernate — `dish-store/`**
The recipe book that talks to the fridge. Describe a `Dish` (name, origin, borrowed-by). Tell Hibernate to save it, fetch it, change it, delete it. Four operations. CRUD as cooking, saving, reheating, and throwing out leftovers. You never write SQL.

**NotebookLM — `notebooks/`**
Different from the rest — not code, but Google's AI that reads documents and lets you interrogate them. Feed it a Wikipedia article on laksa, ask about origin theories, copy the trustworthy parts into `research-notes.md`. The exercise is also a hygiene check: every answer goes through a **smart zone vs dumb zone** review and a token-efficiency reflection. This is how you learn to feel when an LLM is actually saving you time and when it's just feeling productive.

## Rules

One folder gets a new file each day. The commit message is your one-sentence reflection on what you learned, not what you built.

## Learning log

| Day | Folder | What I learned |
|-----|--------|----------------|
|     |        |                |
