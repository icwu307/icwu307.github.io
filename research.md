# Research of [I-Chen Wu][icwu]

## Research Interests

Most of our research interests are related to **machine learning** and **computer games** applications, especially for **Deep Reinforcement Learning (DRL)**. 

- In 2005-2015, we focused more on various research topics related to computer games, such as board games, card games, puzzle games, video games, etc. 
- After 2015, we extended our researches from computer games to various DRL applications, such as learning-based autonomous vehicles (like AWS DeepRacer), intelligent traffic managements, scheduling, combinatorial optimization, large language models (RLHF), etc. 

**Welcome to join us, NCTU+Sinica CGI lab, as Postdoc, RA, M.S./Ph.D. students. If interested, please contact Cindy Ko <cindyko@nycu.edu.tw>.** 

(Updated in October, 2021)

---

## Research Topics and Achievements

List our research topics as well as achievements (since 2005).  
(In publications, notations: J: Journal, C: Conference, B: Book Chapter, #: the ordinal number, but the numbers may be incorrect in IE browser.)

---

(Machine-learning-related)

### Deep Reinforcement Learning Related to AlphaZero

- Developed a multi-labelled value network (ML-VN) with a Go program, which allows programs to play different komis. Also see [publications [J 58]][publications] and [honors][honors].
  - June 2017: Won the human-AI-cooperation match (China-Korea-Taiwan) in the Go AI and IoT workshop in Fu-Chou, China (中韓台人機配對賽冠軍).
  - August 2017: Won the second place in the 1st World AI Go Open, held in Ordos, Inner Mongolia, China. (首屆世界智能圍棋公開賽亞軍) Actually, we won all games during the day-1 preliminary, including beating FineArt (developed by Tencent Inc.; 中國騰訊) and DeepZenGo. Received a prize of RMB$100,000 (about NT$450,000).
  - July 2017: Won two games against Chun-Hsun Chou (9p; 周俊勳九段–––紅面棋王) in IEEE FUZZ 2017 Go Human-Computer competitions.
  - December 2017 - March 2018: Won against Yuan-Jun Wang (王元均) in all of the three man-machine Go games in Mei-Chu tournament. (戊戌梅竹人機圍棋對弈)
  - October 2017 – March 2018: Won against many top Go players, including those ranked top 3 in the world (世界排名前三名), Ke Jie (柯潔), Park Junghwan (朴廷桓), Mi Yuting (羋昱廷).
  - October 2017: CGI was awarded a 10-dan title from Fox Weiqi website. (中國野狐網站十段頭銜)
  - 2017: Received NT$6,600,000 donation from HaiFong Weichi Foundation (海峰棋院), and NT$3,000,000 donation from MediaTek (聯發科).
- Proposed an approach to strength adjustment and assessment for MCTS based game-playing programs, especially for Go. Particularly, developed a computer Go lifelong learning system, which is the world's first Go system that is able to cover different strengths from beginners to super-human, and dynamically analyze the opponent's strength.
  - This research result was selected as an exhibition in the 2018 Future Tech.
  - A paper for this was presented in the top-tier conference AAAI-19 for presentation (acceptance rate = 1,150/7,095 = 16.2%) and published in IEEE CIM (IF=11.356). Also see [publications [C 76, J 65]][publications].
- Proposed a technique to improve AlphaZero, named Multiple Policy Value Monte Carlo Tree Search, presented in IJCAI 2019 (Acceptance rate: 850/4752 = 17.9%). Also see [publications [C 78]][publications].
- Proposed a novel method to adjust hyperparameters of AlphaZero programs such that CGI obtained a winrate of 74% against ELF OpenGo (developed by Facebook), the state-of-the-art open-sourced AlphaZero with 20-block Network then. 
  - In addition, this method can also save 10+ times computing resources. 
  - The result was presented in AAAI 2020 (Oral Presentation 453/7737 ~= 5.85%). Also see [publications [C 83]][publications].
- Proposed a technique to learn AlphaZero faster, namely learning to stop, presented in AAAI 2021 (Acceptance rate: 1,692/7,911 ~= 21.4%). Also see [publications [C 88]][publications].
- Develop an AlphaZero framework.
  - On top of the framework, we have developed some game programs which can beat state-of-the-art programs, such as NoGo.
- Develop a Dark Chess AlphaZero program, an AlphaZero program for stochastic games. Also see [publications [C 73]][publications].
  - Won the Best Paper Award in TAAI 2018. Also see [honors].
- Develop game solving algorithms based on AlphaZero.
  - Propose state-of-the-art algorithms for solving life-and-death (tsumegos) problems (like those in 趙治勳死活辭典). Also see [publications [C 92 93 105, J 76]][publications]

### Deep Reinforcement Learning for Robotics

- Propose a new end-to-end hybrid action space DRL method, which can greatly improve the profermance of grasping and pushing tasks for robotics arms. The result is presented in NIPS 2018 workshop. Also see [publications [C 74]][publications].
- Propose a new cross entropy method (combined with DDPG), which can achieve a much better success rate than DDPG.

### Deep Reinforcement Learning for AI bots of video games

- Developed a distributed end-to-end DRL algorithm that can surpass human players for some specific video games.
- Proposed a new state presentation method that can characterize the perception on environmental changes of AI bot, which helps provide a way of interpretability.
- Proposed the ﬁrst metric for video game playstyles directly from the game observations and actions, without any prior speciﬁcation on the playstyle in the target game, and also proposed a human-like RL algorithm. 
  - This method was presented in a top-tier conference, UAI 2021. Also see [publications [C 90 104]][publications].

### Deep Reinforcement Learning for Autonomous Car Racing

- Proposed an approach to running fast for car racing and raising stability at the same time. 
  - This method was published in a workshop related to autonomous agile vehicles of IROS. Also see [publications [C 86 95 96 103]][publications].
  - The 1st and 3rd places (among 90+ participants) in AWS DeepRacer Summit Taipei (台北實體賽)
  - The 1st and 2nd places (among 1983 competitors) in Virtual Circuit Toronto Turnpike (虛擬賽) of AWS DeepRacer League, in October 2019. **Achieve a world record of 7.172 seconds**, noted in [the AWS web site](https://aws.amazon.com/tw/blogs/machine-learning/aws-deepracer-league-the-championship-lineup-is-complete-making-for-an-exciting-reinvent-2019-final/). 
  -	The 3rd place among 60+ competitors (selected among 8000+ participants) in AWS re:Invent 2019 (世界賽) held in Las Vegas, 2019.
  - **The 1st and 3rd places among competitors (selected among 10000+ participants) in 2020 Championship Cup of AWS DeepRacer League**.
  - **The 1st, 2nd and 3rd places (top three) among 150,000+ participants in 2022 Championship Cup of AWS DeepRacer League**.


### Reinforcement Learning for Other Games

- Temporal Difference Learning for Connect6. Also see [publications [C 39, B 5]][publications].
- Temporal Difference Learning for 2048. Also see [publications [J 41 52 68, C 56]][publications]. The algorithm in [J 69] reached state-of-the-art. 
- Monte-Carlo Tree Search, which are included in most of our developed game programs (see below) and our FJSP work (see below).

### Reinforcement Learning for combinational optimization problems, such as job-shop scheduling.

- Propose new RL algorithms for job-shop scheduling. See also [publications [C 52 64 80 101, R 23]][publications].

### Deep Learning

- Propose a new stochastic gradient descent with hyperbolic-tangent decay. Also see [publications [C 75]][publications].
- Use deep learning to predict sleep quality from wearable data.

Note: since the progress in this part has been made so fast, the research topics and achievements described here may not be up to date. Please directly consult with lab members for the latest research in more detail.

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
  - Some new techniques were developed, including M&M, Dynamic Tree Splitting for parallelization, etc. Also see [publications [C 47, J 64]][publications].
  - **Honor:** A developed Chinese chess program, named Chimo (棋謀), won a gold medal in Computer Olympiad 2017. Also see [honors].
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

### Game-playing programs for imperfect information and stochastic games 

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
  - Novel TD learning techniques were developed to improve AI programs for 2048-like games. Also see [publications [J 41 52 68, C 56]][publications].
  - **Achievement: The first 2048 AI program reached 65536-tile in the world, to the best of our knowledge.** See the [replay](http://2048.cgilab.nctu.edu.tw/replay.php).
  - state-of-the-art: [J 69] reached state-of-the-art, namely, **the reaching rate of 32,768 is up to 72%**. 
  - **Honor:** A 2048 AI program, named CGI-2048, won the second place in the 2048 group of Taiwan 2048 Bot Tournament in 2014. Also see [honors].  
  - **_More information about our 2048 program can be found in [here](aigames/2048.html)._**
  - **Honor:** A Threes! AI program, named CGI-Threes, won the first place in the Threes group of Taiwan 2048 Bot Tournament in 2014. Also see [honors].
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
