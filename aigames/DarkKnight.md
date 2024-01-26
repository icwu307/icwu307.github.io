# Introduction to Chinese Dark Chess Program Developed at CGI Lab

This page introduces the history of Chinese dark chess program, DarkKnight, developed in [Computer Games and Intelligence (CGI) Lab][cgi_lab], led by Professor [I-Chen Wu][icwu], at [Department of Computer Science][nctu_cs], National Chiao Tung University, Taiwan; and also acknowledges the contributors who are/were the members of the CGI lab.

- [Early design of DarkKnight (2012-2013)](#early-design-of-darkknight-2012-2013-)
- [More strength improvements for DarkKnight (2014-)](#more-strength-improvements-for-darkknight-2014-)

---

## Early design of DarkKnight (2012-2013)

Wen-Jie Tseng (曾汶傑) wrote the whole Chinese dark chess program based on Monte-Carlo Tree Search (MCTS), when he served as a TA in the course, Theory of Computer Games, taught by Professor [I-Chen Wu][icwu] in 2012 fall. Note that the project of this course in 2012 was to write Chinese dark chess programs. He did not use much domain-specific knowledge except for using piece weights in playouts. He developed the program quickly by reusing part of his code for Chimo, a Chinese chess program developed mainly by him in [CGI lab][cgi_lab].

### Authors

<table>
<tbody>
<tr>
<td>Wen-Jie Tseng (曾汶傑)</td>
<td>2012-2013</td>
<td>Wrote most of the code of DarkKnight, which is based on MCTS.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2012-2013</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- Mainly implemented Monte Carlo Tree Search with few domain-specific knowledge, except for playouts which used capturing and escaping.
- Supported multi-threading.
- The program ran fast, about 30,000 simulations per second in a single thread for initial positions.

### Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2013</td>
<td>TAAI computer game tournaments</td>
<td>3rd place (Bronze)</td>
</tr>
<tr>
<td>2013</td>
<td>Computer Olympiad</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2013</td>
<td>TCGA computer game tournaments</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2012</td>
<td>TAAI computer game tournaments</td>
<td>5th place</td>
</tr>
</tbody>
</table>

### Publications

1. Shi-Jim Yen, Jr-Chang Chen, Bo-Nian Chen, and Wen-Jie Tseng, "DarkKnight Wins Chinese Dark Chess Tournament", ICGA Journal, Vol. 36, No. 3, pp. 175-176, 2013
1. Wen-Jie Tseng, Jr-Chang Chen, Lung-Ping Chen, Shi-Jim Yen, and I-Chen Wu, "TCGA 2013 Computer Game Tournament Report", ICGA Journal, Vol. 36, No. 3, pp. 166-168, 2013
1. Tsan-Cheng Su, Shi-Jim Yen, Jr-Chang Chen, and I-Chen Wu, "TAAI 2012 Computer Game Tournaments", ICGA Journal, Vol. 37, No. 1, pp. 33-35, 2014

---

## More strength improvements for DarkKnight (2014-)

Based on the original DarkKnight, Chu-Hsuan Hsueh (薛筑軒) incorporated several techniques including early playout terminations, implicit minimax backups, quality-based rewards, and progressive bias to improve the playing strength. Besides, she also did some tunings for tournaments, e.g. time management, dealing with 180 plies to draw.

### Authors

<table>
<tbody>
<tr>
<td>Chu-Hsuan Hsueh (薛筑軒)</td>
<td>2014-current</td>
<td>Made most changes and improvements over original DarkKnight.</td>
</tr>
<tr>
<td>Wen-Jie Tseng (曾汶傑)</td>
<td>2014-current</td>
<td>Assisted on implementing early playout terminations and implicit minimax backups.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2014-current</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- Early playout terminations: Terminate a playout much earlier when it is very likely to win, lose, or draw.
- Implicit minimax backups: Guide MCTS selections by using minimax scores (from heuristic evaluations) of tree nodes together with the original simulated win rates.
- Quality-based rewards: Use simulation length and terminal state quality to adjust the rewards returning from simulations.
- Progressive bias: Guide MCTS selections by heuristic scores from domain-specific knowledge.

### Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2015</td>
<td>Computer Olympiad</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2015</td>
<td>TCGA computer game tournaments</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2014</td>
<td>TAAI computer game tournaments</td>
<td>7th place</td>
</tr>
<tr>
<td>2014</td>
<td>TCGA computer game tournaments</td>
<td>2nd place (Silver)</td>
</tr>
</tbody>
</table>

### Publications

- Chu-Hsuan Hsueh, I-Chen Wu, Wen-Jie Tseng, Shi-Jim Yen, and Jr-Chang Chen, "Strength Improvement and Analysis for an MCTS-Based Chinese Dark Chess Program", in the 14th International Conference Advances in Computer Games 2015 (ACG 2015), Leiden, the Netherland, 2015.
- Chu-Hsuan Hsueh and I-Chen Wu, "DarkKnight Wins Chinese Dark Chess Tournament", to appear in ICGA Journal in 2015.

[icwu]: ..
[cgi_lab]: http://www.aigames.nctu.edu.tw/
[nctu_cs]: https://www.cs.nctu.edu.tw/cswebsite/
