# Research of [I-Chen Wu][icwu]

## Research Interests

All current research interests are related to **machine learning** and **computer games** applications, especially for **Deep Reinforcement Learning (DRL)**. We have an ongoing project sponsored by MOST, named "Studies of Applications with Deep Reinforcement Learning Technologies", and several industry-university cooperation projects on machine learning, mainly for DRL.

For DRL, we focus on the following research topics.

- Developing a Go program CGI (see below) including DeepMind's AlphaZero technique (called Zero in this page).
- Applying Zero to other game AI, including a framework for Zero.
- Researching on Explainable AI (XAI), especially for Zero-related.
- Developing AI bots of video games.
- Researching on learning-based robotics.

For Computer Games, we are still interested in various topics related to games, such as board games, card games, puzzle games, video games, etc.

Welcome to join us!!

---

## Research Topics and Achievements

List our research topics as well as achievements (since 2005).  
(In publications, notations: J: Journal, C: Conference, B: Book Chapter, #: the ordinal number, but the numbers may be incorrect in IE browser.)

---

(Machine-learning-related)

### Deep Reinforcement Learning Related to Zero

- Develop a multi-labelled value network (ML-VN) with a Go program, which allows programs to play different komis. Also see [publications \[J 58\]][publications].
- Developed a computer Go lifelong learning system, which is the world's first Go system that is able to provide different strengths from beginners to super-human, and dynamically analyze the opponent's strength.
  - This research result is selected as an exhibition in the 2018 Future Tech.
  - A paper for this is accepted by the top conference AAAI-19 for presentation. (acceptance rate = 1,150/7,095 = 16.2%) Also see [publications \[C 76\]][publications].
- Develop a Zero framework.
  - On top of the framework, we have developed some game programs which can beat state-of-the-art programs, such as NoGo.
- Develop a Dark Chess Zero program, a Zero program for stochastic games. Also see [publications [C 73]][publications].
  - **Honor:** Won the Best Paper Award in TAAI 2018. Also see [honors].

### Deep Reinforcement Learning for Robotics

- Propose a new end-to-end hybrid action space DRL method, which can greatly improve the profermance of grasping and pushing tasks for robotics arms. The result is presented in NIPS 2018 workshop. Also see [publications [C 74]][publications].
- Propose a new cross entropy method (combined with DDPG), which can achieve a much better success rate than DDPG.

### Deep Reinforcement Learning for AI bots of video games

- Develop a distributed end-to-end DRL algorithm that can surpass human players for some specific video games.
- Propose a new state presentation method that can characterize the perception on environmental changes of AI bot, which helps provide a way of interpretability.

### Deep Learning

- Propose a new stochastic gradient descent with hyperbolic-tangent decay. Also see [publications [C 75]][publications].
- Use deep learning to predict sleep quality from wearable data.

### Reinforcement Learning for Games

- Temporal Difference Learning for Connect6. Also see [publications [C 39, B 5]][publications].
- Temporal Difference Learning for 2048. Also see [publications [J 41 52, C 56]][publications].
- Monte-Carlo Tree Search, which are included in most of our developed game programs (see below) and our FJSP work (see below).

**Note: since the progress in this part has been made so fast, the research topics and achievements described here may not be up to date. Please directly consult with lab members for the latest research in more detail.**

---

(Computer-games-related)

### New games

- Present a new family of _k_-in-a-row games, including the new game [Connect6] in 2005. Also see [publications [J 11, C 26, B 2]][publications].
  - Connect(m,n,k,p,q): Black plays first and puts only q black stone on unoccupied intersections (also called grids) of an mxn board. Subsequently, Black and White alternately put p of their own stones on unoccupied grids. The one who first gets k or more consecutive stones (horizontally, vertically or diagonally) of her/his own wins. Modern Connect6 is Connect(19,19,6,2,1).
  - It has become a computer game tournament in Computer Olympiad since then.
  - The game has been supported in some game sites, e.g., www.cycgame.com, www.littlegolem.net, pente.org, www.renrousousuo.com, BrainKing.com, etc...
- Present a new Domineering game, named XT Domineering. Also see [publications [J 32, C 35]][publications].
  - The game is much more complicated than Domineering with the same size.
  - The game includes a large number of infinitesimals in terms of combinatorial game theory.

### Solving open problems

- Solve some Connect(k,p), where Connect(k,p) is Connect(infinity,infinity,k,p,p). Also see [publications [J 26, C 32, B 3]][publications].
  - Connect(11,2) is a draw.
  - Consider all p >= 3. Let P(d-1) < p <= P(d), where P(d) = 6\*2^d - d - 4. Then, Connect(3p+3d+8, p) is a draw.
- Solve several Connect6 openings based on job-level computing. Also see [publications [J 34, C 34, B 4]][publications].
  - Include the well-known Mickey Mouse opening and Straight opening.
- Solve a Nim game, called Triangular Nim. Also see [publications [J 29, C 36]][publications].
  - Triangular Nim with size 9 are solved with the first player winning, in both normal and misere versions.
- Solve the minimum Sudoku problem. Also see [publications [J 28 38, C 37]][publications].
  - No 16-clue puzzles exist. BOINC was used to solve it after 2 years and 8 months or so. We are the second team to solve this, independently developed from the first team led by Professor McGuire.
  - All 17-clue puzzles with 3 clues in one column/row block are solved.

### Game-playing programs for perfect information games

- Develop game-playing programs for Connect6.
  - Many new techniques were developed, including relevance-zone-oriented threat-space search, job-level proof-number search, TD-learning, dependency-based learning, dovetaling for parallelization, etc. Also see [publications [J 11 13 15 19 21 25 37, C 26 34 39 42 49, B 2 4 5]][publications].
  - A developed program, named NCTU6 (交大六號), is at the level of top human players.
    - **Honor**: NCTU6 attended Computer Olympiad in 2006 and 2008, and won the gold medal each time. Also see [honors].
    - **Honor:** NCTU6 won against top human players in the first/second/third annual Man-Machine Connect6 Championship, in 2008/2009/2011. Also see [honors].
    - **Honor:** NCTU6 won in 8 championship tournaments among the latest 12 in [Littlegolem](http://littlegolem.net/jsp/games/gamedetail.jsp?gtid=connect6&page=ch) (account: Lomaben and Happy6).
    - **_More information about NCTU6 can be found [here](aigames/NCTU6.html)_**.
  - Another, named mobile6 based on NCTU6, is a mobile version. Note that mobile devices generally run about 10 times slower and support much smaller memory (about 2M bytes only are used in mobile6). Also see [publications [J 37, C 42]][publications].
    - **Honor:** Still won the gold medal in Computer Olympiad 2013. Also see [honors].
  - NCTU6 was used to help build Connect6 puzzle generator (in [Connect6]).
- Develop game-playing programs for Chinese chess.
  - Some new techniques were developed, including M&M, Dynamic Tree Splitting for parallelization, etc. Also see [publications [C 47]][publications].
  - **Honor:** A developed program, named Chimo (棋謀), at about 7-8 dan, won silver medals in the past three Computer Olympiad. Also see [honors].
- Develop game-playing programs for Go.
  - Some new techniques were developed, including MCTS, RAVE, MCTS parallelism, supervised learning (SL) policy network, reinforcement learning (RL) policy network, value network (VN), etc.
  - **Honor:** A developed program, named HappyGo, won the silver medal in TAAI 2010 tournament.
  - **Honor:** Another program, named Amigo, was in the fourth place in Computer Olympiad in 2013.
  - **Honor:** Our latest program, named CGI (renamed CGI abbreviated from "CGI Go Intelligence"), won the gold metal for 9x9, 13x13, 19x19 Go in TCGA 2015, and the bronze metal for 9x9 Go in Computer Olympiad 2015.
  - **Honor:** CGI 2.0 won the 6th among 30+ teams in UEC Cup 2016. Also won all games (including ZEN, the first in the tournament) and the first on the first-day preliminary tournament, and won the only student award.
  - **Ongoing:** Develop new deep learning (DL) and deep reinforcement learning (DRL) techniques for CGI 3.0.
  - **_More information about our Go project and program can be found in [here](aigames/CGI.html)._**
- Develop game-playing programs for NoGo.
  - Some new techniques were developed, including MCTS, RAVE, etc.
  - **Honor:** A developed program, named HappyNoGo, won NoGo tournament in Computer Olympiad in 2013. Especially, it won against BobNoGo, which won the following tournaments without any losses, BIRS 2011, TAAI 2011, Computer Olympiad 2011, TCGA 2012. Also see [honors].
  - **Honor:** Another developed program, named PohsuanNoGo, won the silver medal in the same NoGo tournament of Computer Olympiad in 2013. Also see [honors].
  - **_More information about our NoGo program can be found in [here](aigames/NoGo.html)._**

### Game-playing programs for imperfect information games

- Develop game-playing programs for Mahjong.
  - Some new techniques were developed, including PO-MDP (partially observable Markov decision process), etc.
  - **Honor:** A developed program, named LongCatMJ, won Mahjong tournament in Computer Olympiad in 2013. Also see [honors].
  - **_More information about our Mahjong program can be found in [here](aigames/VeryLongCat.html)._**
- Develop game-playing programs for Dark chess.
  - Some new techniques were developed, including MCTS, etc. Also see [publications [J 49 52 55, C 58]][publications].
  - **Honor:** A developed program, named DarkKnight, won Dark chess tournament in Computer Olympiad in 2013. Also see [honors].
  - **_More information about our DarkKnight program can be found in [here](aigames/DarkKnight.html)._**
- Develop game-playing programs for EinStein würfelt nicht.
  - Some new techniques were developed, including MCTS/n-tuple networks, etc. Also see [publications [C 68]][publications].
  - **Honor:** A developed program, named DarkKnight, won Eistein tournament in Computer Olympiad in 2018. Also see [honors].
  - **Honor:** Won Merit Paper Award in TAAI 2017. Also see [honors].

### Game-playing programs for puzzle games

- Develop 2048-like AI games based on the technique of TD (temporal difference) learning.
  - A new TD learning technique was developed to improve AI programs for 2048-like games. Also see [publications [J 41 52, C 56]][publications].
  - **Achievement: The first 2048 AI program reached 65536-tile in the world, to the best of our knowledge.** See the [replay](http://2048.aigames.nctu.edu.tw/replay.php).
  - **Honor:** A 2048 AI program, named CGI-2048, won the second place in the 2048 group of Taiwan 2048 Bot Tournament in 2014. Also see [honors].  
    The performance of CGI-2048 is still improving. The table (below) shows the performances of the early CGI-2048 (the one for the tournament),
    the latest improved CGI-2048, and [Xificurk's program](https://github.com/nneonneo/2048-ai/pull/27). To the best of our knowledge, Xificurk's
    outperformed all the known 2048 programs (see below) at the time before Octobor 2014. In November 2014, our latest CGI-2048 is able to perform better than Xificurk's.
    More importantly, ours runs about 300 times faster.
    <table align="center">
    <thead>
    <tr>
    <th align="center"></th>
    <th align="center">Early CGI-2048</th>
    <th align="center">Xificurk's Program</th>
    <th align="center">Latest CGI-2048</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td align="center">2048</td>
    <td align="center">100.0%</td>
    <td align="center">100.0%</td>
    <td align="center">100.0%</td>
    </tr>
    <tr>
    <td align="center">4096</td>
    <td align="center">100.0%</td>
    <td align="center">100.0%</td>
    <td align="center">100.0%</td>
    </tr>
    <tr>
    <td align="center">8192</td>
    <td align="center">94%</td>
    <td align="center">99.1%</td>
    <td align="center">99.5%</td>
    </tr>
    <tr>
    <td align="center">16384</td>
    <td align="center">59%</td>
    <td align="center">92.7%</td>
    <td align="center">93.6%</td>
    </tr>
    <tr>
    <td align="center">32768</td>
    <td align="center">0%</td>
    <td align="center">31.7%</td>
    <td align="center">33.5%</td>
    </tr>
    <tr>
    <td align="center">Max score</td>
    <td align="center">367956</td>
    <td align="center">829300</td>
    <td align="center">833300</td>
    </tr>
    <tr>
    <td align="center">Ave score</td>
    <td align="center">251794</td>
    <td align="center">442419</td>
    <td align="center">446116</td>
    </tr>
    <tr>
    <td align="center">Speed</td>
    <td align="center">1200 moves/sec</td>
    <td align="center">2-3 moves/sec</td>
    <td align="center">661 moves/sec</td>
    </tr>
    </tbody></table>
  - **_More information about our 2048 program can be found in [here](aigames/2048.html)._**
  - **Honor:** A Threes! AI program, named CGI-Threes, won the first place in the Threes group of Taiwan 2048 Bot Tournament in 2014. Also see [honors].
    To the best of our knowledge (in August 2014), our program outperforms all the known Threes AI program. Its performance is as follows.
    <table align="center">
    <tbody><tr> 
    <td>384 </td> 
    <td>100%</td> 
    </tr> 
    <tr> 
    <td>768 </td> 
    <td>100%</td> 
    </tr> 
    <tr> 
    <td>1536 </td> 
    <td>97.2%</td> 
    </tr> 
    <tr> 
    <td>3072 </td> 
    <td>68.6%</td> 
    </tr> 
    <tr> 
    <td>6144 </td> 
    <td>10.8%</td> 
    </tr> 
    <tr> 
    <td>Max score</td> 
    <td>790,416</td> 
    </tr> 
    <tr> 
    <td>Ave score</td> 
    <td>229,717</td> 
    </tr> 
    <tr> 
    <td>Speed</td> 
    <td>About 300 moves/sec</td> 
    </tr> 
    </tbody></table>
  - **Honor:** Won the Best Paper Award in TAAI 2014. Also see [honors].
- Develop puzzle game solvers.
  - Some new techniques were developed, including fully-probing techniques, line-painting, etc. Also see [publications [J 22 28 30 38 39, C 37 44]][publications].
  - **Honor:** A Nonogram solver, named LaLaFrogKK, won Nonogram tournament in Computer Olympiad in 2013. Also see [honors].  
    **_More information about our Nonogram program can be found in [here](aigames/LalaFrogKK.html)._**
  - **Honor:** A Nuricabe solver, named HappyNuri, won Nuricabe tournament in Computer Olympiad in 2010. Also see [honors].
  - Some solvers were developed for some other puzzle games, e.g., Slitherlink, Lightup, etc.

### Mathematical optimization problems

- Develop a program to solve MO-FJSP (Multi-Objective Flexible Job Shop Scheduling Problem). Also see [publications [C 52]][publications].
  - The first MCTS-based algorithm that can find the 17 best Pareto solutions for Kacem benchmark problems. </li>
  - **Honor:** Won Merit Paper Award in TAAI 2013. Also see [honors].

### Cloud/grid/software environments

- Propose the job-level (JL) computation model. Also see [publications [J 34, C 34, B 4]][publications].
  - Develop JL proof number search to help solve many Connect6 openings.
  - Develop JL alpha-beta search to help build Chinese chess opening book.
- Develop a desktop grid for developing computer games, named CGDG (computer game desktop grid). Also see [publications [C 31 33 48 50]][publications].
  - Support volunteering computing and job-level algorithms.
  - Include at least 1000 cores, collaborated by at least six research organizations in Taiwan.
- Develop a Generic Board Game Development Framework, which facilitates the developments of computer game. Also see [publications [C 38 40 43 46 51]][publications].
  - Support editing environments for different games by plugin mechanisms.
  - Support different job-level algorithms.
- Develop a Portable AWT/Swing Architecture for Java Game Development. Also see [publications [J 10 12 14 18, C 19 21 29]][publications].
  - Support faster GUI rendering on different platforms.

[icwu]: .
[honors]: honors.html
[publications]: publications.html
[connect6]: http://www.connect6.org
