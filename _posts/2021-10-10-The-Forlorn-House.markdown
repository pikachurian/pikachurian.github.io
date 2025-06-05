---
layout: project
title:  "The Forlorn House"
year: 2021
#date:   0000-00-00 00:00:00 -0400
categories: 'Video-Game'
category-text: 'Video&nbsp;Game'
thumbnail: 'forlorn-house-thumbnail.png'
image-folder: '/assets/img/the-forlorn-house/'
#description: Fightcorin'

game-engine: 'Unity.'
art-software: 'Aseprite, Adobe Photoshop, and Blender.'
music-software: 'FL Studio.'
sfx-software: 'Bfxr, and Audacity.'

#![Image]({{ site.page }}/assets/img/FightcoreThumbnail.png)
---


<h1>The Forlorn House</h1>

<figure>
    <img src= '{{ page.image-folder }}forlorn-house-thumbnail.png' alt='Game title'/>
    <figcaption></figcaption>
</figure>

<a href="https://pikachurian.itch.io/theforlornhouse" class="pika-button">
    Game Link
</a>

<h2>GAMEPLAY</h2>

<p>
    You are stuck in a house with a creature. You must collect keys around the house to unlock different rooms and, eventually, escape. You must have the correct key selected while interacting with a locked door to unlock it. If you have the incorrect key or a different item selected from your inventory the game will tell you which key you need. While your flashlight is off, your sanity depletes. However, leaving your flashlight on could alert the creature. You need to find and select the flashlight in order to use it. You can restore your sanity by standing under a light. You can turn on lights by interacting with nearby light switches. The creature is alerted when you switch and leave on a light. You lose if the creature catches you or your sanity depletes to 0%.
</p>

<h4>CONTROLS</h4>

<ul>
    <li>
        Use the WASD keys to move.
    </li>
    <li>
        Use the mouse to look around.
    </li>
    <li>
        Press the E key to interact with doors or switches and collect items.
    </li>
    <li>
        Keys 1 through 9 on the keyboard correspond to different items you have, or null if there isn’t an item at that key, press the key to select that item. You can also use the scroll wheel on the mouse to cycle through the items.
    </li>
    <li>
        After you’ve found the flashlight, Right click toggles your flashlight while it is selected.
    </li>
</ul>

<h2>INFO</h2>

<p>
    The Forlorn House was created in 72 hours for 49th Ludum Dare game jam; one of the most popular jams. This was my first horror game made in Unity. The creature AI roams around the house to turn off lights and will chase the player if it sees them. The player restores sanity while under a light. Each light has an invisible detection zone. The game knows to restore the player’s health when they’re in the zone and the light is set to on. The creature tracks what lights are on and will move toward them to turn them off. The creature checks if the player is within range, if so, the creature will enter its chasing state. Otherwise, if none of these conditions are true the creature will pick a random reachable space in the house and move towards to it, entering a roaming state. The player will lose shortly after touching the creature. To create uncertainty in the player as to when the creature will strike, touching the creature doesn't instantly defeat you. Instead, the game will wait a certain amount of time before triggering the creature to appear suddenly in front of you, causing a game over. Looking around during this time can cause the creature to appear sooner. This game ranked 74th for mood out of 2939 game submissions; someone even made a YouTube video on it. During the Halloween following the game’s release, I printed and gave out small pamphlets, stylized to look like game cases, featuring a link to the game. The game is playable in the browser via itch.io, though, the downloadable version performs significantly better than the web version. The low-resolution aesthetic of the game is inspired by 90s PlayStation games. In this vein, the SpaceStation logo, which appears in the games intro and cover, is a spoof on the PlayStation logo.
</p>

<h2>ROLES & CREDITS</h2>
<p>
    I was a designer, sole composer, and sole coder for the game.
</p>

<h4>GAME ENGINE</h4>
<p>{{ page.game-engine }}</p>

<h4>ART SOFTWARE</h4>
<p>{{ page.art-software }}</p>

<h4>MUSIC SOFTWARE</h4>
<p>{{ page.music-software }}</p>

<h4>SOUND EFFECT SOFTWARE</h4>
<p>{{ page.sfx-software }}</p>

<h2>IMAGES</h2>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig5.PNG'/>
    <figcaption>Figure 8: Main menu.</figcaption>
</figure>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig6.PNG' alt='Nightcore song selection menu.'/>
    <figcaption>Figure 9: Freeplay menu. Currently nightcore songs are shown. Tab can be pressed to show the regular song versions.</figcaption>
</figure>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig7.PNG' alt='Victory screen.'/>
    <figcaption>Figure 10: Victory screen.</figcaption>
</figure>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig8.png' alt='A retro brawler themed level.'/>
    <figcaption>Figure 11: Level editor. Currently editing a place holder song.</figcaption>
</figure>






<style type="text/css">
    a.toolbar {
      color: wheat;
      background-color: #f44336;
      padding: 14px 25px;
      display: inline-block;
    }
    a.pika-button {
        color: wheat;
        background-color:rgb(59, 149, 39);
        padding: 14px 25px;
        display: inline-block; 
    }
</style>