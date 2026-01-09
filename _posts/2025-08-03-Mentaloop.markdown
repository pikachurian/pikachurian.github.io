---
layout: project
title:  "MENTALOOP"
year: 2025
#date:   0000-00-00 00:00:00 -0400
categories: 'Video-Game'
category-text: 'Video&nbsp;Game'
thumbnail: 'MentaloopThumbnail.png'
image-folder: '/assets/img/mentaloop/'

game-engine: 'Godot.'
art-software: 'Scratch, Aseprite.'
music-software: 'Audacity, FL Studio.'
sfx-software: 'Audacity, FL Studio.'

#![Image]({{ site.page }}/assets/img/FightcoreThumbnail.png)
---

<h1>MENTALOOP</h1>

<figure>
    <img src= '{{ page.image-folder }}MentaloopThumbnail.png' alt='Game title'/>
    <figcaption></figcaption>
</figure>

<a href="https://pikachurian.itch.io/mentaloop" class="pika-button">
    Game Link
</a>

<h2>GAMEPLAY</h2>

<p>
    You are the visionary. Help people overcome their circular struggles by entering their minds to slay their inner demons.
</p>

<figure>
    <img src= '{{ page.image-folder }}MentaloopPlatformer1.png'/>
    <figcaption>Figure 1: Platformer gameplay. The character with the white goggles is the player. The white diamond shape under the player is an active weakpoint that can be attacked to damage the inner demon. </figcaption>
</figure>

<p>
    Levels consist of looping serpent-like inner demons. Because the levels loop, the player can run in one direction and end up on the other side of the level. The player progresses by slaying the inner demon, which is achieved through ground pounding its weakpoints.
</p>

<figure>
    <img src= '{{ page.image-folder }}MentaloopPlatformer2.png'/>
    <figcaption>Figure 2: Zoomed out view of the same level.</figcaption>
</figure>

<p>
    The player can also ground pound the inner demon to shift the level. This causes airborne objects to stay in place, while those attached to the demon move along with it.
</p>

<figure>
    <img src= '{{ page.image-folder }}MentaloopOverworld.png'/>
    <figcaption>Figure 3: The player's room as seen in the overworld. Notice how the artstyle shifts into pixel art to show a distinction between the vector art platformer levels that take place in the psyche, and the pixel art physical overworld.</figcaption>
</figure>

<p>
    Between levels, the player navigates a pixel art rpg-like overworld where they look for more people to help. When the player discovers who to help, the player can then enter their psyche to start the next level.
</p>

<p>Note: Due to the length of the controls segment, information about controls is at the bottom of this page.</p>

<h2>INFO</h2>

<p>
    This game was created in four days for the Game Maker's Toolkit 2026 game jam. The theme of the jam was loop, so my collaborators and I thought it would be interesting if the gameplay involved walking around on a looping level.
</p>

<p>
    A challenge we came across early in development was figuring out how to have the player walk around and upside down on a loop, while retaining jumping physics. The solution used in a game with similar looping levels, <i>Mario Galaxy,</i> involved creating pockets around the level that determined the direction gravity was applied in that area. Godot, the game engine we were using, has a built in system for creating these gravity pockets. However, Godot's system uses its physics engine, which works fine for most cases, but might make our platformer feel less responsive. I ended up going with a non-physics based solution. Using Godot's path system I made a loop representing the level and made each object a path follower that could move along the loop. Programming the player's movement was similar to a non-looping game, with the main difference being changing the player's progress around the loop, instead of their horizontal position, for left and right movement, and changing their offset from the loop, instead of their y position, for jumping.
</p>

<p>
    Using paths for the level also made creating a looping serpent-like creature easier, as the inner demons in the game are made of a bunch of small circular segments created close together presenting the illusion of a solid creature. When we needed to shift the level and move the serpent, it involved shifting the progress position of the segments of the serpent, as well as the objects on it.
</p>

<h2>ROLES & CREDITS</h2>

<p>
    I was a designer, programmer, level designer, and composer for the game.
</p>

<h4>GAME ENGINE</h4>
<p>{{ page.game-engine }}</p>

<h4>ART SOFTWARE</h4>
<p>{{ page.art-software }}</p>

<h4>MUSIC SOFTWARE</h4>
<p>{{ page.music-software }}</p>

<h4>SOUND EFFECT SOFTWARE</h4>
<p>{{ page.sfx-software }}</p>


<h2>CONTROLS</h2>

<h4>Platformer</h4>

<h6>Keyboard</h6>

<ul>
    <li>
        WASD - move
    </li>
    <li>
       SPACE - jump, speed up text
    </li>
    <li>
       CTRL - ground pound
    </li>
    <li>
       TAB - zoom out
    </li>
    <li>
       E - confirm text
    </li>
    <li>
       ESC - return to title
    </li>
</ul>

<h6>Controller</h6>

<ul>
    <li>
        Joystick or D-Pad - move
    </li>
    <li>
       Bottom face button - jump, confirm text
    </li>
    <li>
       Left face  button - ground pound
    </li>
    <li>
       Top face button - zoom out
    </li>
    <li>
       Right face button - speed up text
    </li>
    <li>
       START - return to title
    </li>
</ul>

<h4>Overworld</h4>

<h6>Keyboard</h6>

<ul>
    <li>
        WASD - move
    </li>
    <li>
       SPACE - run, speed up text
    </li>
    <li>
       E - interact, confirm text
    </li>
    <li>
       ESC - return to title
    </li>
</ul>

<h6>Controller</h6>

<ul>
    <li>
       Joystick or D-Pad - move
    </li>
    <li>
       Right face button - run, speed up text, 
    </li>
    <li>
       Bottom face button - interact, confirm text
    </li>
    <li>
       START - return to title
    </li>
</ul>



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