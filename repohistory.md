# Testing File for: rrl / Recreational Reading Log: Audio Books  

(*started 2022 July 25*)  

# Repository History:
* In July 2022 I started tracking my reading by adding a reference and notes for each book that I read or listened to.  
* Over time the pages grew to *an unreasonable length* -- becoming user-unfriendly.  I started trying to use Github markdown collapsible sections.  Technically, they worked well, but the native github UI did not seem to be a great fit for some non-Github users on their mobile devices...  
* Then I tried using [`Github pages`](https://docs.github.com/en/pages), which was kind of a trial because of the unclear and sometimes conflicting guidance for pages that employed collapsible sections and Github markdown.  For this site, the most important *fixes* were:  
  * Always put an empty line after collapsible section tags.  
  * Put double quotes around any string that included whitespace in the site config file (_config.yml).  
  * Use the `markdown: GFM` processor in the site config file (_config.yml).  

My _config.yml file:  
```yml
title: "Recreational Reading Log"
description: "List of my reading since 2022 July 25"
logo: https://mccright.github.io/rrl/m.svg
# https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/setting-a-markdown-processor-for-your-github-pages-site-using-jekyll 
markdown: GFM
```

I did not originally format this resource for Github-pages, which left me with a lot of page layout sloth and a little legacy technology debt to deal with before these pages would display properly.  Native Github repos support sloppy authoring practices that do not appear to transparently port over to Github pages.  Unfortunely, the [source repo](https://github.com/mccright/rrl) required material format updating...  
The Github pages GitHub Action build logs for my repo identified `jekyll-theme-primer-0.6.0` as its default theme (*Github pages [support a number of themes](https://pages.github.com/themes/)*).  It displayed bright white pages, but I prefer dark background with *white* text.  The [RubyDocs for `jekyll-theme-primer`](https://rubydoc.info/gems/jekyll-theme-primer) said that adding a new [style sheet](https://rubydoc.info/gems/jekyll-theme-primer#stylesheet) (`/assets/css/style.scss`) with the following content starts the customization process:  

```css
---
---

@import "{{ site.theme }}";
```

To that add your customizations.  To get a simple `dark` theme, you can use the `body` CSS recommended by [Mark A Vitale](https://github.com/markavitale) at [https://github.com/pages-themes/primer/issues/64#issuecomment-975787330](https://github.com/pages-themes/primer/issues/64#issuecomment-975787330) for a simple `style.scss` that looks like this:  

```css 
---
---

@import "{{ site.theme }}";
body {
	background-color: black;
	filter: hue-rotate(180deg) invert(90%);
}
``` 

There is [some valid criticism](https://news.ycombinator.com/item?id=26472246) of this approach, but it works for this github-pages site.  


# Now, Testing page content is below  

## Completed:  

<details><summary>Hamnet -- Love in the Time of Plague. By Maggie O'Farrell. 2020 </summary>

### Hamnet -- Love in the Time of Plague. (13:00)  
[https://www.overdrive.com/media/5067417/hamnet](https://www.overdrive.com/media/5067417/hamnet)  
By [Maggie O'Farrell](https://en.wikipedia.org/wiki/Maggie_O%27Farrell)  (1972 - _)  

Reader Notes:  Enter one family's world, more than 4 centuries ago.  Maggie O'Farrell delivers the magic (*her expertly-tuned imagination,  skilful editing and extremely hard work*) of helping the reader join the extended family of William Shakespeare.  The primary lens for this exploration is Agnes (*Anne*) Hathaway -- William Shakespeare is only a minor supporting role.  Marriage, motherhood, power, loss & grief, along with the *daily life* in late 16th century England are made so rich, immediate, intense, and so *real* that it is easy to lose yourself in this story.  In addition to exceptional writing, the reading by [Ell Potter](https://www.beeaudio.com/narrator/ell-potter) seemed a perfect fit.  
Literary Review by : [https://literaryreview.co.uk/love-in-the-time-of-plague-2](https://literaryreview.co.uk/love-in-the-time-of-plague-2)  
Wikipedia Summary: [https://en.wikipedia.org/wiki/Hamnet_(novel)](https://en.wikipedia.org/wiki/Hamnet_(novel))  
Review by Miranda France in the Literary Review:   [https://literaryreview.co.uk/love-in-the-time-of-plague-2](https://literaryreview.co.uk/love-in-the-time-of-plague-2)  

</details>


<details><summary>Shaman, By Kim Stanley Robinson. 2013 </summary>

### Shaman (15:00)  
[https://www.overdrive.com/media/1372669/shaman](https://www.overdrive.com/media/1372669/shaman)  
By [Kim Stanley Robinson](https://en.wikipedia.org/wiki/Kim_Stanley_Robinson)  (1952 -_)  
Kim Stanley Robinson bibliography:  [https://en.wikipedia.org/wiki/Kim_Stanley_Robinson_bibliography](https://en.wikipedia.org/wiki/Kim_Stanley_Robinson_bibliography)  

Reader's Notes: What an excellent book!  We go on a fast-moving journey with a young apprentice shaman, his teacher, a small band of hunter-gatherers, and the others who join the story along the way.  We learn a lot about [stone age](https://en.wikipedia.org/wiki/Stone_Age) / [ice age](https://en.wikipedia.org/wiki/Last_Glacial_Period) [European early modern humans](https://en.wikipedia.org/wiki/European_early_modern_humans) and their cultures.  

3rd Party Summaries:  
Wikipedia Summary/Review: [https://en.wikipedia.org/wiki/Shaman_(novel)](https://en.wikipedia.org/wiki/Shaman_(novel))  

</details>


<details><summary><a name="aurora_kim_stanley_robinson"></a>Aurora, By Kim Stanley Robinson. 2015 </summary>

### Aurora (17:00)  
[https://www.overdrive.com/media/2234713/aurora](https://www.overdrive.com/media/2234713/aurora)  
By [Kim Stanley Robinson](https://en.wikipedia.org/wiki/Kim_Stanley_Robinson)  (1952 -_)  
Kim Stanley Robinson bibliography: [https://en.wikipedia.org/wiki/Kim_Stanley_Robinson_bibliography](https://en.wikipedia.org/wiki/Kim_Stanley_Robinson_bibliography)  

<details><summary>Reader's Notes and Other 3rd Party Summaries:</summary>

Reader's Notes: Another excellent book!  
A [generation ship](https://en.wikipedia.org/wiki/Generation_ship) is launched from Earth in 2545 at 0.1 c (i.e. traveling at 108,000,000 km/h or 10% the speed of light). It includes twenty-four self-contained biomes and an average population of two thousand people.  Their destination is the Tau Ceti system to begin colonization of a planet's moon, an Earth analog, which has been named Aurora.  
The book follows Devi (the ship's de facto chief engineer and leader) and Freya (Devi's daughter) and the ship's AI quantum computer through a journey of discovery.  

3rd Party Summaries:  
Wikipedia Summary/Review: [https://en.wikipedia.org/wiki/Aurora_(novel)](https://en.wikipedia.org/wiki/Aurora_(novel))  

</details>

</details>


<details><summary>The Giver of Stars.  By Jojo Moyes.  2019 </summary>

### The Giver of Stars. (13:52)  
[https://www.overdrive.com/media/4581755/the-giver-of-stars](https://www.overdrive.com/media/4581755/the-giver-of-stars)  
By [Jojo Moyes](https://en.wikipedia.org/wiki/Jojo_Moyes)  (1969 -- _)  
Reader's notes:  
Wikipedia summary: [https://en.wikipedia.org/wiki/The_Giver_of_Stars](https://en.wikipedia.org/wiki/The_Giver_of_Stars)  

</details>
