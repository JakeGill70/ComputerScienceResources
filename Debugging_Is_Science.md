# Debugging Is Science

---

> **Stop trying to make it pass. Try to find out why it fails.**

Debugging is the scientific method applied to code. You form a hypothesis about what's wrong, change one variable at a time, and design experiments that could prove you wrong. Your program is the system you're studying, every run is an experiment, and every bug is a place where your understanding of the program doesn't match what it actually does.

## Patching vs. Predicting

**Patching** is adding code until the problem seems to go away: another if-statement, another special case, another helper function. Each patch feels like progress, but it only treats a symptom. The code gets harder to read, the real bug gets harder to find, and the cycle repeats.

**Predicting** is knowing what your code *should* do before you run it, then using the result to test that expectation. When the prediction is wrong, you've found exactly where your understanding breaks down, and that's where the bug is.

> **More code is rarely the fix.**

## When in Doubt, Sketch It Out!

Before writing code, draw the problem on paper or a whiteboard. Trace how your data changes, step by step: the values in your variables, the contents of an array, or the connections between objects. If you can't sketch what your code should do, you aren't ready to write it yet. Experienced programmers sketch too, especially when a problem is new to them.

## The Predict–Observe–Explain Loop

If you can't say what you expect, you aren't testing anything. You're writing code without writing programs. You're a parrot repeating strange noises in hopes of a cracker.

1. **Predict:** Before you run your code, write down what you expect to happen.
2. **Observe:** Run the code and compare the actual result to your prediction.
3. **Explain:** If they differ, figure out *why* before changing anything.

> **No run without a prediction.** 

## Good Debugging Habits

- **One change at a time.** If you change three things at once, you won't know which one mattered.
- **State each fix as a hypothesis.** *"I think the bug is ___ because ___. If I'm right, changing ___ will make ___ happen."* If you can't complete that sentence, don't make the change.
- **Predict in the debugger too.** Before stepping over a line, predict the new values of your variables. The first value that surprises you is likely to be your bug.
- **A wrong prediction is progress.** "I thought it would do X, but it did Y" isn't a failure. It shows you exactly where your understanding is off.

## Check Yourself

Every so often, ask yourself:

> **What have I changed in the last 10 minutes, and what did I expect it to do?**

If the answer is "I added another if-statement, and I'm not sure," you're patching. Put the keyboard down and pick up a sheet of paper.

> **Are you still cooking, or are you getting cooked?**

If a problem is taking much longer than it should, something has probably gone wrong. Ask for help from an instructor, a tutor, or a classmate, and bring your sketches.
