# NumGuesser
This was a fun project to help develop my html and javascript skills.

NumGuesser Features:
A leaderboard,
A button that shows stats like average guesses per win, total wins, total guesses, guesses on current number,
Entering a username is mandatory (then click submit username)

The code for numguesser is fairly simple,

*(all stats that arent shown on Leaderboard.html are session based, so if you reload the page it all resets other then whats uploaded to leaderboard)*

you start by entering a name then clicking submit name after you click "Click to start",
upon clicking it a random number will be set with "Math.floor(Math.random(1)*1000000)", this just makes a random number between 0 and 1,000,000 (1 million).
you then enter a guess into the dark green-y text box that says "enter number", after which you click the submit guess button (same as click to start button just different text).
Based on what you guessed and what the random number was it will say "***Guess*** is too low" or, "too high", if the guess was correct and it was a new best it will say that it was a new best,
if your guess is the least amount of guesses for a win under the username you entered you'd be entered on the leaderboard with your score
(if your entered on the leaderboard it'll say the score and what position your put at.) then you can just click to start again and keep guessing numbers.

Stats under the random stats button are:
Guesses, which is the total number of guesses for the current random number
Total guesses, which is the total number of guesses in the session
Wins, which is how many times you've guessed the number correct in the session
average guesses per win, its how many guesses you've had divided by wins so totalguesses/wins
your least guesses, it shows the least amount of guesses you've had in the session.

## Leaderboard info

The leaderboard was made with supabase so I can manually go to the supabase website and like enter, remove, or change data on the leaderboard.
Sadly I'm not really good with like Secret key's, and auth and whatnot so anyone could go into the console and use the function to upload guesses to the supabase data base which will be shown on the leaderboard page.
*Also I renamed the variable name from number to something hopefully making it slightly harder for people to figure out if they haven't seen the code.*
The leaderboard is fairly simple it shows position number, username and the number of guesses it took. (and a button to go back to number guessing)
if two people have the same amount of guesses it will display as:
1. user1 - 17 guesses
2. user2 - 20 guesses
2. user3 - 20 guesses
3. user4 - 21 guesses
Or whatever the scores, username and positions are at the time.
