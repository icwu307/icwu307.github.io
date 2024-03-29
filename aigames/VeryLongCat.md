# Introduction to Mahjong Programs Developed at CGI Lab

This page introduces the history of Mahjong programs, mainly for LongCat/VeryLongCat, developed in [Computer Games and Intelligence (CGI) Lab][cgi_lab], led by Professor [I-Chen Wu][icwu], at [Department of Computer Science][nctu_cs], National Chiao Tung University, Taiwan. This page also wants to acknowledge all the contributors involved in the development.

- [LongCat](#longcat)
- [VeryLongCat](#verylongcat)
- [Ongoing](#ongoing)

---

## LongCat

Cheng-Hong Lin (林正宏) wrote a Mahjong program for his thesis on 2010. The program makes moves based on the least number of cards required to win (進聽數), or called N-to-win in this page.

### Authors

<table>
<tbody>
<tr>
<td>Cheng-Hong Lin (林正宏)</td>
<td>2010-2011</td>
<td>Whole code design</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2010-2011</td>
<td>Supervised the whole project</td>
</tr>
</tbody>
</table>

### Features

- Expectimax tree search
- Building the N-to-win table

### Publications

1. I-Chen Wu, Yi-Chang Shan, Cheng-Hung Lin and Shi-Jim Yen, "LONGCATMJ Wins in Mahjong Tournament 2011", ICGA Journal, vol. 34(3), September 2011.
1. Cheng-Hung Lin, Yi-Chang Shan, I-Chen Wu, "Tournament Framework for Computer Mahjong Competitions", The 2011 International Conference on Technologies and Applications of Artificial Intelligence (TAAI), Chungli, Taiwan, November 2011.
1. W.-J. Tseng, L.-K. Chuang, I-Chen Wu, S.-S. Lin and S.-J. Yen, "LONGCAT Wins Mahjong Tournament", ICGA Journal, Vol. 36(3), September 2013.

---

## VeryLongCat

Li-Kai Chuang (莊立楷) improved the quality and speed of searching of LongCat. The modified program is renamed to "VeryLongCat".

### Authors

<table>
<tbody>
<tr>
<td>Cheng-Hong Lin (林正宏)</td>
<td>2010-2011</td>
<td>Designed the original LongCat</td>
</tr>
<tr>
<td>Li-Kai Chuang (莊立楷)</td>
<td>2013-2015</td>
<td>Designed and implemented the improvement (major contributor for the improvement)</td>
</tr>
<tr>
<td>Shih-Chieh Tang (唐士傑)</td>
<td>2014-2015</td>
<td>Assisted the improvement</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2013-2015</td>
<td>Supervised the whole project</td>
</tr>
</tbody>
</table>

### Features

- Transposition table
- Extension of N-to-win
- Improvement of dynamic table
- More heuristics

### Publications

1. Yi-Chang Shan, Ching-Hsuan Wei, Cheng-Hung Lin, I-Chen Wu, Li-Kai Chuang, and Shi-Jie Tang, "A Framework for Computer Mahjong Competitions", ICGA Journal, Vol. 37(1), pp. 44-56, March 2014.
1. I-Chen Wu, Li-Kai Chuang, "A Study of Mahjong Program Design", the domestic track of 2015 Conference on Technologies and Applications of Artificial Intelligence(TAAI 2015), Tainan, Taiwan, November 2015.

---

## Ongoing

Our CGI lab continues to improve VeryLongCat and expect to compete with human players.

### Authors

<table>
<tbody>
<tr>
<td>Shih-Chieh Tang (唐士傑)</td>
<td>2015-current</td>
<td>Improvement of winning quality</td>
</tr>
<tr>
<td>Feng-Sheng Liao (廖峰聖)</td>
<td>2015-current</td>
<td>Improvement of defensive strategies</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2015-current</td>
<td>Supervised the whole project</td>
</tr>
</tbody>
</table>

### Publications

Not available yet.

---

## Competition Summary

### Computer Competitions

<table>
<tbody>
<tr>
<td><h4>Year</h4></td>
<td><h4>Competition</h4></td>
<td><h4>Place</h4></td>
</tr>
<tr>
<td>2013, 2015</td>
<td>Computer Olympiad</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2011, 2012, 2015</td>
<td>TAAI computer game tournaments</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2011, 2012, 2015</td>
<td>TCGA computer game tournaments</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2013, 2014</td>
<td>TAAI computer game tournaments</td>
<td>2nd place (Silver)</td>
</tr>
<tr>
<td>2014</td>
<td>TCGA computer game tournaments</td>
<td>2nd place (Silver)</td>
</tr>
</tbody>
</table>

### Human Competitions

<table>
<tbody>
<tr>
<td><h4>Year</h4></td>
<td><h4>Competition</h4></td>
<td><h4>Human</h4></td>
<td><h4>Result</h4></td>
</tr>
<tr>
<td>2014</td>
<td>TAAI Man-Machine Mahjong Demo Contest</td>
<td>李亞萍, 余筱萍</td>
<td>1st place</td>
</tr>
</tbody>
</table>

[icwu]: ..
[cgi_lab]: http://www.aigames.nctu.edu.tw/
[nctu_cs]: https://www.cs.nctu.edu.tw/cswebsite/
