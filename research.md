# Research of [I-Chen Wu][icwu]

## Research Interests

Most of our research interests are related to **machine learning** and **computer games** applications, especially for **Deep Reinforcement Learning (DRL)**. 

- In 2005-2015, we focused more on various research topics related to computer games, such as board games, card games, puzzle games, video games, etc. 
- After 2015, we extended our researches from computer games to various DRL applications, such as learning-based autonomous vehicles (like AWS DeepRacer), intelligent traffic managements, scheduling, combinatorial optimization, large language models (RLHF), etc. 
- After 2022, while DRL is still our main focus, we further extended our researches to **large language models (LLMs)**, such as LLM alignment, LLM evaluation and benchmarking, and LLM agents. 

**Welcome to join us, NYCU+Sinica CGI lab, as Postdoc, RA, M.S./Ph.D. students. If interested, please contact Cindy Ko <cindyko@nycu.edu.tw>.** 

(Updated in August, 2026)

---

## Research Topics and Achievements

List our research topics as well as achievements (since 2005).  
(In publications, notations: J: Journal, C: Conference, B: Book Chapter, #: the ordinal number, but the numbers may be incorrect in web browsers.)

---

(Machine-learning-related)

### Deep Reinforcement Learning Related to AlphaZero

- Developed a multi-labelled value network (ML-VN) with a Go program, which allows programs to play different komis. Also see [publications [J 59]][publications] and [honors][honors].
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
  - Propose an AlphaZero-based proof cost network (PCN) to guide game solving, presented in ICLR 2022. Also see [publications [C 93]][publications].
  - Propose game solving with online fine-tuning, which fine-tunes the network during solving. The result was presented in NeurIPS 2023 (Acceptance rate: 26.1% among 12,343). Also see [publications [C 107]][publications].
  - Solve 7x7 Killall-Go with a seki database, and further propose relevance-zone reduction to reduce the solving cost significantly. Also see [publications [C 112 121]][publications].
  - Propose a local-pattern related look-up table to speed up game solvers. Also see [publications [J 81]][publications].
  - Make a comprehensive study of relevance-zone based solvers for Go life-and-death problems, published in the IEEE Transactions on Games. Also see [publications [J 85]][publications].
- Investigate the robustness of AlphaZero-like agents, and show that such agents are still vulnerable to adversarial perturbations. The result was presented in NeurIPS 2022 (Acceptance rate: 2,672/10,411 ~= 25.6%). Also see [publications [C 99]][publications].
- Extend AlphaZero/MuZero to stochastic and imperfect information games.
  - Analyze tabular AlphaZero on strongly-solved stochastic games, and study Gumbel MuZero on EinStein Würfelt Nicht! and 2048. Also see [publications [J 73, C 98 106]][publications].
  - Propose MAPLE (Multi-state Aggregated Policy Evaluation), which extends AlphaZero to imperfect information games, presented in IEEE Conference on Games 2026. Also see [publications [C 127]][publications].
  - Develop WallZero, an AlphaZero-based program together with strategic analysis for the game of WallGo. Also see [publications [C 124]][publications].

### Large Language Models (LLM)

- Propose Auto-Guideline Alignment (AGA), an alignment framework which uses concise and human-readable guidelines as transparent reward proxies, instead of expensive human labeling in RLHF.
  - AGA uses a small amount of human-annotated data (e.g., 1,000 pairs) to iteratively refine alignment guidelines through a feedback loop between annotator and reflector models, and then synthesizes large-scale preference data (e.g., 240,000 pairs) accordingly.
  - AGA is further used to uncover, audit and steer the hidden ideological preferences of LLMs by prompt engineering only, without any parameter updates. Experiments on a dataset of 600 political dilemmas covering 30 topics show that LLMs exhibit a consistent left-leaning bias, and that AGA is able to steer models to all 25 domain-level ideology mixtures.
  - The result was presented in the 2nd Workshop on Models of Human Feedback for AI Alignment (MoFA) in ICML 2025. Also see [publications [C 118]][publications].
- Study political sycophancy of LLMs, namely how LLMs shift their political stances to cater to users during conversations.
  - Propose a framework that disentangles two distinct triggers of political sycophancy, opinion (aligning with explicit narratives) and identity (stereotyping based on demographic labels), evaluated on 450 manually-checked political dilemmas over 13 instruction-tuned LLMs.
  - The results show that susceptibility to explicit opinions does not predict the tendency to stereotype by identity labels, and that system-level personas fail to restrict user-driven drifts. This warns that naive personalization may trap users in stealthy algorithmic echo chambers.
  - The results will be presented in the 2026 Conference on Empirical Methods in Natural Language Processing (EMNLP 2026). Also see [publications [C 130]][publications].
  - This work is supported by a four-year NSTC project (國科會計畫) "Towards Communicative Agentic AI via Strategic Reasoning Agents" (從策略推理邁向溝通型代理式人工智慧) starting from 2025.  
- Propose a belief-shift evaluation benchmark for LLM agents in social-deduction games, such as Werewolf (狼人殺).
  - Most existing evaluations for LLM agents rely on final game outcomes only, which reveal little about communication behaviors. Instead, we measure how an observing agent's beliefs change before and after each suspicion or accusation message, which is closely related to theory of mind.
  - Evaluate 40 open-weight LLM configurations on 1,224 annotated messages from 200 LLM-played games. The results show that larger models better distinguish wolves from villagers, but their beliefs are still strongly influenced by accusations, especially from accusers they trust. This suggests that current LLMs still struggle to integrate accusation content with source trust.
  - The results will be presented in the 2026 Conference on Empirical Methods in Natural Language Processing (EMNLP 2026). Also see [publications [C 129]][publications].
  - This work is supported by a four-year NSTC project (國科會計畫) "Towards Communicative Agentic AI via Strategic Reasoning Agents" (從策略推理邁向溝通型代理式人工智慧) starting from 2025.  
- Develop TaiwanVQA, a visual question answering (VQA) benchmark for evaluating and enhancing cultural understanding of vision-language models (VLMs), collaborated with the TAIDE project.
  - The benchmark contains 2,736 images and 5,472 manually designed questions on culturally specific topics of Taiwan, such as traditional food, public signs, festivals and landmarks, among which 1,000 images and 2,000 questions form the official benchmark set.
  - Experiments show that state-of-the-art VLMs perform well on recognition but poorly on cultural reasoning. We further propose a culture-specific data augmentation strategy, which significantly improves the performance on TaiwanVQA while maintaining that on other multimodal tasks.
  - The results were presented in NeurIPS 2025 (Datasets and Benchmarks Track; acceptance rate: 497/1,995 = 24.91%) and in the First Workshop on Evaluation of Multi-Modal Generation (EvalMG25) in COLING 2025. Also see [publications [C 114 122]][publications].

### Deep Reinforcement Learning for Autonomous Car Racing

- Proposed an approach to running fast for car racing and raising stability at the same time. 
  - This method was published in a workshop related to autonomous agile vehicles of IROS. Also see [publications [C 86 95 96 103]][publications].
  - The 1st and 3rd places (among 90+ participants) in AWS DeepRacer Summit Taipei (台北實體賽)
  - The 1st and 2nd places (among 1983 competitors) in Virtual Circuit Toronto Turnpike (虛擬賽) of AWS DeepRacer League, in October 2019. **Achieve a world record of 7.172 seconds**, noted in [the AWS web site](https://aws.amazon.com/tw/blogs/machine-learning/aws-deepracer-league-the-championship-lineup-is-complete-making-for-an-exciting-reinvent-2019-final/). 
  -	The 3rd place among 60+ competitors (selected among 8000+ participants) in AWS re:Invent 2019 (世界賽) held in Las Vegas, 2019.
  - **The 1st and 3rd places among competitors (selected among 10000+ participants) in 2020 Championship Cup of AWS DeepRacer League**.
  - **The 1st, 2nd and 3rd places (top three) among 150,000+ participants in 2022 Championship Cup of AWS DeepRacer League**.

### Deep Reinforcement Learning for Robotics

- Propose a new end-to-end hybrid action space DRL method, which can greatly improve the profermance of grasping and pushing tasks for robotics arms. The result is presented in NIPS 2018 workshop. Also see [publications [C 74]][publications].
- Propose a new cross entropy method (combined with DDPG), which can achieve a much better success rate than DDPG.
- Propose to use dense object descriptors, learned from simulation and transferred to the real world, for picking cluttered general objects with RL. The results were presented in ICRA 2022 and ICRA 2023. Also see [publications [C 94 100]][publications].
- Propose image-based and gradient-based regularization methods for action smoothness in robotic control, which help reduce jerky behavior without sacrificing performance. The results were presented in IROS 2023 and IROS 2024. Also see [publications [C 104 109]][publications].
- Propose a curriculum RL approach, from avoiding collisions to navigating among movable obstacles (NAMO) in diverse environments, published in IEEE Robotics and Automation Letters and presented in IROS 2023. Also see [publications [J 74, C 103]][publications].

### Deep Reinforcement Learning for AI bots of video games

- Developed a distributed end-to-end DRL algorithm that can surpass human players for some specific video games.
- Proposed a new state presentation method that can characterize the perception on environmental changes of AI bot, which helps provide a way of interpretability.
- Proposed the ﬁrst metric for video game playstyles directly from the game observations and actions, without any prior speciﬁcation on the playstyle in the target game, and also proposed a human-like RL algorithm. 
  - This method was presented in a top-tier conference, UAI 2021. Also see [publications [C 90 104]][publications].
  - The metric was further extended to perceptual similarity for measuring decision-making styles and policy diversity in games, published in TMLR. Also see [publications [J 82]][publications].
- Propose methods of analyzing game balance for PvP games, by identifying and clustering counter relationships of team compositions, and by online learning of counter categories and ratings. Also see [publications [J 83, C 117]][publications].
- Propose new approaches to human-like RL agents.
  - Propose adaptive behavioral costs to tame non-naturalistic behavior of deep RL agents in 3D games, presented in ACML 2023. Also see [publications [C 105]][publications].
  - Propose to learn human-like RL agents through trajectory optimization with action quantization, presented in NeurIPS 2025 (Acceptance rate: 5,290/21,575 = 24.52%). Also see [publications [C 123]][publications].

### Multi-Agent Reinforcement Learning (MARL)

- Propose dynamic sight range selection, which adjusts the sight ranges of agents during training and thus improves the learning efficiency of MARL. The result was presented in AAMAS 2025 as a full paper (Acceptance rate = 24.5%). Also see [publications [C 116]][publications].
- Propose a multi-agent training approach for Pommerman, based on curriculum learning and population-based self-play. Also see [publications [C 110]][publications].

### Deep Reinforcement Learning for Intelligent Traffic Management

- Propose a robust and efficient MARL framework for traffic signal control, which is designed to work in real-world road networks. Also see [publications [C 126]][publications].
- Develop VissimRL, an MARL framework for traffic signal control based on the Vissim traffic simulator, which is widely used by traffic engineers. Also see [publications [C 125]][publications].

### Reinforcement Learning for Other Games

- Temporal Difference Learning for Connect6. Also see [publications [C 39, B 5]][publications].
- Temporal Difference Learning for 2048. Also see [publications [J 41 52 68, C 56]][publications]. The algorithm in [J 71] reached state-of-the-art. 
- Monte-Carlo Tree Search, which are included in most of our developed game programs (see below) and our FJSP work (see below).

### Reinforcement Learning for combinational optimization problems, such as job-shop scheduling.

- Propose new RL algorithms for job-shop scheduling. See also [publications [C 52 64 80 101, R 23]][publications].
- Propose residual scheduling, a new RL approach based on graph neural networks (GNN) for job shop scheduling (JSP) and flexible JSP, which reaches the state-of-the-art and even finds optimal solutions for some public benchmarks. Also see [publications [J 80, C 101]][publications].

### Theoretical Analysis for Reinforcement Learning

- Prove that PPO-Clip attains global optimality, which offers deeper understandings of the clipping mechanism widely used in practice. The result was presented in AAAI-24 (Acceptance rate = 23.75%). Also see [publications [C 108]][publications].
- Propose POIL (Preference Optimization for Imitation Learning), which applies preference optimization to imitation learning without adversarial training. Also see [publications [C 119]][publications].

### Deep Learning

- Propose a new stochastic gradient descent with hyperbolic-tangent decay. Also see [publications [C 75]][publications].
- Use deep learning to predict sleep quality from wearable data.
  - Collaborating with Belun Technology, develop deep-learning-based algorithms on a wearable ring for detecting obstructive sleep apnea (OSA), categorizing apnea severity, and classifying sleep stages. Also see [publications [J 69 78]][publications].
  - Propose a synthetic-to-real diffusion-based approach to denoising photoplethysmography (PPG) signals for sleep monitoring applications, to be presented in the 22nd Annual International Conference on Body Sensor Networks (IEEE EMBS BSN 2026). Also see [publications [C 128]][publications].
- Use DRL and deep learning for autonomous underwater vehicles (AUV), including an intelligent underwater recognition system and a depth-keeping control system. Also see [publications [J 72 75]][publications].

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
- Solve 7x7 Killall-Go, based on AlphaZero-based solvers together with a seki database. Also see [publications [C 112]][publications].

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
  - **Honor:** Won the gold medals of Connect6 in Computer Olympiad 2020, 2021, 2022 and 2023. Also see [honors].
- Develop game-playing programs for Chinese chess.
  - Some new techniques were developed, including M&M, Dynamic Tree Splitting for parallelization, etc. Also see [publications [C 47, J 64]][publications].
  - **Honor:** A developed Chinese chess program, named Chimo (棋謀), won a gold medal in Computer Olympiad 2017. Also see [honors].
- Develop game-playing programs for Go.
  - Some new techniques were developed, including MCTS, RAVE, MCTS parallelism, supervised learning (SL) policy network, reinforcement learning (RL) policy network, value network (VN), etc.
  - **Honor:** A developed program, named HappyGo, won the silver medal in TAAI 2010 tournament.
  - **Honor:** Another program, named Amigo, was in the fourth place in Computer Olympiad in 2013.
  - **Honor:** Our latest program, named CGI (renamed CGI abbreviated from "CGI Go Intelligence"), won the gold metal for 9x9, 13x13, 19x19 Go in TCGA 2015, and the bronze metal for 9x9 Go in Computer Olympiad 2015.
  - **Honor:** CGI 2.0 won the 6th among 30+ teams in UEC Cup 2016. Also won all games (including ZEN, the first in the tournament) and the first on the first-day preliminary tournament, and won the only student award.
  - **Honor:** Won the gold medals of Go 9x9 in Computer Olympiad 2019, 2020, 2021 and 2023. Also see [honors].
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
  - New techniques were further developed, including Monte-Carlo simulation, importance sampling for MCTS, a look-up table for deficiency number calculation, and an efficient method for assessing the strength of Mahjong programs. Also see [publications [J 70 84, C 113 115]][publications].
  - **Honor:** Won the gold medals of Mahjong in Computer Olympiad 2020, 2022, 2023 and 2024. In particular, a developed program, named MEOWCATS, won the Mahjong tournament in Computer Olympiad 2023. Also see [honors].
- Develop game-playing programs for Dark chess.
  - Some new techniques were developed, including MCTS, etc. Also see [publications [J 49 52 55, C 58]][publications].
  - **Honor:** A developed program, named DarkKnight, won Dark chess tournament in Computer Olympiad in 2013. Also see [honors].
  - **Honor:** Won the gold medals of Dark chess in Computer Olympiad 2022 and 2024. Also see [honors].
  - **_More information about our DarkKnight program can be found in [here](aigames/DarkKnight.html)._**
- Develop game-playing programs for EinStein würfelt nicht.
  - Some new techniques were developed, including MCTS/n-tuple networks, etc. Also see [publications [C 68]][publications].
  - **Honor:** A developed program, named DarkKnight, won Eistein tournament in Computer Olympiad in 2018. Also see [honors].
  - **Honor:** Won Merit Paper Award in TAAI 2017. Also see [honors].
  - Gumbel MuZero was further applied to both stochastic and deterministic versions of the game. A developed program, named MuMu, won the Einstein tournament in Computer Olympiad 2023. Also see [publications [J 79, C 106]][publications].

### Game-playing programs for puzzle games

- Develop 2048-like AI games based on the technique of TD (temporal difference) learning.
  - Novel TD learning techniques were developed to improve AI programs for 2048-like games. Also see [publications [J 41 52 68, C 56]][publications].
  - **Achievement: The first 2048 AI program reached 65536-tile in the world, to the best of our knowledge.** <!-- See the [replay](http://2048.cgilab.nctu.edu.tw/replay.php). -->
  - state-of-the-art: [J 69] reached state-of-the-art, namely, **the reaching rate of 32,768 is up to 72%**. 
  - Optimistic temporal difference learning was further proposed for 2048, published in the IEEE Transactions on Games. Also see [publications [J 71]][publications].
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
  - New solving approaches were also proposed for other puzzle games, e.g., an entropy-based two-phase optimization algorithm for Wordle-like games, and a study of evaluating game difficulty in Tetris block puzzles. Also see [publications [C 97 120]][publications].

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
