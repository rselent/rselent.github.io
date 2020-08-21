---
layout: post
published: false
readtime: true
title: Asteroids!
subtitle: Can data science help identify life-threatening space rocks?
thumbnail-img: assets/img/posts/asteroids/ast-thumb.png
cover-img: 
  - "assets/img/posts/asteroids/ida-dactyl-cover.png" : "Asteroid Ida + moon Dactyl from 6,500 miles away"
social-share: true
gh-repo: rselent/lambda-buildweek2-asteroids
gh-badge: [star, fork, follow]
---


Ever since the days of Tycho Brahe studying the distance of comets from Earth in the 16th century, or the 1898 discovery of the first-ever recorded Near-Earth Asteroid, 433 Eros, we've been captivated by and enamoured with what happens beyond the veil of our atmosphere. We've also been fearful of being smote by cosmic deities, forces, or even just the cosmos itself.

### Background 

100 years after the discovery of 433 Eros, in March of 1998, new observational data gathered from the University of Arizona's Spacewatch Project led the Minor Planet Center in Cambridge, Massachusetts to make a prediction that ultimately shook both media headlines and the world: *recently discovered 1km-wide asteroid 1997 XF<sub>11</sub> could hit Earth in 2028!*  
According to NASA, an asteroid that has a diameter of just 140 meters (a little more than 1.5 football fields) is large enough to destroy an entire city; one with a diameter of over 1 kilometer (just under half of a mile) is capable of destroying *billions* of people on Earth, releasing over *100,000 megatons* of energy on impact.  
For comparison, the nuclear bombs dropped on Hiroshima and Nagasaki during World War II released only *36 kilotons* (or *0.036 megatons*) of energy.

-----

On its surface, this new prediction seemed as dire as ever, *miscalculated* as it was. Within hours of the media breakout, its orbital prediction was refined and corrected to its now-certain trajectory: passing Earth on 26 October 2028, at a distance of 0.0062 astronomical units (930,000km, or about twice the distance to the moon).  
*1 astronomical unit (au) is equal to the mean distance between the Earth and the Sun.*

That media frenzy and panic, however, demonstrated a need for much greater clarity and precision when communicating with the public about close passes of Near-Earth Objects (NEOs), according to NASA. Especially when they could see that their understanding of the solar system was only really just beginning to open up -- in the first 3 months of 1998 alone, over 40 Near-Earth Asteroids were discovered, approximately 75% of which were over that city-leveling 140m diameter size:

![](../assets/img/posts/asteroids/recorded-neo-cum-1998.png)

So, in 1998, NASA Headquarters requested that Jet Propulsion Laboratory (JPL), based in Pasadena, California, create a new office to specifically work with and catalogue data provided by the International Astronomical Union-sanctioned Minor Planet Center, and coordinate with academic institution observatories and US Air Force space surveillance assets.  
This office, the Near-Earth Object Program Office, was renamed in 2016 to the Center for Near-Earth Object Studies (CNEOS). And without this office, I doubt that any of what you're about to read here could have happened, so I felt I should at least give some semblance of deference or reverence, however minor.

### Space is big.

As an artist, as someone who has studied art most of their life, whenever I approach a project like this, I'm often inundated with creative thoughts and impulses of "*Wouldn't it be cool if...*"

"*Wouldn't it be cool if?*"

Wouldn't it be cool if I could create something that could literally help ***save the world??***

![](../assets/img/posts/asteroids/small-bodies.gif)

Every one of those dots in the above animation has been identified as a Near-Earth Object in our solar system. An asteroid or comet is classified as a Near-Earth Object if its closest distance to the Sun is, at any point, less than 1.3au.

-----

My previous project had an at-the-time whopping 50,000 observations, and I definitely wanted to top that. I discovered a dataset that someone else had published, wherein they pulled data from JPL's Small-Body Database (created under the aforementioned Near-Earth Object Program Office) and were trying to predict various features of asteroids. 

-----


* build domain knowledge
* clean / reduce features
* unbalanced nature of data
* models that were built (highlight feature reduction)
* measuring those models
* Deployment