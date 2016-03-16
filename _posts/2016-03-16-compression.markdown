---
layout: post
title:  "What is limiting?"
date:   2016-03-16 11:57:04 -0500
categories: music
---
_A quick overview of dynamic range and the 'loudness wars' in music production._

Imagine you're looking at a waveform, i.e. the waveform for Animals by Martin Garrix:

![Animals]({{ site.url }}/assets/animals_clear.png)
<button onclick="if (document.getElementById('yt').style.display=='block') {document.getElementById('yt').style.display='none';this.innerHTML='Show Animals Youtube Embed'} else {document.getElementById('yt').style.display='block';this.innerHTML='Hide Animals Youtube Embed'}">Show Animals Youtube Embed</button>
<iframe id="yt" width="560" height="315" src="https://www.youtube.com/embed/gCYcHz2k5x0" frameborder="0" style="display: none;"></iframe>

You'll notice that the waveform stays really close to the maximum aplitude for almost the whole song. This is a highly compressed or more accurately, "limited" song, as it's dynamic range is rather small. This means that the hightest peaks of the song are relatively close to the level of the lowest valleys.

Contrary to what you might expect, this is actually desireable, to some degree. A big difference between the highest peaks and valleys, i.e. a large dynamic range will result in an overall quiter sounding soung. In essence, squashing dynamic range allows you to exchange the dynamic nature of a song for overall loudness.

Let's look at another example.

Here's a song I've been working on. Nothing pretty, just messing around with layering melodies.

<audio controls>
  <source src="{{ site.url }}/assets/layers_uncomp.mp3" type="audio/mp3">
</audio>

And the corresponding waveform:

![Layers-Uncompressed]({{ site.url }}/assets/layers_uncomp.png)

Notice how the peaks are much more distinct; this song hasn't been compressed or limited at all. Now, we'll limit it in Audacity.

Let's go ahead and see a quick video of this:

<video  height="340" width="512" controls>
  <source src="{{ site.url }}/assets/limiting.webm" type="video/webm">
</video>

Here's the new waveform:

![Layers-Compressed]({{ site.url }}/assets/layers_comp.png)

And finally, here's how the new, compressed audio sounds:

<audio controls>
  <source src="{{ site.url }}/assets/layers_comp.mp3" type="audio/mp3">
</audio>

Now, it may take a somewhat sentive ear to notice the subtle differences between this clip and the original, but one thing is abundantly clear: this new clip is much, much louder than the original. Visually, this is apparent from the waveforms; the second occupies way more space, geometrically, than the original. Like Animals, it is much closer to the maximum amplitude for the duration of the song.

In doing this, however, we have lost some of the preciseness of the stick and clap. They no longer cut through the bassline as  well, since we have squashed all the peaks down to a single edge at the maximum volume. This effect is a little less apparent than the volume boost, so some might consider this compressing successful. However, the 8 dB gain we used is generally way too much, and would seriously deteriorate the quality for any track more complex than this one.

_What is the takeaway here?_

Ultimately, people want their tracks to sound loud. Really loud. Like in-your-face-till-you-dont-hear-anything-else-loud. This is okay, since research with ABX experiments[^1] and Fletcher–Munson curves[^2] shows that essentially, our ability to distinguish sounds (acutity) increases as sounds get louder. What has happened, over time, is that artists have gradually compressed their songs more an more, especially in the hip-hop and rock genres[^3], and presumably in the electronic genres as well. Classical music retains it's dynamic range, for the most part. This gradual decent into loudness sacrifices the fidelity of music, and is generally not a good thing. Paul Lamere has a great [article](http://musicmachinery.com/2009/03/23/the-loudness-war/) on this issue.

__tl;dr__ Limiting makes your song's volume less dynamic, in exchange for an overall increase in loudness. Artists do this more and more as time goes on, to the detriment of their music's fidelity.

[^1]: http://www.bostonaudiosociety.org/bas_speaker/abx_testing.htm
[^2]: http://upsilonaudio.com/wp-content/uploads/2013/06/Loudness-Its-Definition-Measurement-and-Calculation.pdf
[^3]: http://musicmachinery.com/2009/03/23/the-loudness-war/
[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
