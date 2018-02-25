---
layout: post
title: Google Hashcode<p>The Quest For Employability</p> 
---
Whilst searching for jobs a common theme regually came up: what events do you do in regards to your degree, outside of your degree? The reason they ask this is more than likely to make sure that you enjoy doing what you do, rather than just being in for the money. This led myself and a few friends to enter as many of these as possible before september 2018, the first being Google Hashcode. Below is a practice example they send to try and get you in the right frame of mind.

<center><b>The Challenge </b></center> 

The practice issue Google provided was named 'Pizza' and the aim was to slice the pizza to the specification they provided you with. The pizza had two ingredients, mushroom and tomato, with each ingredient taking up one grid. You are provided with three specifications: 

<ul style="list-style-type:disc">
  <li>The minimum and maximum slice size</li>
  <li>The minimum and maximum amount of each ingredient on each slice</li>
  <li>The column and row size of the pizza</li>
</ul> 

This leaves you something like the below, which is the small pizza grid specifications. 

![_config.yml]({{ site.baseurl }}/images/Screen Shot 2018-02-25 at 17.58.11.png)

In this case each slice needed to have 1 of each ingredient per slice with a maximum slice size of 5. The aim is to create an algorithm to use as many of the grids as possible. 

<center><b>Our Solution</b></center> 

<b>Spoiler alert:</b> this may be the worst spoiler alert ever given but if you want to try and figure it out for yourself don't read on. 

We decided that initially we would go through horizontally pairing adjacent T and Ms and then do the same horizontally. This initially left us with something like this:

![_config.yml]({{ site.baseurl }}/images/Screen Shot 2018-02-25 at 17.58.22.png)

Once the first was complete and the slices had been coupled the grids with no coupling would then look around and attack themselves to the most appropriate slice, depending on the given variables. If there were multiple slices it could attach to it would attack to the smallest, and if they were the same size, it would just attack to the one it checked first. 

The grid below shows how the first in paired piece would look around:

![_config.yml]({{ site.baseurl }}/images/Screen Shot 2018-02-25 at 17.58.30.png)

As can be seen the 2nd and 4th checks are the most suitable, however as they are the same size the chosen slice is the first checked out of the two, so will join slice check two. After this process has been completed a couple of times the pizza will look like this. 

![_config.yml]({{ site.baseurl }}/images/Screen Shot 2018-02-25 at 17.58.40.png)

After this process has ran through a couple of times the pizza will look like this. Leaving 41/42 of the pizza slices fitting the specification.

This solution was found in about 30 minutes due to time restraints, so the full 42 slices couldn't be filled. If you had a solution that managed to fill all slices, I'd enjoy hearing from you. 

