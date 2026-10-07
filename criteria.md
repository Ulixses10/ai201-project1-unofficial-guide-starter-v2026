# Acceptance criteria — The Unofficial Guide

Five criteria that say what "working" means for this system, written in unit 1
**before** any results existed.

An acceptance criterion names a target: a number, a count, a rate, or something
a person could plainly observe. *"Retrieval works"* is an opinion. *"For at
least 4 of my 5 test questions, the top results include a chunk containing the
answer"* is a criterion.

Under each one, write a sentence or two on **why that target** and not a
stricter or looser one. A reason that says something about your corpus or your
pipeline earns credit; *"80% seemed reasonable"* does not.

> Missing your own targets next unit costs you nothing. Setting a target so
> easy you can't miss it does.

---

## 1. Retrieved chunks contain the answer

For at least 4 of my 5 test questions, the retrieved chunks include one that
contains the answer.

**Why this target:**
I expect question 5 to be the hardest out of the 5 since when it comes to extending your deadline there is many different factors from asking permission before the deadline or simply not asking for permission and also sickness excuse. There is many different factors here so the system may respond incorrectly 

---

## 2. Every answer names a source

Every answer the system produces names at least one source document.

**Why this target:**
my setup makes this achievable because all the information in the questions are coming directly from the threads document which contain the thread question and the replies. This allows the system to answer the question since the documents provide the information and in the addition this system document are all lable for example thread_bike_commute.txt which allows the app  to identify which document it was used for.
 

---

## 3. The relevance gate stops out-of-corpus questions

When I ask a question my documents clearly don't cover, the relevance gate
stops it and the system returns "I don't have enough information about that" —
in at least 4 of 5 tries.


The five questions are the ones in `OUT_OF_SCOPE` at the bottom of
     `questions.py`, and `run_eval.py` puts them through the gate and writes
     what happened into your run log. Swap them for your own if you'd rather —
     just keep five of them, or the "4 of 5" above has nothing to be 4 of.

**Why this target:**
What did your distances look like when you set the cutoff in Milestone 4?
     Was there a clean gap, or did the two groups overlap? 
     Answer: The distance of the out of scope question was a big difference compared to the 5 question that was in scope and it would always go above the cut off which the cut off distance was 0.7. For example the out of scope ranged from 0.8077 to 0.8966.
     

---

## 4. Something about your chunks

YOU WRITE THIS ONE.
     When i'm inspecting the 5 chunks I would expect atleast 4 should contain an idea that can help answer the question about the thread. If the starting chunk contains a small amount of character chunks such as 200 characters or below I can expect atleast 1 of the 5 chunks to not answer the question correctly. 
     
     
     



**Why this target:**



---

## 5. Your choice

YOU WRITE THIS ONE TOO.

     I care about how accurate something is and how close I can get something to perfection. For example within this project I would want my system to understand atleast 4 out of 5 questions and correctly print out the expected response. I know there can be some errors here and there, but I would hope for the system to get it close to right. 



**Why this target:**



---

<!-- ─────────────────────────────────────────────────────────────────────────
     UNIT 2 — read this before you change anything above.

     If a criterion turns out to be BROKEN rather than merely unmet, you can
     revise it, and that earns credit. But never delete or edit the original
     line. Add the revision underneath it, like this:

         ## 1. Retrieved chunks contain the answer

         For at least 4 of my 5 test questions, the retrieved chunks include
         one that contains the answer.

         **Why this target:** ...

         > **Revised in unit 2:** For at least 4 of 5 questions, the top three
         > results contain the answer.
         >
         > **Why revised:** I couldn't judge "the chunks include one that
         > contains the answer" the same way twice — I scored two questions
         > differently on Monday than on Wednesday. The new version is
         > something I can actually check.

     That's a revision because the criterion couldn't be MEASURED.

     Lowering a target because you missed it is not a revision, and it costs
     you the point:

         ✗ "I said 4 of 5 but got 2 of 5, so 2 of 5 is more realistic."

     A number you missed stays where it is, gets diagnosed, and gets a fix
     attempted. That's where the points are.

     The whole reason the originals stay visible is so someone can see what you
     said before you knew the answer.
     ───────────────────────────────────────────────────────────────────────── -->
