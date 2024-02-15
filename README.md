<h1 align="center">Poppy: League of Legends analysis tool</h1>

<p align="center"> 
<a href="https://github.com/lprtk/poppy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/lprtk/poppy"></a> 
<a href="https://github.com/lprtk/poppy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/lprtk/poppy"></a> 
<a href="https://github.com/lprtk/poppy/stargazers"><img alt="Github Stars" src="https://img.shields.io/github/stars/lprtk/poppy"></a> 
<a href="https://github.com/lprtk/poppy/blob/master/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/lprtk/poppy"></a> 
<a href="https://github.com/lprtk/poppy/"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a> 
</p> 

## Table of contents 
* [Overview :loudspeaker:](#Overview)
* [Objectives :mag_right:](#Content)
* [Solution :dart:](#Content)
* [Requirements :page_with_curl:](#Requirements)
* [File details :open_file_folder:](#File-details)
* [Features :computer:](#Features)

<a id="section01"></a> 
## Overview

<p align="justify">Riot Games, through League of Legends, provides a data portal listing a large number of in-game indicators. These data are used to work on usecases such as performance evaluation in esports. But first of all, why should we be inclined to evaluate the performance of a team or player in League of Legends?<br>
As with more conventional sports, by having a set of games and statistics on a player, we want to be able to tell whether or not a game was good from a player's point of view. In other words, we want to calculate the player's performance during a game to determine who is the best player.<p>

<a id="section02"></a> 
## Objectives

<p align="justify">When we hear about statics and performance to evaluate a League of Legends player, it's always the standard metrics that are used: KDA, KP, DPM, CSPM and so on.<br>
In reality, these metrics are biased because they don't provide a detailed summary of a player's performance during a game, they reward certain styles of play more than others, and they don't cover all aspects of the game. Through this project, we have multiple objectives:</p>
<ul>
    <li>
        <p align="justify">
            Measure individual performance across the skill set of a professional professional League of Legends player.
        </p>
    </li>
    <li>
        <p align="justify">
            Develop a scouting tool for professional players to monitor individual individual performance.
        </p>
    </li>
    <li>
        <p align="justify">
            Optimize and facilitate talent identification using data-driven criteria.
        </p>
    </li>
</ul>

<a id="section03"></a> 
## Solution

<p align="justify">Our solution uses a different approach. Standard metrics can be considered, but they need to be complemented by others. In particular, by taking everything a player can do in a game: kill enemies, die or stay alive, manage his lane, farm resources, inflict damage on champions or structures/neutral objectives, mitigate/tank damage, take control of the map and vision, take decisions about his rotate, have impact in fight.<br>
By considering all this information, it is possible to compare it with a set of enemy team statistics to calculate relevant performance metrics. Comparing the metrics of the player with those of the entire enemy team enables us to measure the player's impact in relation to the whole enemy team and not in relation to his direct opponent, since if the player plays a good matchup, his metrics will be overvalued in relation to his direct opponent.</p>

<p align="justify">So the idea is to be able to evaluate a player's performance in all aspects of the game. To achieve this, our solution is:</p>
<ul>
    <li>
        <p align="justify">
            Create relevant performance indicators for each dimension of the game.
        </p>
        <ul>
            <li>
                <p align="justify">
                    Individual performance
                </p>
            </li>
            <li>
                <p align="justify">
                    Mechanical skills
                </p>
            </li>
            <li>
                <p align="justify">
                    Fighting and aggression
                </p>
            </li>
            <li>
                <p align="justify">
                    Survivability
                </p>
            </li>
            <li>
                <p align="justify">
                    Farming
                </p>
            </li>
            <li>
                <p align="justify">
                    Vision and map awarness
                </p>
            </li>
            <li>
                <p align="justify">
                    Objectives and strategy
                </p>
            </li>
            <li>
                <p align="justify">
                    Adaptability
                </p>
            </li>
        </ul>
    </li>
    <li>
        <p align="justify">
            Create a global index of individual performance comparable between players and between leagues.
        </p>
    </li>
</ul>

<a id="section04"></a> 
## Requirements
* **Python version 3.11.1** 
* **Install requirements.txt** 
```console
$ pip install -r requirements.txt 
``` 

<a id="section05"></a> 
## File details
```
- poppy
    - wrapper.py
    - __init__.py
    > api
        - config.py
        - __init__.py
    > endpoints
        - challenge.py
        - champion.py
        - item.py
        - league.py
        - match.py
        - summoner.py
        - __init__.py
        > urls
            - endpoint_urls.py
            - __init__.py
```

<a id="section06"></a> 
## Features 
<p align="center"><a href="https://github.com/lprtk/lprtk">My profil</a> • 
<a href="https://github.com/lprtk/lprtk">My GitHub</a></p>
