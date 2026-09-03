### Millefeuille
A working architecture for exploring what happens when new information changes the meaning of context a system already holds.

### What I’m trying to understand

Context is often described as though it accumulates.

Something happens. We add information. Then we add more.

But new information does not always sit neatly on top of what was already there.

Sometimes it changes the significance of an earlier piece.

Something that seemed irrelevant becomes important. Two pieces of context begin to contradict one another. An earlier interpretation stops making sense in quite the same way.

Millefeuille asks:

**How should a system represent context when new information can change the meaning of what came before?**

### The idea

Millefeuille treats context as layered, but not as a static stack.

Layers can accumulate.

They can also interact.

A new layer may bring an earlier one forward, push something else into the background, create a contradiction, or reorganize the meaning of what the system already held.

The technical question is how to represent enough of those relationships for a system to update without treating every new piece of information as equally important.

### Current status

**Architecture / pre build**

Right now I am working out the smallest version of the problem worth implementing.

I do not want to build an elaborate context architecture before I understand what behavior I actually need from it.

8-ish is already helping expose some of those questions in a smaller form.

It can store information and combine some context across turns.

It cannot yet tell whether new information should change the meaning of what it already holds.

That boundary is part of what Millefeuille will eventually explore more directly.

### First build

The first useful version should make a change in interpretation visible.

A system holds an initial piece of context.

New information arrives.

The system has to determine whether the new information:

- simply adds something
- changes the significance of something already present
- conflicts with what was previously held
- does not matter to the current decision

I am still working out how little machinery I can use to make that problem observable.

### Why Millefeuille

A millefeuille is made through layers, but the thing I care about is not simply that there are many of them.

The pastry is repeatedly turned, folded, and worked. Existing layers change their relationship to one another as the whole thing is made.

That is closer to the behavior I am interested in.

Context does not necessarily become richer just because there is more of it.

Sometimes what arrives next changes the shape of what was already there.
