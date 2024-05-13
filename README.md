<h1 align="center"><b><img align="center" alt="Coding" width="65" src="https://github.com/BIB-HACKER/Cricket-Fever---Born-of-New-IPL-Team/blob/main/Logo.png">&nbsp;&nbsp;&nbsp;Project :  NEW IPL TEAM  </b></h1>     

<p align="center">
  <img src="https://github.com/BIB-HACKER/Cricket-Fever---Born-of-New-IPL-Team/blob/main/InShot_20240511_171603299.jpg" width="400" />
  <img src="https://github.com/BIB-HACKER/Cricket-Fever---Born-of-New-IPL-Team/blob/main/preview-01.jpeg.jpg" width="400" height="400" style="float:right"/>
</p>


# Introduction
Welcome to the New IPL Team Analysis project! In this project, we’ll explore data related to the Indian Premier League (IPL) using various sources. Our goal is to gain insights into player statistics, team performance, and social media presence. Let’s dive in!

# Table of Contents
## 1.  <a href="https://jupyter.org/" target="_blank" rel="noreferrer"> <img src="https://github.com/devicons/devicon/blob/master/icons/jupyter/jupyter-original.svg" alt="jupyter" width="25" height="25"/> </a>	Data Collection
We’ll scrape data from the following sources:
IPL Official Website(https://www.iplt20.com/),
Cricket Influencers on Feedspot(https://influencers.feedspot.com/cricket_instagram_influencers/),
Kaggle(https://www.kaggle.com/code/ashwinshetgaonkar/ipl-batting-analysis-2008-2021/input),
Howzat Blog: Which Indian T20 League Team Has Most Fans?(https://www.howzat.com/blog/cricket/which-indian-t20-league-team-has-most-fans),
We’ll show the tools used for data scraping.
<p float="left">
  <img src="https://github.com/BIB-HACKER/Cricket-Fever---Born-of-New-IPL-Team/blob/main/Screenshot%202024-05-13%20105753.png" width="400" height="430"/>
  <img src="https://github.com/BIB-HACKER/Cricket-Fever---Born-of-New-IPL-Team/blob/main/Screenshot%202024-05-13%20105914.png" width="400" height="430" style="float:right"/>
</p>

## 2.	<a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> Creating Schema
We’ve designed the schema using Miro. Below is a screenshot of the schema: !Schema Design
Integration of Python scripts with SQL:
We’ll explain how Python scripts interact with our SQL database.

#### Schema
![image](https://github.com/BIB-HACKER/Cricket-Fever---Born-of-New-IPL-Team/blob/main/Screenshot%20(24).png)

## 3. 📊	Table Descriptions
Let’s break down the tables and their columns:<br>
PlayerName: Name of the player (datatype: string)
Current Team: The team the player currently represents (datatype: string)
Nationality: Player’s nationality (datatype: string)
And ETC.

#### Players Table
| Name              | Type        | Nationality | Team | Sum of RUNS | Sum of MAT | Sum of INNS | Sum of HS | Sum of 4S | Sum of 6S | Sum of 50s | Sum of 100s | Sum of Wkts | Average of RunsConceded | Sum of MAT | Sum of INNS | Average of Econ | Sum of Overs | Sum of 4w |
|-------------------|-------------|-------------|------|-------------|------------|-------------|-----------|------------|------------|-------------|--------------|--------------|--------------------------|------------|-------------|-----------------|--------------|------------|
| Arshdeep Singh   | Bowler      | Indian      | PBKS | 25          | 48         | 11          | 13        | 3          | 0          | 0           | 0            | 54           | 359.5                    | 48         | 48          | 8.61            | 166          | 1          |
| Glenn Maxwell    | Australian  | NAN         | RCB  | 1322        | 55         | 52          | 242       | 117        | 67         | 12          | 0            | 15           | 140.75                   | 55         | 30          | 8.11            | 71           | 0          |
| Hardik Pandya    | All-Rounder | Indian      | GT   | 1241        | 57         | 54          | 253       | 100        | 57         | 7           | 0            | 11           | 225                      | 31         | 21          | 8.19            | 55           | 0          |
| Jasprit Bumrah   | Bowler      | Indian      | MI   | 21          | 29         | 8           | 10        | 2          | 0          | 0           | 0            | 63           | 399                      | 43         | 43          | 7.12            | 168          | 2          |
| Kagiso Rabada    | Bowler      | Overseas    | PBKS | 117         | 45         | 19          | 49        | 11         | 4          | 0           | 0            | 75           | 410.5                    | 51         | 51          | 8.75            | 192          | 4          |
| KL Rahul         | Wicket-Keeper | Indian    | PBKS | 1296        | 27         | 27          | 230       | 106        | 53         | 11          | 1            | NAN          | NAN                      | NAN        | NAN         | NAN             | NAN          | NAN        |
| Mohammad Shami   | Bowler      | Indian      | GT   | 20          | 45         | 9           | 16        | 1          | 0          | 0           | 0            | 87           | 466.25                   | 61         | 61          | 8.02            | 231          | 2          |
| Pat Cummins      | All-Rounder | Overseas    | KKR  | 302         | 26         | 21          | 175       | 19         | 22         | 3           | 0            | 28           | 286                      | 26         | 26          | 9.12            | 99           | 1          |
| Ravi Bishnoi     | NAN         | NAN         | LSG  | 28          | 38         | 11          | 12        | 2          | 0          | 0           | 0            | 53           | 361.25                   | 52         | 51          | 7.47            | 190          | 0          |
| Ravindra Jadeja  | All-Rounder | Indian      | CSK  | 765         | 56         | 45          | 163       | 58         | 34         | 2           | 0            | 44           | 335.75                   | 56         | 55          | 7.72            | 175          | 0          |
| Rishabh Pant     | Wicket-Keeper | Indian    | DC   | 1102        | 44         | 43          | 158       | 108        | 35         | 4           | 0            | NAN          | NAN                      | NAN        | NAN         | NAN             | NAN          | NAN        |
| Rohit Sharma     | Batsman     | Indian      | MI   | 1313        | 55         | 55          | 256       | 123        | 63         | 6           | 0            | NAN          | NAN                      | NAN        | NAN         | NAN             | NAN          | NAN        |
| Ruturaj Gaikwad  | NAN         | NAN         | CSK  | 368         | 14         | 14          | 99        | 33         | 14         | 3           | 0            | NAN          | NAN                      | NAN        | NAN         | NAN             | NAN          | NAN        |
| Shreyas Iyer     | Batsman     | Indian      | KKR  | 1095        | 39         | 39          | 220       | 88         | 32         | 6           | 0            | NAN          | NAN                      | NAN        | NAN         | NAN             | NAN          | NAN        |
| Suryakumar Yadav | Batsman     | Indian      | MI   | 1705        | 54         | 53          | 332       | 189        | 65         | 14          | 1            | NAN          | NAN                      | NAN        | NAN         | NAN             | NAN          | NAN        |
| Trent Boult      | Bowler      | Overseas    | RR   | 57          | 55         | 17          | 33        | 3          | 2          | 0           | 0            | 67           | 416.75                   | 55         | 55          | 8               | 208          | 1          |
| Virat Kohli      | Batsman     | Indian      | RCB  | 1851        | 60         | 60          | 336       | 163        | 44         | 14          | 2            | NAN          | NAN                      | NAN        | NAN         | NAN             | NAN          | NAN        |
| Yuzvendra Chahal | Bowler      | Indian      | RR   | 16          | 47         | 6           | 14        | 0          | 0          | 0           | 0            | 87           | 434.5                    | 61



## 4.	<a href="https://powerbi.microsoft.com/en-us/desktop/" target="_blank" rel="noreferrer"> <img src="https://github.com/microsoft/PowerBI-Icons/blob/main/PNG/Power-BI.png" alt="Power-BI" width="25" height="35"/> </a> Dashboard (Power BI)
We’ve created an interactive dashboard using Power BI. Here’s a screenshot: !Power BI Dashboard
Analysis:
We’ll discuss key insights and visualizations from the dashboard.
Final Player List:
We’ll provide the list of players based on our analysis.
#### Batting

![image](https://github.com/BIB-HACKER/Cricket-Fever---Born-of-New-IPL-Team/blob/main/Screenshot%202024-05-12%20202506.png)
#### Bowling
![image](https://github.com/BIB-HACKER/Cricket-Fever---Born-of-New-IPL-Team/blob/main/Screenshot%202024-05-12%20202534.png)

<h1 align="center"><b> THANK YOU </b> </h1>
