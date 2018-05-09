+++
title = "Hello World!"
date = 2018-03-02T13:48:36-08:00
tags = ["environment","gis","remote sensing"]
categories = ["posts"]
draft = false
+++
Hello world! This is my very first post to this mini resume-blog site. Primarily, I hope to use this to maintain a working version of my resume, but I will also use it to display some of my side projects “&” hopefully teach some interesting remote sensing or GIS techniques along the way.

This site is generated using Hugo, a static site generator, and is being hosted via GitHub. I’d suggest the combo to anyone who is willing to delve a little into HTML/CSS and likes being cheap. Honestly you can make a killer looking site by sticking to the per-created themes, but if you have a little drive you can make some worthwhile alterations.

I spent a decent amount of time looking for a web presence that worked for me… essentially I wanted something, free(maybe extremely cheap), slick, and something that allowed me to use my limited front-end experience to funk it up. Specifically, I was looking to incorporate story maps & an image slider from Knightlabs because I really liked how easy they made the process. For my work as a Geoinformatics fellow science communication is an important aspect and being able to freely and quickly host these things on the web was an interesting topic to me. Places like Wordpress or GoogleSites didn’t make the cut because or pay-to-blog or iFrame restrictions.
Using Hugo I can have full control of my site…while not having to have full control, if you catch my drift. To display this two image slider I made a “short-code.” Basically, its just a wrapper so you can quickly embed it via the markdown format for Hugo sites.

{{<2pan 805d51aa-1e7d-11e8-b263-0edaf8f81e27>}}

The short-code for the slider (just a reminder that it is knightlabs that did all the real work here) to embed on a hugo site is:
~~~
<div>
<iframe frameborder="0" class="juxtapose" width="600" height="396" src="https://cdn.knightlab.com/libs/juxtapose/latest/embed/index.html?uid={{ index .Params 0 }}"></iframe>
</div>
~~~
then to call it in you're post all you need to the id generated when you make your slider, for example:
~~~
<2pan 805d51aa-1e7d-11e8-b263-0edaf8f81e27>
~~~