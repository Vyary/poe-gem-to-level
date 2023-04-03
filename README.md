<p align=center>
    <a href="https://www.pathofexile.com/" title="Path of Exile Website">
      <img align="center" src="https://web.poecdn.com/protected/image/layout/sanctumlogo.png?v=1670373174098&key=j1DUgpyrwdlKZcGWzaFxxA" />
    </a>
</p>

<h2 align="center">Path of Exile Gem Profit</h2>

## Table of Contents
- [Introduction](#introduction)
- [Overview of Skill Gems](#overview-of-skill-gems)
- [In-Game Profit](#in-game-profit)
- [Script Functionality](#script-functionality)
- [Using the CSV Files](#using-the-csv-files)
- [CSV Files Location](#csv-file-locations)
- [CSV Files Contents](#csv-file-contents)
- [Auto-Updating Google Sheet](#auto-updating-google-sheet)

## Introduction
Path of Exile is a dark fantasy online Action RPG that offers players the chance to level up Skill Gems, which can increase in power through different levels and quality variants. Corrupting these gems using Vaal Orbs can result in a chance for them to reach level 21, significantly increasing their value.

This document provides information on a Python script that scrapes data from https://poe.ninja/ to collect gem names and prices, and calculate in-game profits.

## Overview of Skill Gems
Skill Gems, also known as Active Skill Gems, are items that provide players with new abilities when placed into an item socket. These gems come in different levels and quality variants that can increase their power. 

## In-Game Profit
In-game profit can be made by leveling Skill Gems to level 20 and selling them, or by corrupting them using Vaal Orbs to increase their value. Successfully upgrading a corrupted gem to level 21 can result in a significant increase in price, though this has a success rate of around 12%.

## Script Functionality
The Python script in question uses an API to scrape data from https://poe.ninja/. It collects gem names, gem prices, and calculates profits.

## Using the CSV Files
The CSV files generated by the script can be imported into programs such as Microsoft Excel or Google Sheets, which allow users to filter and find the best gems to level for in-game profit.

## CSV Files Location
The CSV files can be found in the output folder of this directory or accessed via [this link](https://github.com/Vyary/poe-gem-prices/blob/main/output/).

## CSV Files Contents
The gems_to_level.csv file contains the following information:
- Gem Name
- Buy price
- Leveled 20/20: Price for leveled gems
- Listed L20/20: Number of leveled gems on the market, indicating a stable price.

The gems_to_corrupt.csv file contains the following information:
- Gem Name
- Corrupted 20/20: Price for a gem that has been corrupted and failed
- Success 21/20: Price for a gem that has been corrupted and successfully upgraded, which increases the price significantly
- Listed 21/20: Number of successful 21/20 gems on the trade site, including offline offerings (note that gems with higher listing counts are more likely to have an appropriate price and provide more accurate profits).
- Vaal price: Specific to gems that have a Vaal version, the Vaal price unlocks an additional skill for the gem set.

## Auto-Updating Google Sheet
For ease of use, users can access an auto-updating Google Sheet with the latest data from the script.

**For Leveling:**
* Filter 1: This sheet includes gems with 50%-ish profit just for leveling them, they are not for corruping [click here](https://docs.google.com/spreadsheets/d/1qcYu22DIwEORUYuTJNnYnxS5ceQx8y6XJhVjBai_0lI/edit#gid=1128179025&fvid=2016462890)

**For Corrupting:**
* Filter 1: Good for league start with buy price under 20, 50%-ish profit if it fails, sell price for success is set to be more than 100 and only show gems with 10 or more listings [click here](https://docs.google.com/spreadsheets/d/1qcYu22DIwEORUYuTJNnYnxS5ceQx8y6XJhVjBai_0lI/edit#gid=520131547&fvid=434671070)

* Filter 2: Great for mid-late league with buy price under 100, 50%-ish profit if it fails, sell price for success is set to be more than 200 and only show gems with 10 or more listings [click here](https://docs.google.com/spreadsheets/d/1qcYu22DIwEORUYuTJNnYnxS5ceQx8y6XJhVjBai_0lI/edit#gid=520131547&fvid=1816347774)

* Filter 3: Has the same settings as Filter 2 but includes awakened gems but keep in mind they take longer to level. Good if you don't want to buy gems often [click here](https://docs.google.com/spreadsheets/d/1qcYu22DIwEORUYuTJNnYnxS5ceQx8y6XJhVjBai_0lI/edit#gid=520131547&fvid=1324263742)
