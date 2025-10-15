# Exercise 1: Minecraft calculator!

There are two goals of this assignment (in order of priority):
- learning how to read,
- kickstart getting into the flow of programming.

Being a good programmer *heavily* involves good language skills, a lot more than people think. Even more than that,
programming requires so much more reading than writing. Practicing reading skills is the fastest way of getting gud AND
the easiest way to stand out from other programmers. So we're going to focus on that in the beginning.

## The Situation

You're doing a build, and the video you're following gives you a list of materials you need. You want to know how much
corresponding raw material to gather to get as close as possible.

You need the following:
- 1200 planks
- 768 stairs
- 46 gold blocks
- 15 bookshelves

### The Meta-Situation

(this exercise will involve a lot of hand-holding. The point here is to introduce skills one at a time. This won't be the
case soon, though! You'll start taking initiative in these exercises and have less and less hand-holding. For now,
though, the next section is here to help)

## The Process

Your end goal: how much of the base raw materials do you need to make ^? Let's ask a few questions to get there:

1. What _are_ the materials we need for each of these?
    - ? > planks
    - ? > ? > stairs
    - ? > ? > gold blocks
    - ? > ? AND ? > bookshelves

2. What are the rate of each conversion? In other words, how much of each do we need to make the next? (one at a time!)
    - Stairs:
        - \# ? > # ? (we need this number of ? to make this number of ?)
        - \# ? > # stairs (we need this number of ? to make this number of stairs)
    - ...
    - Bookshelves:
        - \# ? > # ? (we need this number of ? to make this number of ?)
        - \# ? AND # ? > # bookshelves (we need this number of ? AND this number of ? to make this number of bookshelves)

3. Some of these materials are overlapping right? Would it make sense to do this one at a time, as in figure out how
   much of a material for each recipe first, before combining the amounts for the overlapping ones?


You should have everything we need to calculate this, so let's write a Python program that does just that. Open up
`exercise_1.py`. Read it through once on your own.

Remember, reading is important, so now let's practice that:

4. What's going on already in this file? There are 18 lines, could you explain EACH line and their purpose?

5. Some of these are organized into groups. What's the grouping pattern? What does putting them like this accomplish,
   versus just putting them all together?

6. Notice how some of the variables are named with just "material" in them (`material_for...` or `...for_material`).
   These are _kind of_ descriptive names, but we can do better, right? (some of them are even the same name, which we
   don't want to do!) How could we do better/improve, and why is that actually an improvement?


Alright, now we have a good understanding of the file, without even writing a single character. *Now*, we can now start writing.

- Go ahead and start with adding your name as an author. I don't want all the credit for your assignment!
- Next, do the change you talked about in the above question/response.
- Let's focus on the first grouping. Can you calculate the amount of the raw material needed to make that many
  planks? (note, we don't want just the final number here, we want Python to do that calculation for us, it should look
  like a formula)
  - But how are we supposed to know what the actual amount is? Can you write something to print out the value somehow?
- This is a good stopping place to make sure our changes so far are working as expected. It's good principle to make
  *incremental* changes, testing at each step, instead of writing a whole bunch of stuff, testing, and finding out we
  messed up hours ago. Go ahead and run the Python file.
  - !!!!!
  - We never learned that??
  - That's okay, there's a few ways of doing it, and we'll use multiple ways throughout this course. For now, ask your
    professor (me) to show you how it's done _for this exercise_. Or, if you already know, take a stab at it yourself!

7. Did it work? Can you double check on your own calculator and make sure it's the same number?

Why did we have to plug it into a calculator too? It's *very* important to always check your work. Not just here, in
*all* programming. Writing code and not validating it is exactly the same as sitting a monkey at a typewriter, asking
them to write a book, and expecting Shakespeare. So don't do that.

- Now, go ahead and work on the second grouping! Same thing, these should be formulas. Add something else at the end to
  print out the final value.
- Do the same thing for the other two groupings.

We're done!(?) Not yet. Let's talk about question 3 again. There's a few raw materials that are the same. Our end goal
is how much of the raw materials to make *everything*.

- Combine the amounts for the ones that are the same material into new variables. Print out the total amounts now.

The last thing is related to that readability aspect, specifically adding comments to our code to explain what's going
on. In Python, what you write becomes a comment when you start it with a `#`.

- Go ahead and add some. Use what you feel is an appropriate amount, there's a balance between having too many comments
  and not enough.
