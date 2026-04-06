# notebooks — NotebookLM

## How this one is different
The other tools in this stack are code you run. NotebookLM is **Google's AI that reads documents and lets you interrogate them**. It is a research layer that feeds your data curation. You don't write code here — you write questions, and you check the answers.

## The exercise

1. Open NotebookLM. Create a new notebook.
2. Upload the Wikipedia article for **"Laksa"** as a source. (You can also upload your own `data/dishes.json`, or a cookbook PDF.)
3. Ask it: *"Which languages does the word 'laksa' appear in, and what are the competing origin theories?"*
4. Read the answer. Click through to the citations it gives.
5. Copy the parts that are actually grounded in the source into `research-notes.md`. That becomes the source material for your next round of `dishes.json`.

## The hygiene check — smart zone vs dumb zone

This is the part that matters more than the answer itself. **Every time you use an LLM, you have to know which parts of the answer to trust and which parts to throw out.**

Before you copy anything into `research-notes.md`, run this checklist on the model's answer:

### 1. Token efficiency
Look at the answer. Then look at the source you gave it. Roughly: **how much of what the model said is actually in the source?**

- If the answer is long but the source only supports a few sentences of it → the rest is the model padding. Throw the padding out.
- A short, dense answer that maps cleanly to citations is usually a better sign than a long, flowing one.

### 2. The smart zone (trust this)
- **Direct extraction:** "Laksa is mentioned in Hokkien, Peranakan Malay, and Persian." ← either it's in the doc or it isn't. Easy to verify.
- **Quoting with a citation you can click:** if NotebookLM hands you a number you can hover and see the source paragraph, that's the smart zone.
- **Listing things from a list that exists in the source.**

### 3. The dumb zone (don't trust this without checking)
- **Synthesis across sources** the model wasn't given. ("Combined with Tamil influences…") — where did Tamil come from? Was it in the source? If not, the model is making it up out of training data, and you have no way to verify it.
- **Confident dates, percentages, or "first recorded in…" claims** with no citation. Especially fabricated.
- **Causal stories** ("This is because traders in the 14th century…"). Plausible. Often wrong.
- **Anything that sounds like a Wikipedia summary but isn't actually from your uploaded Wikipedia.**

### 4. The reflection question
After you've copied the trustworthy parts into `research-notes.md`, ask yourself:

> *If I had read the source myself for 10 minutes, would I have gotten the same information faster, slower, or with more confidence?*

Write the honest answer in your reflection. This is how you build a feel for **when an LLM is actually saving you time and when it's just feeling productive**.

## You'll know it works when
Your `research-notes.md` only contains things you can point at in the original source. Nothing the model invented made it through.

## Reflection (fill in after)
Token efficiency (rough %): how much of the model's answer was load-bearing?
Smart-zone wins:
Dumb-zone catches:
Would I trust this method for the next dish?:
