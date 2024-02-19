# DM9
9-Band Dynamic Mastering Suite for Reason Studios

## Required Rack Extensions / VST Plugins
 - [FabFilter Pro-C2, Pro-Q3, Pro-L2](https://www.fabfilter.com/products#mixing-and-mastering)
 - [Selig Auto-Leveler](https://www.reasonstudios.com/shop/rack-extension/selig-leveler/)
 - [Tinker CV](https://www.reasonstudios.com/shop/rack-extension/tinker-cv-math-assistant/)
 - [Unfiltered Audio YOKO Band-Splitter](https://www.reasonstudios.com/shop/rack-extension/yoko-band-splitter/)

## The Basics

### _Project Quickstart

If you've already purchased the above rack extensions and the FabFilter mastering plugins, you should be able to load _Project with no issues.
Once it is loaded, you can import any audio track you want. **BE SURE TO NORMALIZE PEAK LEVELS TO 0 DB**. You can do this either in Reason itself
or beforehand in another program, e.g. [Audacity](https://www.audacityteam.org/). 

Once you have imported the normalized track, you should *generally* be good to export the audio without making further
modifications, however, you may have more success trying one of the following:
 - Play the full length of the track within _Project. Then, open each of the 9 limiters in the 'DM9 - base' combinator and find the band with the loudest observed peak level.
   Next, adjust the **band gain** control on the combinator to add enough gain to raise that peak level to 0db. Then run the export.
 - Play the full length of the track within _Project. Then, adjust the gain level for each of the 9 limiters and independently set each to raise its peak level to 0db. Then run the export.
   You may need to be careful with tracks that have a lot of background noise when setting bands 7-9 and may want to consider adding less/no gain to prevent introducing unwanted noise.

Once the export is complete it is up to you what to do next. If this is a song meant to be uploaded to a streaming platform, I would recommend using Audacity to normalize the track according to perceived loudness
(effects -> Loudness Normalization; set the LUFS value to -14 [youtube,spotify]). This should give you a positive gain boost, so you will likely want to run a final limiter over the result before exporting the final track to prevent
clipping.

### What is Sensitivity?

Loosely defined, sensitivity is the degree to which the band processor adjusts itself when there is a change in the input signal. It also reflects how long it takes to recover from periods of intense signal. Generally, you should scale the sensitivity levels proportionally with frequency. 
9 bands makes this pretty easy as you can start at 0 for band 1 and add 16 for each band until 9.

I've added automation lanes for this already so all you need to do is adjust the values as you see fit.
