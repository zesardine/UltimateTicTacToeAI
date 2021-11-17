# Ultimate Tic-Tac-Toe AI

## Details

[Here's a YouTube video](https://youtu.be/BfmivoVFins) about this project.

This is a _minimax_ AI I coded for the game _Ultimate Tic-Tac-Toe_. There were many fun problems I had to solve, most of which I go over in the YouTube video. Even after figuring them out, the AI isn't completely perfect. However, in it's current form, it usually wins, or we tie. I have only won against it once over the span of many dozens of games, although I'm admittedly not a professional Ultimate Tic-Tac-Toe player. I've also put it up against other AIs and it seems to mostly win or tie. (However, I don't really want to make it practice against other AIs, as those also have their flaws).

I will admit, the code is quite old, and there were a lot of problems with the version that I had when I created the video (from the game sometimes crashing when a tie happened to the AI just ignoring the fact that the player was about to win). I have gone over these in the past few days and am happy to say that, to the best of my knowledge, they're all fixed and should work. 

Obviously, if you find any bugs, feel free to inform me. It's possible that there are certain cases that I've not had happen, or I have a specific playstyle which manages to evade a certain issue. It's honestly really hard to debug anything like this, because the AI has a vision of what the _perfect move_ is, and with high search depths it starts to become difficult to understand why it's the _perfect_ move. Thus, many bugs and edge cases can slip under the radar.

## How to Play

Download the source code, unzip it, and open the index.html file. You should be good to go from there.

## Author's side note

The AI starts to get slower as the game progresses, because the search depth is progressively bumped up. Sometimes it will seem like something lagged, but really the AI is just thinking. I tried to place the search depth at the minimum margin at which the AI will win 99% of the time, but as was noted above, I don't think I've gone through enough game combinations to figure out how beatable it is, or what strategies work against it. 

From what I've observed, the games will usually end in a tie if both players play solid moves, but the AI thrives as soon as you make a mistake that it can use against you. Once again, I haven't tested it all that much, this is just what I have observed. When the AI knows that the player will most likely win, it will skew the dark part of the evaluation bar towards the players color. If you see that, you can be quite certain that there's a set of moves you can make to win the game. Good luck finding them!

With this in mind, I'm quite sure that the AI would be significantly better if the search depth was bumped up a bit more, but that'd require some optimization.

## About the code

Honestly, the code is quite poorly formatted, since I had to constantly edit and adjust it, and I didn't exactly pick the best way to make this program in the first place. I tried to put comments at the most important locations, but even then, there's still temporary variable names like _mm_ and _trr_ which eventually just stuck. 
