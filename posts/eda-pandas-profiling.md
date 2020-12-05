---
title: 'Using Pandas Profiling for Meal Kit Data Validation'
date: '2020-12-05'
blogCategory: EDA Meal Kits
slug: pandas-profiling-meal-kits
author: Robert Nakano
blogImage: pandas-profiling-mealkits1.jpg
---
<strong>Methods</strong>: Exploratory Data Analysis, Pandas Profiling

<h4><a href='/other/meals_report_2020-12-04_00-36.html' target='_blank'>Pandas Profiling</a></h4>
<!-- embedded profile report -->
<iframe src='/other/meals_report_2020-12-04_00-36.html' height="350" width="680" title='Pandas Profiling Report'></iframe>

<h2>Summary</h2> 
One of the many weekly tasks at Pick a Kit is collecting meal kit menus from various services. This data is used in the Pick a Kit <a href="https://pickakit.com/meals">list of menus</a>. 
<a href="https://pickakit.com/meals"><p><img src='/images/pick-a-kit-meals.jpg'/></p></a>

We have been looking at better ways to understand and validate our data on a weekly basis: enter <a href="https://github.com/pandas-profiling/pandas-profiling">Pandas Profiling</a>. With a few lines of code, Pandas Profiling generates reports using data from a pandas dataframe. Check out a sample of Pick a Kit weekly meal kit data above!

<h2>Conclusion</h2>
It's great to have a quick, reproducible view of data in a variety of dimensions! Like any data report, the true benefit comes with the analysis; we'll be using this report as one entry point to understanding. Additionaly, <a href="https://en.wikipedia.org/wiki/Hofstadter%27s_law">Hofstadter's Law</a> was in full effect; in order to get Pandas Profiling working, I performed a much needed update to Windows 10, Windows Subsystem for Linux (WSL), and updated Node.js, Python, and their respective packages. A reminder to keep paying down your technical debt!

