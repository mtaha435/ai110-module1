# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
UI is nice but logic is totally broken
- List at least two concrete bugs you noticed at the start  
U can get negative numbers, and it'll always say "lower" even if you put in -9999999
You can't start a new game its just stuck on game over
  (for example: "the secret number kept changing" or "the hints were backwards").

---

## 2. How did you use AI as a teammate?
- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
ChatGPT free
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
it caught a glitch i didn't notice at first, the game says pick a # between 1 and 100 regardless of the difficulty instead of a number between 'low' and 'high'
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
I think i prompted well enough to not get bad suggestions
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
running app.py or pytesting it, or if it's something like testing upper/lower bounds you can just tell from looking at the code
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
  displaying the upper and lower bounds, tested by running the streamlit app and looking at the displayed text
- Did AI help you design or understand any tests? How?
No i did tests on my own
---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
Streamlit reruns the entire script every time you interact with the app
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
reruns your whole program every time you click a button or type something
- What change did you make that finally gave the game a stable secret number?
I made sure the secret number always stayed as an integer and removed the logic that randomly converted it into a string
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
marking bugs with comments like # FIXME
- What is one thing you would do differently next time you work with AI on a coding task?

- In one or two sentences, describe how this project changed the way you think about AI generated code.
showed me that AI-generated code can look correct on the surface but still have major logic issues underneath.