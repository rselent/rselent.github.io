---
layout: post
published: false
title: Untitled
---


When I set out on the long journey that this project was, I was just a wee data sprout scientist. I found this relatively new and unused dataset, and I thought to myself, "_I miss this big city that I grew up around; wouldn't it be cool if..._" and not much more. I _wanted_ a bigger question -- perhaps something with more gravitas, or that could actually impact peoples' lives -- but that _wouldn't it be cool_ question just kept invading my thoughts. So, eventually, I followed that impulse, as all artists tend to do.  
I tried to make the best of it, expecting that my audience (or customers, clients, or whomever) would maybe, at best, gain a better understanding or picture of the Airbnb market in New York. I'll admit, it was a little didactic and so I struggled to invent a question that this dataset could answer. But follow me down this rabbit hole -- I doubt you'll be disappointed.

One of the very first interesting things I found was that the dataset had over 48,000 observations -- and that's in a city that only covers 302mi^2 (782km^2). That's over 158 Airbnb rental properties per mile^2 (or over 61 per km^2). If we look at that in map form, it looks a little something like this:

## CONTEXT VISUALIZATION (1st visualization)

If we remove the map from underneath all those datapoints, we'd still be able to clearly define all five Boroughs of New York City. That's insane. Here's a look at those 48,000 Airbnb rentals and how they're divided up between each Borough:

## POPULATION BARPLOT (3rd visualizations)

I started to wonder, though. With over 48,000 possible places for someone to rent on any given day, surely many of these Airbnb rentals must be dirt cheap, right? Well, after a little exploration and data wrangling -- which, honestly, can feel like herding cats sometimes -- I had my answer...  
(and a fancy graph or two, too!)

## CODE SNIP price.min()

## CODE SNIP price.max()

You're probably thinking to yourself now, much like I was, "_Wait, there are Airbnb's available for $0 per night, and others for $10,000 per night???_" Like I said, this comes with some cool graphs, and this is kind of where it starts to get interesting:

## PRICE BOXPLOT (5th visualization)

First, you'll probably notice that I capped the graph at ~$4,000. I did this to preserve readability in the sub-$500 range -- if I left it uncapped, the boxes would have just been lines, because remember: the
















