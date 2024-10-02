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
Once it is loaded, you can import any audio track you want. **Adjust the input level depending on how much noise suppression you want to have using the guide below**. You can do this either in Reason itself
or beforehand in another program, e.g. [Audacity](https://www.audacityteam.org/). 

Once you have adjusted your track accordingly, you should *generally* be good to export the audio without making further
modifications, however, you may have more success trying one of the following:
 - **Minimum Noise**: Reduce the input input gain of the track by 5-10db. 10db should be enough to really reduce background hiss. If you are still getting hiss at 10db, then try going further or follow the recommendation in the *sensitivity* section below.
 - **Moderate Loudness**: Normalize the track to 0db peak loudness.
 - **Maximum Loudness**: Play the full length of the track within _Project 2. Then, check each input limiter to see which has the loudest recorded peak amplitude on the upper right hand side. Adjust the overall band gain on the DM9-base combinator upwards until the peak amplitude of the loudest input limiter shows between -3db to -4db. Going louder than -3db is not recommended.   

Once the export is complete it is up to you what to do next. If this is a song meant to be uploaded to a streaming platform, I would recommend using Audacity to normalize the track according to perceived loudness
(effects -> Loudness Normalization; set the LUFS value to -14 [youtube,spotify]). This should give you a positive gain boost, so you will likely want to run a final limiter over the result before exporting the final track to prevent
clipping. Audacity should let you use the FabFilter pro-L2 limiter to do this final limiting stage. I would recommend using 32x oversampling and maximum lookahead as this is a single-pass application of the limiter so live performance won't be a concern.

### What is Sensitivity?

Loosely defined, sensitivity is the degree to which the band processor adjusts itself when there is a change in the input signal. If you have a track that has a LOT of hiss, then you should scale the sensitivity levels inversely proportional with frequency. 
9 bands makes this pretty easy as you can start at 127 for band 1 and subtract 16 for each band until 0 for band 9.

I've added automation lanes for this already so all you need to do is adjust the values as you see fit.
