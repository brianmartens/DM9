# DM9
9-Band Dynamic Mastering Suite for Reason Studios

## Required Rack Extensions / VST Plugins
 - [FabFilter Pro-C2, Pro-Q3, Pro-L2](https://www.fabfilter.com/products#mixing-and-mastering)
 - [Selig Auto-Leveler](https://www.reasonstudios.com/shop/rack-extension/selig-leveler/)
 - [Tinker CV](https://www.reasonstudios.com/shop/rack-extension/tinker-cv-math-assistant/)
 - [Unfiltered Audio YOKO Band-Splitter](https://www.reasonstudios.com/shop/rack-extension/yoko-band-splitter/)

## The Basics

### _Project Quickstart

If you've already purchased the above rack extensions and the Fab Filter mastering plugins, you should be able to load _Project with no issues.
Once it is loaded, you can import any audio track you want. **BE SURE TO NORMALIZE PEAK LEVELS TO 0 DB**. You can do this either in Reason itself
or beforehand in another program, e.g. Audacity. Once you have imported the normalized track, you should *generally* be good to export the audio without making further
modifications.

### What is Sensitivity?

Loosely defined, sensitivity is the degree to which the band processor adjusts itself when there is a change in the input signal. *Higher* levels of sensitivity are useful 
for tracks that have *low* dynamic variance, i.e. tracks that have already been heavily compressed / limited. Try to scale the sensitivity levels inversely with frequency for
smoother highs and punchier lows. 9 bands makes this pretty easy as you can start at 0 and add 16 for each band below band 9, or you can start at 64 and add 8 for each band below 9.
