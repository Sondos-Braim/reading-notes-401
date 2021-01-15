# Read 36
## Whiteboard interviews

Whiteboard-style interviews are ubiquitous in the tech industry. For those who not had the pleasure, whiteboard interviewing is the practice of asking candidates to solve technical questions on a whiteboard, piece of paper, or computer during the interview. This kind of environment can feel like a pressure cooker and cause even the most competent engineer to fall apart.


What Do You Mean Communicate?

Let’s say you are in the interview and your interviewers throw you a whiteboard question. Do you step up to the whiteboard and feverishly start solving the problem?





No!





That tends to be everyone’s instinct, but it’s definitely not the right way to go. Even if you think you understand the problem, you should take some very important steps before moving forward.





First, Restate the Question

Do you understand what they’re asking you to do? Prove it. Restate the question for them and seek affirmation. You might actually be surprised to find you don’t fully understand what they’re asking for — perhaps the question is similar, but not the same, as a practice problem you have completed in the past. Using the tried-and-true fizz-buzz example, you could restate the problem as follows:

1) Take a few minutes.

Speaking as an interview coach, this is one misstep that I see all the time during mock interviews. The canonical tip that everyone gives is, “talk more!”. What most of those well-meaning advice-givers overlook, however, is that talking and thinking at the same time is extremely hard. Nervous interviewees will jump straight into talking, passing up a great opportunity for concentrated thought.

Don’t waste precious minutes trying to fill the silence by saying everything you’re thinking, while simultaneously trying to solve the problem in your head.

Instead, wait until the interviewer is done explaining the problem. Ask any clarifying questions, and then tell your interviewer:

“Okay, got it. If it’s okay with you, I’m just going to take a minute or two here and think about the problem, and then I’ll start talking.”

Shut your eyes, stare at the ceiling, scribble on the whiteboard — whatever it takes. Think through the basics of the problem, and decide on an approach. Then re-engage the interviewer, and let him know what you’ve concluded. Don’t forget to provide your reasoning!

So, I think that, since the array is sorted, it makes the most sense to do something like a binary search here. Here are the general steps that I think are involved in the solution: …”

2) Write down the steps of the solution.

Even after you have an idea of how to attack the problem, don’t start writing code down. Write down the general steps of how you will solve it on one side of the whiteboard, where it’s visible but won’t get in the way. You don’t need to be verbose, just get the steps in order and somewhat readable.


Start at middle of array.

Keep variables tracking left and right boundaries of search area.

If value equal to search_val, return true.

If left and right boundaries are adjacent, return false.

If value bigger than search_val, go halfway towards left boundary, and move the right boundary along with us.

If value smaller than search_val, go halfway towards right boundary, and move the left boundary along with us.


3) Write pseudocode first.

Time to write code? Nope. Take a “dry run” at writing the code by writing some pseudocode. Often we run into problems halfway through writing the code, and there’s no point wasting time over syntax when you might have to throw the code away. Instead, write some half-baked code-looking stuff that lays out the structure of how your code will work. Do it over on the side of the whiteboard, so you have space left to work.
