# Introduction to Connect6 Programs Developed at CGI Lab

This page introduces the history of Connect6 programs, mainly for NCTU6, developed in [Computer Games and Intelligence (CGI) Lab][cgi_lab], led by Professor [I-Chen Wu][icwu], at [Department of Computer Science][nctu_cs], National Chiao Tung University, Taiwan. The program won ALL the Computer Connect6 tournaments that we participated, and most human-machine competitions. This page also wants to acknowledge all the contributors involved in the development.

<ul>
	<li><a href="http://aigames.nctu.edu.tw/~icwu/games/NCTU6.html#Early">Early design of Connect6 program (2004-2005)</a></li>
	<li><a href="http://aigames.nctu.edu.tw/~icwu/games/NCTU6.html#Core">The core design of NCTU6 (2006-2010)</a></li>
	<li><a href="http://aigames.nctu.edu.tw/~icwu/games/NCTU6.html#Improve">More strength improvements for NCTU6 (2010-)</a></li>
	<li><a href="http://aigames.nctu.edu.tw/~icwu/games/NCTU6.html#competitions">Competition Summary</a></li>
</ul>

---

## Early design of Connect6 program (2004-2005)

Dei-Yen Huang (黃德彥) decided to write a Connect6 program for his M.S. Thesis on 2004. Actually, this is also the first computer game project of our CGI lab. His program was used to prove a loss for an initial breakaway move and play against human players (with a win rate of about 60%) in a game site in 2005.

### Authors

<table>
<tbody>
<tr>
<td>Dei-Yen Huang (黃德彥)</td>
<td>2004-2005</td>
<td>Wrote a Connect6 program with threat space search (TSS) based on double threats (or so-called Live 4).</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2004-2005</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- Mainly included threat space search based on double threats. The program is slow (about hundreds of moves per second).

### Publications

