# Introduction to Go Programs Developed at CGI Lab

This page introduces the history of Go programs developed in [Computer Games and Intelligence (CGI) Lab][cgi_lab], led by Professor [I-Chen Wu][icwu], at [Department of Computer Science][nctu_cs], National Chiao Tung University, Taiwan; and also acknowledges the contributors who are/were the members of the CGI lab, unless specified explicitly.

- [HappyGo (2008-2011)](#happygo-2008-2011-)
- [Amigo (2012-2014)](#amigo-2012-2014-)
- [CGI Go Intelligence (abbr. CGI) 1.0 (2015.01-2015.12)](#cgi-1-0-2015-1-2015-12-)
- [CGI 2.0 or Deep CGI (2015.12-2016.08)](#cgi-2-0-2015-12-2016-8-)
- [CGI 3.0 (2016.08-)](#cgi-3-0-2016-8-)

For the current strength of CGI, see KGS account "[CGI](http://www.gokgs.com/graphPage.jsp?user=CGI)".

---

## HappyGo (2008-2011)

One year before 2008, Yung-Ler Wang (王永樂) wrote a simple version of Go program, named HappyGo, since his nickname was Happy. Although the program was completely rewritten after 2008 by the following authors, we still used the name HappyGo. Note that we focused on 9x9 Go in this version.

### Authors

<table>
<tbody>
<tr>
<td>Chun-Yi Chen (陳俊嶧)</td>
<td>2008-2010</td>
<td>Wrote most of the code of HappyGo, including Monte-Carlo Tree Search (MCTS) and many heuristics.</td>
</tr>
<tr>
<td>Tsun-Tao Tso (左存道)</td>
<td>2011-2012</td>
<td>Wrote a solver inside HappyGo, including the design of relevance zones.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2008-2012</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- Mainly implemented Monte Carlo Tree Search and lots of heuristics from Go knowledge (designed manually, not based on any machine learning methods). The code for playouts was rule-based.
- Run in single thread only (surely without any distributed computing) and for Go 9x9 only.

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
<td>TCGA Go 9x9</td>
<td>2nd place (Silver)</td>
</tr>
<tr>
<td>2011</td>
<td>TAAI Go 9x9</td>
<td>5th place</td>
</tr>
<tr>
<td>2010</td>
<td>TAAI Go 9x9</td>
<td>2nd place (Silver)</td>
</tr>
<tr>
<td>2010</td>
<td>ICGA Go 9x9</td>
<td>8th place</td>
</tr>
<tr>
<td>2009</td>
<td>TAAI Go 9x9</td>
<td>4th place</td>
</tr>
</tbody>
</table>

### Publications

1. Chun-Yi Chen, "A Design of Monte-Carlo Computer Go Program", M.S. thesis, National Chiao Tung University, Hsinchu, Taiwan, 2010.
1. Tsun-Tao Tso, "A Study of Solving Life and Death Problem for 7x7 Kill-All Go", M.S. thesis, National Chiao Tung University, Hsinchu, Taiwan, 2012.

---

## Amigo (2012-2014)

Ting-Fu Liao rewrote the whole Go program that contains a general framework for parallel Monte Carlo Tree Search, which can be used for other games, like Chinese dark chess, NoGo. For generality, the initial version of Amigo by Ting-Fu Liao contained not much Go-specific code, except that it followed the rule-based playouts of HappyGo partially. Note that we still focused on 9x9 Go in this version, but it works for 19x19 due to generality (but very weak). So, we can say that 19x19 had not been developed in this stage.

### Authors

<table>
<tbody>
<tr>
<td>Ting-Fu Liao (廖挺富)</td>
<td>2011-2013</td>
<td>Wrote general framework for parallel Monte Carlo Tree Search, it can be use in any game.</td>
</tr>
<tr>
<td>Ting-Chu Ho (何庭築)</td>
<td>2012-2014</td>
<td>Assisted on Go-specific knowledge like connection.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2011-2014</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- A general framework for parallel Monte Carlo Tree Search. (By Ting-Fu Liao)
- Support distributed and multi-thread computing.

### Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2014</td>
<td>TAAI Go 9x9</td>
<td>2nd place (Silver)</td>
</tr>
<tr>
<td>2014</td>
<td>TCGA Go 9x9</td>
<td>2nd place (Silver)</td>
</tr>
<tr>
<td>2013</td>
<td>ICGA Go 9x9</td>
<td>3rd place (Bronze)</td>
</tr>
<tr>
<td>2013</td>
<td>TCGA Go 9x9</td>
<td>3rd place (Bronze)</td>
</tr>
</tbody>
</table>

### Publications

1. Ting-Fu Liao, "Software Framework for Parallel Monte Carlo Tree Search", M.S. thesis, National Chiao Tung University, Hsinchu, Taiwan, 2013.
1. Ting-Chu Ho, "The Study of Connections for Computer Go", M.S. thesis, National Chiao Tung University, Hsinchu, Taiwan, 2014.
1. Ting-Fu Liao, I-Chen Wu, Guan-Wun Chen, Chung-Chin Shih, Po-Ya Kang, Bing-Tsung Chiang, Ting-Chu Ho and Ti-Rong Wu, "A Study of Software Framework for Parallel Monte Carlo Tree Search," the 19th Game Programming Workshop (GPW-2014), Hakone Seminar House, Kanagawa, Japan, November 7-9, 2014.

---

## CGI 1.0 (2015.1-2015.12)

Since Amigo had name conflict with an old Go program, it was renamed to **CGI Go Intelligence** (abbr. **CGI**, a kind of recursive acronym). The program was not changed until Ti-Rong Wu (the key developer) as well as some authors (see below) made significant changes in the Go side on top of the framework in 2015. So, CGI is usually referred to the changed version starting from 2015. Since some machine learning methods like M&M were incorporated, the program started working reasonably for 19x19 and the strength grows to 2d or so.

### Authors

<table>
<tbody>
<tr>
<td>Ti-Rong Wu (吳廸融)</td>
<td>2015-current</td>
<td>Made most significant changes and improvements over Amigo (nearly rewrote the code in the Go side) , mainly including the tuning of pattern features by machine learning method and many detailed work. (The key developer of this CGI version)</td>
</tr>
<tbody>
<tr>
<td>Ting-Fu Liao (廖挺富)</td>
<td>2011-2013</td>
<td>Wrote general framework for parallel Monte Carlo Tree Search, which this version is still based on.</td>
</tr>
<tr>
<td>Guan-Wen Chen (陳冠文)</td>
<td>2015-current</td>
<td>Worked on distributed computing, handling server and worker synchronization.</td>
</tr>
<tr>
<td>Chung-Chin Shih (施仲晉)</td>
<td>2015-current</td>
<td>Assisted on the implementation of some patterns. To implement knowledges like life and death in Go, also used in KillAll Go.</td>
</tr>
<tr>
<td>Li-Cheng Lan (藍立呈)</td>
<td>2015-current</td>
<td>Assisted on MCTS including dynamic komi, argument tuning.</td>
</tr>
<tr>
<td>Kun-Hao Yeh (葉騉豪)</td>
<td>2015-current</td>
<td>To build Go 9x9 opening book by Job-Level System.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2015-current</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- Follow the framework of Amigo, but make a significant change (nearly rewrite) as follows.
- Use machine learning skill to train lots of pattern feature, human made knowledge.
- Use some technique like progressive bias, progressive widening, dynamic komi to improve MCTS.

### Competitions

#### Human Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions (19x19)</th>
<th>Human (White)</th>
<th>Rule</th>
<th>Result</th>
</tr>
<tr>
<td>2015</td>
<td>IEEE CIG 2015 Go</td>
<td>Chun-Hsun Chou 9p <br>(周俊勳 職業九段)</td>
<td>H6, komi: 0.5, 45 minutes each</td>
<td>Lose (W+5.5)</td>
</tr>
<tr>
<td>2015</td>
<td>IEEE CIG 2015 Go</td>
<td>Kai-Hsin Chang 5p <br>(張凱馨 職業五段)</td>
<td>H6, komi: 0.5, 45 minutes each</td>
<td>Lose (W+Res)</td>
</tr>
<tr>
<td>2015</td>
<td>IEEE CIG 2015 Go</td>
<td>Li-Chun Yu 1p <br>(俞俐均 職業一段)</td>
<td>H6, komi: 0.5, 45 minutes each</td>
<td>Win (B+Res)</td>
</tr>
</tbody>
</table>

#### Computer Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Place</th>
</tr>
<tr>
<td>2015</td>
<td>ICGA Go 19x19</td>
<td>4th place</td>
</tr>
<tr>
<td>2015</td>
<td>ICGA Go 13x13</td>
<td>4th place</td>
</tr>
<tr>
<td>2015</td>
<td>ICGA Go 9x9</td>
<td>3rd place (Bronze)</td>
</tr>
<tr>
<td>2015</td>
<td>TCGA Go 19x19</td>
<td><b>1st place (Gold)</b></td>
</tr>
<tr>
<td>2015</td>
<td>TCGA Go 13x13</td>
<td><b>1st place (Gold)</b></td>
</tr>
<tr>
<td>2015</td>
<td>TCGA Go 9x9</td>
<td><b>1st place (Gold)</b></td>
</tr>
</tbody>
</table>

(Note: TCGA refers to Taiwan Computer Game Association (台灣電腦對局學會), which hosts competitions every year.)

---

## CGI 2.0 (2015.12-2016.8)

As of Dec 2015, we started incorporating Deep Convolutional Neural Network (DCNN) or so-called Deep Learning into CGI, which is called CGI 2.0 or Deep CGI for convenience. Here, we would like to thank and acknowledge Detlef Schmicker for sharing his DCNN data set (with 54% prediction rate), which was used as our initial DCNN data set, though we changed to our own training data in mid-Jan 2016. The following list simply shows the persons involved in this project and is subject to change (Note: Ti-Rong Wu, Li-Cheng Lan, and Guan-Wen Chen are three key developers in the current project).

### Authors

<table>
<tbody>
<tr>
<td>Ti-Rong Wu (吳廸融)</td>
<td>2015-current</td>
<td>Made most significant changes and improvements over CGI 1.0, and also worked on DCNN.</td>
</tr>
<tr>
<td>Li-Cheng Lan (藍立呈)</td>
<td>2015-current</td>
<td>Worked on the DCNN architecture, mainly for multi-GPU versions.</td>
</tr>
<tr>
<td>Guan-Wen Chen (陳冠文)</td>
<td>2015-current</td>
<td>Worked on DCNN training.</td>
</tr>
<tr>
<td>Hung-Chun Wu (吳宏君)</td>
<td>2016-current</td>
<td>Assisted on DCNN.</td>
</tr>
<tr>
<td>Jin-Bo Huang (黃勁博)</td>
<td>2016-current</td>
<td>Assisted on DCNN.</td>
</tr>
<tr>
<td>Ting-Fu Liao (廖挺富)</td>
<td>2011-2013</td>
<td>the code he wrote for general parallel MCTS framework is still used in this version.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2015-current</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- Supervised Learning (SL) policy network, but no Reinforcement Learning (RL) policy network and Value Network (VN) yet.

### Competitions

#### Computer Competitions

<table>
<tbody>
<tr>
<th>2016</th>
<th>UEC Cup (19x19 Go)</th>
<th>Rank</th>
</tr>
<tr>
<td>Day 1 (Preliminary League)</td>
<td>All wins for 7 games (including Zen, Ray etc.)</td>
<td>1st place</td>
</tr>
<tr>
<td>Day 2 (Final Tournament)</td>
<td>Won 2 and lost 2 <br>(Also won the best student award.)</td>
<td>6th place</td>
</tr>
</tbody>
</table>

#### Human Competitions

<table>
<tbody>
<tr>
<th>Year</th>
<th>Competitions</th>
<th>Human (White)</th>
<th>Rule</th>
<th>Result</th>
</tr>
<tr>
<td>2016</td>
<td>IEEE WCCI 2016 Go</td>
<td>Chun-Hsun Chou 9p <br>(周俊勳 職業九段)</td>
<td>H2, komi: 6.5, 45 minutes each</td>
<td>Lose</td>
</tr>
</tbody>
</table>

---

## CGI 3.0 (2016.8-)

As of Aug. 2016, we start the CGI 3.0 project, mainly developing value network (VN), and some other DCNNs, like RL policy network.

As of Dec 2015, we started incorporating Deep Convolutional Neural Network (DCNN) or so-called Deep Learning into CGI, which is called CGI 2.0 or Deep CGI for convenience. This version is still being developed. Here, we would like to thank and acknowledge Detlef Schmicker for sharing his DCNN data set (with 54% prediction rate), which was used as our initial DCNN data set, though we changed to our own training data in mid-Jan 2016. The strength of this version grows significantly, but it is still unknown and not final yet, since the project is still ongoing now. The following list simply shows the persons involved in the Deep CGI project and is subject to change (Note: Ti-Rong Wu, Li-Cheng Lan, and Guan-Wen Chen are three key developers in the current project).

### Authors

<table>
<tbody>
<tr>
<td>Ti-Rong Wu (吳廸融)</td>
<td>2015-current</td>
<td>Made most significant changes and improvements over CGI 1.0, and also worked on DCNN.</td>
</tr>
<tr>
<td>Guan-Wen Chen (陳冠文)</td>
<td>2015-current</td>
<td>Worked on distributed computing.</td>
</tr>
<tr>
<td>Hung-Chun Wu (吳宏君)</td>
<td>2016-current</td>
<td>Worked on DCNN training.</td>
</tr>
<tr>
<td>Dong-Yi Lai (賴東億)</td>
<td>2016-current</td>
<td>Worked on DCNN training.</td>
</tr>
<tr>
<td>Peter Wu (吳慈仁)</td>
<td>Current</td>
<td>To help customization.</td>
</tr>
<tr>
<td>Some more</td>
<td>Current</td>
<td>To help the development.</td>
</tr>
<tr>
<td>I-Chen Wu (吳毅成)</td>
<td>2015-current</td>
<td>Supervised the whole project.</td>
</tr>
</tbody>
</table>

### Features

- Supervised Learning (SL) policy network
- Reinforcement Learning (RL) policy network
- Value Network (VN)
- Rollout improvement (using simulation balancing)
- Distributed computing

### Competitions

#### Computer Competitions

- 2017 UEC Cup, held in Tokyo, Japan, March 2017.
  <table>
  <tbody><tr>
  <th>Days </th>
  <th>Description </th>
  <th>Rank</th>
  </tr>
  <tr>
  <td>Day 1 (Preliminary)</td>
  <td>Won 2 and lost 2 </td>
  <td>6th place</td>
  </tr>
  <tr>
  <td>Day 2 (Final)</td>
  <td>Won 2 and lost 2</td>
  <td>7th place</td>
  </tr>
  </tbody>
  </table>
- "CITIC Securities Cup", the 1st World AI Go Open, held in Ordos, Inner Mongolia, China, August 2017.
  <table>
  <tbody>
  <tr>
  <th>Days</th>
  <th>Description</th>
  <th>Rank</th>
  </tr>
  <tr>
  <td>Day 1 (Preliminary)</td>
  <td>Won all 5 games </td>
  <td>1st place</td>
  </tr>
  <tr>
  <td>Day 2 (Final)</td>
  <td>Won 2 and lost 1<br>Price: \$RMB 100k</td>
  <td>2nd place</td>
  </tr>
  </tbody>
  </table>

#### Human Competitions

- 2017: IEEE FUZZ 2017, held in Naples, Italy, July 2017.  
  The first academic Go program beating professional 9dan player officially.
  <table>
  <tbody>
  <tr>
  <th>Year</th>
  <th>Competitions</th>
  <th>Human (White)</th>
  <th>Rule</th>
  <th>Result</th>
  </tr>
  <tr>
  <td>2017</td>
  <td>IEEE FUZZ 2017</td>
  <td>Chun-Hsun Chou 9p <br>(周俊勳 職業九段)</td>
  <td>No handicap, komi: 6.5, 45 minutes each</td>
  <td>Won two games</td>
  </tr>
  </tbody>
  </table>

### Publications

1. Ti-Rong Wu, I-Chen Wu, Guan-Wun Chen, Ting-han Wei, Tung-Yi Lai, Hung-Chun Wu, Li-Cheng Lan, "Multi-Labelled Value Networks for Computer Go", arXiv:1705.10701, 2017.

### More

- As of October 2017, this webpage is no longer maintained.
- For all who wants to get the latest information about CGI program, please go to our Facebook page: [CGI Go Intelligence](https://www.facebook.com/CGI-Go-Intelligence-1469816663064693/), or Weibo page: [CGI Go Intelligence](https://www.weibo.com/u/6367137600/home).

[icwu]: ..
[cgi_lab]: http://www.aigames.nctu.edu.tw/
[nctu_cs]: https://www.cs.nctu.edu.tw/cswebsite/
