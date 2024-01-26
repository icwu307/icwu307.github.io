# Introduction to NoGo Programs Developed at CGI Lab

This page introduces the history of NoGo programs developed in [Computer Games and Intelligence (CGI) Lab][cgi_lab], led by Professor [I-Chen Wu][icwu], at [Department of Computer Science][nctu_cs], National Chiao Tung University, Taiwan. The main contributor for the NoGo programs is Po-Hsuan She (佘博玄); other contributors are also acknowledged on this page.

NoGo is a variant of Go, with the difference being that no players are allowed to capture pieces or commit suicide. The first player that is unable to play without breaking these two rules loses. A very brief history of the game and early competitions can be read [here](https://webdocs.cs.ualberta.ca/~mmueller/nogo/history.html) (by Martin Müller).

Our current program, HappyNoGo, has consistently won the gold medal in competitions, including the Computer Olympiad.

- PSABR (2010-2011)
- PohsuanNoGo (2011-2012)
- HappyNoGo (2012-)

---

## PSABR (2010-2011)

NoGo was assigned as the term project for the course “Theory of Computer Games” in the fall semester of 2010. Students were then encouraged to register for the [TAAI 2011](http://aigames.nctu.edu.tw/TAAI2011/eng/) competition using their course projects. Of these participants, PSABR and MoonGo received the silver and bronze medals, respectively.

The first place program was Coldmilk, written by [Cheng-Wei Chou](http://www.coldmilk.tw/Eng/Results.aspx) (National Dong Hwa University, Taiwan).

While PSABR is not directly related to the current program in terms of features, it served as the spring board for future NoGo Program development at CGI lab.

The sole author of the program is Po-Hsuan She; the main search engine uses alpha-beta search.

### Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2011</td>
<td>TAAI NoGo</td>
<td>2nd place (Silver)</td>
</tr>
</tbody>
</table>

---

## PohsuanNoGo (2011-2012)

Po-Hsuan She then improved his NoGo program by incorporating MCTS and RAVE. This new program, named PohsuanNoGo, went on to place second in the [TCGA 2012](http://tcga.ndhu.edu.tw/TCGA2012/eng/) competition. The report can be accessed [here](http://tcga.ndhu.edu.tw/TCGA2012/Result/TCGA2012_NoGo.pdf). The undefeated champion at the time was [BobNoGo](https://webdocs.cs.ualberta.ca/~mmueller/nogo/BobNoGo.html), developed by Bob Hearn and Martin Müller.

### Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2012</td>
<td>TCGA NoGo</td>
<td>2nd place (Silver)</td>
</tr>
<tr>
<td>2013</td>
<td>17th Computer Olympiad</td>
<td>2nd place (Silver)</td>
</tr>
</tbody>
</table>

---

## HappyNoGo (2012-)

Later in the same year, Po-Hsuan She worked with Ting-Fu Liao (廖挺富) to incorporate elements of Liao’s general framework for parallel MCTS and Li-Cheng Lan (藍立呈) also joined to assist in some code design. This program was named HappyNoGo, after our Go program at the time, [HappyGo](CGI.html#happygo-2008-2011-). HappyNoGo was able to run in parallel, which greatly increased its playing strength.

### Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2012</td>
<td>TAAI NoGo</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2013</td>
<td><b>17th Computer Olympiad NoGo</b></td>
<td><b>1st place (Gold)</b></td>
</tr>
<tr>
<td>2014</td>
<td>TAAI NoGo</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2015</td>
<td>TCGA NoGo</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2015</td>
<td>18th Computer Olympiad NoGo</td>
<td>1st place (Gold)</td>
</tr>
<tr>
<td>2015</td>
<td>TAAI NoGo</td>
<td>1st place (Gold)</td>
</tr>
</tbody>
</table>
	
Most notably, HappyNoGo and the improved single-threaded PohsuanNoGo were both able to defeat BobNoGo for the 17th Computer Olympiad (2013) in Yokohama, Japan.

[icwu]: ..
[cgi_lab]: http://www.aigames.nctu.edu.tw/
[nctu_cs]: https://www.cs.nctu.edu.tw/cswebsite/