1. I-Chen Wu, Dei-Yen Huang and Hsiu-Chen Chang, "Connect6", ICGA Journal (SCI), Vol. 28, No. 4, pp. 235-242, December 2005.
1. I-Chen Wu, and Dei-Yen Huang, "A New Family of k-in-a-row Games", the 11th Advances in Computer Games Conference (ACG'11), Taipei, Taiwan, September 2005.

---

## The core design of NCTU6 (2006-2010)

I-Chen Wu (吳毅成) rewrote the whole code and named it "NCTU6" in 2006-2008. Hsiu-Chen Chang (張修逞) assisted on it during this period. Then, Ping-Hung Lin (林秉宏) took over the code and added some more heuristics and relevance zones for TSS starting from 2008.

### Authors

<table>
<tbody>
<tr>
<td>I-Chen Wu (吳毅成) </td>
<td>2006-2010</td>
<td>Rewrote the whole code, NCTU6, including alpha-beta search for move selection and double-threat TSS and single-threat TSS for solving positions. Also supervised the whole project.</td>
</tr>
<tr>
<td>Hsiu-Chen Chang (張修逞)</td>
<td>2006-2007</td>
<td>Assisted on the TSS design of NCTU6.</td>
</tr>
<tr>
<td>Ping-Hung Lin (林秉宏)</td>
<td>2008-2010</td>
<td>Added several useful heuristics and relevance zones.</td>
</tr>
</tbody>
</table>

### Features

- Double-threat TSS and single-threat TSS.
- About tens of thousands moves per second, much faster than the early design.
- Several useful heuristics and relevance zone technique.

### Publications

1. I-Chen Wu and Ping-Hung Lin, "Relevance-Zone-Oriented Proof Search for Connect6", the IEEE Transactions on Computational Intelligence and AI in Games (SCI), Vol. 2, No. 3, pp. 191-207, September 2010.
1. Ping-Hung Lin and I-Chen Wu, "NCTU6 Wins in the Man-Machine Connect6 Championship 2009", ICGA Journal (SCI), vol. 32(4), 2009.
1. I-Chen Wu and Ping-Hung, Lin, "NCTU6-Lite Wins Connect6 Tournament", ICGA Journal (SCI), Vol.31, No.4, December 2008.
1. I-Chen Wu and Shi-Jim, Yen, "NCTU6 Wins Connect6 Tournament", ICGA Journal (SCI), Vol.29, No.3, September 2006.

---

## Strength Improvements (2010-)

Even though we won almost all competitions (human or computers), we still kept improving NCTU6's strength. The first significant improvement is to use TD learning to train better feature weights by Hsin-Ti Tsai (蔡心迪) and Hung-Hsuan Lin (林宏軒). The second is to use dependency-based search to improve TSS performance by Hao-Hua Kang (康皓華) and Ting-Han Wei (魏廷翰). The third is to parallelize NCTU6 by Chieh-Min Chang (張傑閔). We also built a job-level proof-number search algorithm using NCTU6 as jobs by Hung-Hsuan Lin (林宏軒) and Ting-Han Wei (魏廷翰), and built a mobile Connect6 program, named mobile6, by modifying it from NCTU6 by Ji-Hong Zheng (鄭吉閎), Chia-Yun Hu (胡嘉芸) and Hung-Hsuan Lin (林宏軒).

### Authors

<table>
<tbody>
<tr>
<td>Hung-Hsuan Lin (林宏軒)</td>
<td>2010-2013</td>
<td>Assisted TD learning, built job-level proof-number search algorithm, and designed the algorithm used in the mobile6 design. </td>
</tr>
<tr>
<td>Hsin-Ti Tsai (蔡心迪)</td>
<td>2010-2011</td>
<td>Designed and implemented TD learning (the key person).</td>
</tr>
<tr>
<td>Hao-Hua Kang (康皓華)</td>
<td>2011-2012</td>
<td>Designed and implemented dependency-based search(the key person).</td>
</tr>
<tr>
<td>Chieh-Min Chang (張傑閔)</td>
<td>2011-2013</td>
<td>Designed and implemented parallelization of NCTU6 (the key person).</td>
</tr>
<tr>
<td>Chia-Yun Hu (胡嘉芸)</td>
<td>2011-2012</td>
<td>Designed and implemented mobile6 on iOS.</td>
</tr>
<tr>
<td>Ji-Hong Zheng (鄭吉閎)</td>
<td>2011-2012</td>
<td>Designed and implemented mobile6 on Android.</td>
</tr>
<tr>
<td>Ting-Han Wei (魏廷翰)</td>
<td>2013-current</td>
<td>Assisted on job-level proof-number search algorithm, and dependency-based search.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2011-current</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- TD learning for more accurate feature weights.
- Dependency-based search.
- Parallelization of NCTU6.
- Mobile version of Connect6.

### Publications

1. Ting-Han Wei, I-Chen Wu, Chao-Chin Liang, Bing-Tsung Chiang, Wen-Jie Tseng, Shi-Jim Yen, and Chang-Shing Lee, "Job-Level Algorithms for Connect6 Opening Position Analysis", ECAI Computer Games Workshop 2014, Prague, Czech Republic, August 2014.
1. I-Chen Wu, Hao-Hua Kang, Hung-Hsuan Lin, Ping-Hung Lin, Ting-Han Wei, Chieh-Min Chang, Ting-Fu Liao, "Dependency-Based Search for Connect6", The International Conference on Computers and Games (CG 2013), Yokohama, Japan, August 2013. (Best Paper Award)
1. Ji-Hong Zheng, Chia-Yun Hu, I-Chen Wu, Wen-Jie Tseng, Ching-Hsuan Wei, Hung-Hsuan Lin, Chieh-Min Chang, Hao-Hua Kang, Hsiu-Chuan Lin, "Connect6 Programs on Mobile Devices", the 2012 Conference on Technologies and Applications of Artificial Intelligence (TAAI 2012), Tainan, Taiwan, November 2012. (Excellent Demo Award)
1. I-Chen Wu, Yi-Shan Lin, Hsin-Ti Tsai and Ping-Hung Lin, "The Man-Machine Connect6 Championship 2011", ICGA Journal (SCI), vol. 34, no. 2, June 2011.
1. I-Chen Wu, Hsin-Ti Tsai, Hung-Hsuan Lin, Yi-Shan Lin, Chieh-Min Chang, Ping-Hung Lin, "Temporal Difference Learning for Connect6", The 13th Advances in Computer Games Conference (ACG 13), Tilburg, The Netherlands, 20-22 November 2011.
1. I-Chen Wu, H.-H. Lin, P.-H. Lin, D.-J. Sun, Y.-C. Chan and B.-T. Chen, "Job-Level Proof-Number Search for Connect6", The International Conference on Computers and Games (CG 2010), Kanazawa, Japan, September 2010.

---

## Competition Summary

### Computer Competitions</h3>

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2013</td>
<td>Computer Olympiad</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2010</td>
<td>Computer Olympiad</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2008</td>
<td>Computer Olympiad</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2010-2014</td>
<td>TAAI computer game tournaments</td>
<td>All 1st place (Gold)</td>
</tr>
<tr>
<td>2011-2015</td>
<td>TCGA computer game tournaments</td>
<td>All 1st place (Gold)</td>
</tr>
</tbody></table>
<h3>Human Competitions</h3>
<table border="1">
<tbody><tr>
<th>Year</th>
<th>Competitions</th>
<th>Human</th>
<th>Result</th>
</tr>
<tr>
<td>2011</td>
<td>The third annual Man-Machine Connect6 Contest</td>
<td>Top human players in Taiwan</td>
<td>Won 5 and lost 3</td>
</tr>
<tr>
<td>2008</td>
<td>The first annual Man-Machine Connect6 Contest</td>
<td>Top human players in Taiwan</td>
<td>Won 11 and lost 1</td>
</tr>
<tr>
<td>2009</td>
<td>The second annual Man-Machine Connect6 Contest</td>
<td>Top human players in Taiwan</td>
<td>Won 8 and lost nothing</td>
</tr>
<tr>
<td>2009-2015(now)</td>
<td><a href="http://littlegolem.net/jsp/games/gamedetail.jsp?gtid=connect6&page=ch">Littlegolem Connect6 Championships</a></td>
<td>Top online human players all over the world</td>
<td>Won 9 champions out of 13 championships (from #7-#19) with names, "lomaben" and "Happy6". </td>
</tr>
</tbody>
</table>


</body></html>
