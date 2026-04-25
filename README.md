# 🎱 BINGO GAME

> *"i just wanted to play bingo with my friends through online and I didn't find any free website that suited my taste, so yea I made one* - what boredom does to a person

---

## What is this

okay so you know how bingo is super fun but like... every online version is either:
- 💀 requires an account
- 💀 has 47 ads
- 💀 looks like it was designed in 2003
- 💀 crashes when more than 2 people join

yeah. **so i built my own.** it took a while. it works. mostly. 

I was inspired by skribble.io so I made this bingo — you create a room, send the link to your friends, everyone makes their own board, and you take turns calling numbers. no login. no nonsense. just vibes and bingo.

---

## features (the cool ones)

```
✅ no login required — just type a name and go
✅ create a room, get a link, share it
✅ custom grid sizes (3x3 all the way to 10x10)
✅ custom number ranges (you decide min and max)
✅ everyone makes their OWN board (drag numbers into slots or just click on the numbers and then on the needed box on the grid)
✅ free space in the middle
✅ real-time number calling with live feed
✅ automatic bingo detection
✅ confetti when someone wins 🎉
✅ up to 6 players
✅ actually works on mobile
```

---

## how to play

**step 1 — create a room**

someone has to be the host (it's a curse but also an honour). as host you pick:
- grid size (5x5 is the classic, 10x10 if you hate your friends)
- number range (1–25? 1–100? go wild)
- how many BINGOs to win

**step 2 — share the link**

copy the room link/code, throw it in the group chat, wait for everyone to join. the host sees a "start game" button once at least 2 people are in.

**step 3 — build your board**

here's where it gets personal. you get a pool of numbers and you arrange them on your grid HOWEVER YOU WANT. just like the paper version from school. no randomiser forcing you to have 13 in the corner (unless you want 13 in the corner).

**step 4 — play!**

turns rotate through everyone. when it's your turn you pick a number. everyone sees it. everyone marks their boards. repeat until someone yells BINGO (the app does it automatically but like, yell anyway, it's more fun).

**step 5 — cry or celebrate**

first to get the required number of BINGOs wins. host can start a rematch.

---

## bingo win conditions

| grid | BINGOs to win |
|------|--------------|
| 3x3  | 3 |
| 4x4  | 4 |
| 5x5  | 5 |
| 6x6+ | 5 |

rows, columns, and diagonals all count. FREE space in the middle. When you want to mark a bingo, click on the boxes that lead to the bingo, mark it.

---

## tech stuff

built with absolutely zero frameworks

```
frontend  → vanilla HTML / CSS / JS (one single file btw)
realtime  → Firebase Realtime Database
hosting   → hosted on vercel - https://bingo-game-01.vercel.app/
confetti  → canvas-confetti 
```

**why Firebase?** free tier is generous enough for a group of friends and i'm not paying for a server for a bingo game.

---

## setup (if you want to run your own)

1. clone this repo or just grab the `index.html` file
2. create a Firebase project at [firebase.google.com](https://firebase.google.com)
3. enable **Realtime Database** (test mode is fine)
4. add a web app and copy your `firebaseConfig`
5. paste your config into `index.html` where it says `// PASTE YOUR FIREBASE CONFIG HERE`
6. open in browser
7. play bingo

that's genuinely it. no npm install. no build step. no docker. just a file.

---

## Bugs to be checked

- if the host closes the tab mid-game, it gets a bit weird. don't do that.
- tested on chrome
- if two people call a bingo at the exact same millisecond... honestly haven't tested that. let me know how it goes.

---

## why did i make this

because me and my friends kept saying "we should play bingo sometime" and then never did because the setup was annoying. now the setup is not annoying. problem solved. 

also i wanted to learn hosting and this seemed like a fun excuse.

---

## contributing

if you find a bug, open an issue! if you want to add something cool, PR is welcome. if you just want to say hi, that's also fine.

please don't add monetisation or ads. this is a bingo game for friends. it should stay free and fun forever.

---

*made by Agila*
