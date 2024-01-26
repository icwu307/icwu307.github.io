# Introduction to Nonogram Programs Developed at CGI Lab

This page introduces the history of Nonogram programs, mainly LalaFrogKK, developed in [Computer Games and Intelligence (CGI) Lab][cgi_lab], led by Professor [I-Chen Wu][icwu], at [Department of Computer Science][nctu_cs], National Chiao Tung University, Taiwan. The program LalaFrogKK won ALL the Computer Nonogram tournaments that we participated. This page also wants to acknowledge all the contributors involved in the development.

- [Early design of Nonogram programs (2010-2011)](#early-design-of-nonogram-programs-2010-2011-)
- [The core design of LalaFrogKK (2011-2013)](#the-core-design-of-lalafrogkk-2011-2013-)

---

## Early design of Nonogram programs (2010-2011)

Nonograms as well as other puzzle games were chosen as projects in the course, Theory of Computer Games, taught by Professor [I-Chen Wu][icwu] in 2010. Some strong programs were written by Hung-Hsuan Lin (林宏軒), Ching-Hua Kuo (郭青樺), and Kan-Yueh Chen (陳干越). They used different kinds of heuristics.

### Authors

<table>
<tbody>
<tr>
<td>Hung-Hsuan Lin (林宏軒)</td>
<td>2010-2011</td>
<td>Wrote a program named HappyNono.</td>
</tr>
<tr>
<td>Ching-Hua Kuo (郭青樺)</td>
<td>2010-2011</td>
<td>Wrote a program named NonoFrog.</td>
</tr>
<tr>
<td>Kan-Yueh Chen (陳干越)</td>
<td>2010-2011</td>
<td>Wrote a program named NonoLala.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2010-2011</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Competitions

The following two competitions were conducted in a two-player-game manner as described in [the document (in Chinese)](https://docs.google.com/document/d/11cB6-YOGf3aeAcTSi9Z4QaEbpAphvlel_RS1baupn4M/edit?hl=zh_TW). In breif, all participants genereates 100 puzzles. Each participant solves all other participants' puzzles. Among two participants, the one solves more puzzles wins.

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2010</td>
<td>TAAI computer game tournaments</td>
<td>1st, 2nd, 3rd</td>
</tr>
<tr>
<td>2011</td>
<td>TCGA computer game tournaments</td>
<td>2nd, 3rd</td>
</tr>
</tbody>
</table>

Note: the winner of TCGA 2011 was Naughty by Kuang-Che Wu, who was a senior engineer in Google Taiwan.

---

## The core design of LalaFrogKK (2011-2013)

After being beaten by Naughty, Kan-Yueh Chen (陳干越), Ching-Hua Kuo (郭青樺) and Hao-Hua Kang (康皓華) coworked and redesigned a new program, named LalaFrogKK (named after their nicknames, Lala, Frog, and KK). Then, Der-Johng Sun (孫德中) wrote a paper about it and modified it following the paper, which was written and published in IEEE Transactions on CIAIG (see below). The program had won all the champions of all Computer Olympiad/TAAI/TCGA Nonogram tournaments, since TAAI 2011 and till Computer Olympiad 2015. The program participated in the tournaments is now available openly at [GitHub](https://github.com/CGI-LAB/Nonogram).

### Authors

<table>
<tbody>
<tr>
<td>Kan-Yueh Chen (陳干越)</td>
<td>2011-2012</td>
<td>Wrote LalaFrogKK.</td>
</tr>
<tr>
<td>Ching-Hua Kuo (郭青樺)</td>
<td>2011-2012</td>
<td>Wrote LalaFrogKK.</td>
</tr>
<tr>
<td>Hao-Hua Kang (康皓華)</td>
<td>2011-2012</td>
<td>Wrote LalaFrogKK.</td>
</tr>
<tr>
<td>Der-Johng Sun (孫德中)</td>
<td>2012-2013</td>
<td>Wrote a paper about it and modified the program following the paper.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2011-2013</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- Fast dynamic programming (DP) method for line solving.
- Fully probing (FP) methods to solve more pixels before running backtracking.
- Backtracking.

### Competitions

Two kinds of nonogram tournaments were held in TAAI 2011. One is described as [the above](#competitions). The other is Nonogram solver as described in [the document (in Chinese)](https://docs.google.com/document/d/1mU9p_7KQXXVtTiG8sETURsIUAH1CN1-2uDoJ8iDFvpA/edit?hl=zh_TW). In breif, all participants solve the same set of 1,000 puzzles provided by tournament organizer. The program solves the most puzzles wins. After TAAI 2011, only [nonogram solver](https://docs.google.com/document/d/1mU9p_7KQXXVtTiG8sETURsIUAH1CN1-2uDoJ8iDFvpA/edit?hl=zh_TW) tournaments remained.

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2015</td>
<td>Computer Olympiad (Solver)</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2013</td>
<td>Computer Olympiad (Solver)</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2013-2014</td>
<td>TAAI computer game tournaments (Solver)</td>
<td>All 1st place (Gold)</td>
</tr>
<tr>
<td>2012-2015</td>
<td>TCGA computer game tournaments (Solver)</td>
<td>All 1st place (Gold)</td>
</tr>
<tr>
<td>2011</td>
<td>TAAI Nonograms</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2011</td>
<td>TAAI Nonogram Solver</td>
<td>1st place (Gold)</td>
</tr>
</tbody>
</table>

- TAAI 2012 did not include Nonogram tournaments.

### Publications

1. I-Chen Wu, Der-Johng Sun, Lung-Ping Chen, Kan-Yueh Chen, Ching-Hua Kuo, Hao-Hua Kang, and Hung-Hsuan Lin, "An Efficient Approach to Solving Nonograms", the IEEE Transactions on Computational Intelligence and AI in Games (SCI), Vol. 5, No. 3, pp. 251-264, September 2013.
1. Der-Johng Sun, Kuang-Che Wu, I-Chen Wu, Shi-Jim Yen, and Kuo-Yuan Kao, "Nonogram Tournaments in TAAI 2011", ICGA Journal, Vol. 35, No. 2, pp. 120-123, 2012
1. TCGA 2015 Nonogram Tournament Result, <http://aigames.nctu.edu.tw/~hsuehch/nonogram/tcga2015/>
1. TAAI 2014 Nonogram Tournament Result, <http://aigames.nctu.edu.tw/~hsuehch/nonogram/taai2014/>
1. TCGA 2014 Nonogram Tournament Result, <http://aigames.nctu.edu.tw/~mike79212001/nonogram/tcga2014/>
1. TAAI 2013 Nonogram Tournament Results, <http://aigames.nctu.edu.tw/~mike79212001/nonogram/TAAI2013/>
1. TCGA 2013 Nonogram Tournament Result, <http://aigames.nctu.edu.tw/~mike79212001/nonogram/tcga2013/>
1. TCGA 2012 Nonogram Tournament Result, <http://aigames.nctu.edu.tw/~mike79212001/nonogram/tcga2012/>

[icwu]: ..
[cgi_lab]: http://www.aigames.nctu.edu.tw/
[nctu_cs]: https://www.cs.nctu.edu.tw/cswebsite/
