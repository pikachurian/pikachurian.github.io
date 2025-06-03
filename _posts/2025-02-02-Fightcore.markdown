---
layout: project
title:  "FIGHTCORE"
year: 2022
#date:   0000-00-00 00:00:00 -0400
categories: 'Video-Game'
category-text: 'Video&nbsp;Game'
thumbnail: 'FightcoreThumbnail.png'
image-folder: '/assets/img/fightcore/'
#description: Fightcorin'

game-engine: 'GameMaker Studio 2.'
art-software: 'Aseprite, Adobe Animate, Adobe Photoshop.'
music-software: 'FL Studio.'
sfx-software: 'Bfxr.'

#![Image]({{ site.page }}/assets/img/FightcoreThumbnail.png)
---


<h1>FIGHTCORE</h1>

<figure>
    <img src= '{{ page.image-folder }}FightcoreThumbnail.png' alt='Game title'/>
    <figcaption></figcaption>
</figure>

<a href="https://pikachurian.itch.io/fightcore" class="pika-button">
    Game Link
</a>

<h2>GAMEPLAY</h2>

<figure>
    <img src= '{{ page.image-folder }}FightcoreGameplayExample.PNG' alt='Gameplay example'/>
    <figcaption>Figure 1: Example of gameplay.</figcaption>
</figure>

<p>
    Move between two lanes and punch enemies to the beat in this fusion of a rhythm game and a fighting game. Your left and right fist target different enemies in your current lane. You can switch lanes to target different enemies. You have two circles in front of your character; these act as visual guides to see where an enemy should be when you punch them. Larger enemies can be hit using both fists. They aren’t defeated in one hit, instead you must punch them until their shield meter depletes. Additional hits dealt to large enemies score bonus points. From the top left corner going down, you have a health bar, this depletes every time an enemy walks past you off-screen. Once your health is depleted, you lose. Underneath your health bar is the multiplier bar. Your multiplier bar shows the value of the multiplier applied to the score received form each enemy you hit; the fuller the meter, the larger the value. Underneath this is the green/red combo bar, which increases with “sick” or “rad” hits (these terms denote levels of accuracy) and determines your rank at the end of a level. Your current rank resets if you miss an enemy. When you hit an enemy, your accuracy is labeled, from most to least accurate, rad, sick, square, and miss. At the end of each level you are given a score based on your accuracy, your percentage of enemies hit, and your combo rank at the end of a level.
</p>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig4.PNG' alt='Start of the nightcore version of the airship level.'/>
    <figcaption>Figure 2: Start of the nightcore version of the airship level.</figcaption>
</figure>

<p>
    There are three different songs/levels each with a nightcore variant, which gives the song a faster remix, changes the appearance of the enemies and scenery in the level, increases the difficulty of the level, and removes the visual guides in front of your character. This gives a total of six songs/levels including nightcore remixes. The six levels are sorted into three themes: a city, an airship, and a castle.
</p>

<p>
    In story mode you’ll play all the levels in order of difficulty. The levels alternate between regular and nightcore. In freeplay you can choose which level you want to play, including nightcore and regular versions.
</p>

<h4>CONTROLS</h4>

<ul>
    <li>
        Press the f4 key to toggle full screen mode. 
    </li>
    <li>
        Use the WASD keys to navigate menus and switch lanes during levels.
    </li>
    <li>
        Down or right array keys cause your character to throw a right punch or make selections in menus.
    </li>
    <li>
        Up or down keys throw a left punch or undo a selection in menus
    </li>
    <li>
        Enter is the start key and is used to pause the game during a level. 
    </li>
    <li>
     Tab is the select key and is used to toggle nightcore mode in the freeplay menu. 
    </li>
</ul>

<h2>INFO</h2>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig1.png' alt='A retro brawler themed level.'/>
    <figcaption>Figure 3: City theme with three different enemy types, in order from left to right: large enemy, regular, and fast.</figcaption>
</figure>

<p>
    Fightcore was developed for the GXC #NoticeMe Game Jam. The deadline was two weeks and you had to publish your game to the GXC online game platform. I love composing music, so I proposed the idea of creating a rhythm game to my siblings. We agreed on the concept and started working on it. My brother designed most of the gameplay concept and my sister handled sound design. We took advantage of the two-week deadline to create the largest jam game we made yet. 
</p>

<p>
    The game has three themes, into which the six levels are grouped, all inspired by different video games: a Street Fighter inspired city, a Mega Man inspired airship, and a Dark Souls inspired Castle. The music of each theme is inspired by a different genre as well: ska, chiptune, and orchestral respectively. Each theme also has unique artwork for the enemies and environment.
</p>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig2.png' alt='Mega Man inspired airship level.'/>
    <figcaption>Figure 4: Airship theme. Same three enemy types as in figure 3 in the same order just with a different appearance.</figcaption>
</figure>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig3.png' alt='Castle themed level.'/>
    <figcaption>Figure 5: Castle theme. Same enemy types.</figcaption>
</figure>

<p>
    I coded a program built into the game that allows developers to create levels for the game. This program cannot be accessed by players of the game, it is for development purposes only. The software is similar to digital music composition software, in that it has a grid for notes to be placed. The difference though, is instead of placing notes, you’re placing enemies that will walk towards the player in time with the music. To edit a level, you load a level file into the program, set the beats per minute (BPM) to match the song loaded in with the level, and start placing enemies on the grid. These levels can be saved locally to the computer. I coded this software, and my brother used it to create the levels for the game. During development though, I ran into an error while uploading the game to GXC; it would not run online. I researched how to solve this problem and asked on the GameMaker Community forums for an answer. I couldn’t find a solution and the forums said to wait for the next update for the error to be fixed; I didn’t have time as the game jam was going to end soon. To solve this problem, I created a separate game program to isolate the bug. I added code from the main game that likely caused the problem to this test program, then uploaded it online to see if it would run. I repeated this process until I found the solution; the online platformer didn’t support having the level files organized into separate directories. I fixed the error, by placing all the levels in the same directory, and submitted the game to the jam.
</p>

<h2>LEVEL EDITOR</h2>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig9.png' alt='Early version of the level editing program.'/>
    <figcaption>Figure 6: Early version of the level editing program.</figcaption>
</figure>

<p>Figure 9 depicts the song/level editor program I developed. The grid represents the level. Enemies/notes placed on this grid will appear when playing the level. The yellow bar represents the space just in front of the players, where enemies are to be hit. The x-axis of the grid represents quarters of a beat. No enemies are placed in the center row; it’s used for programming a screen shake effect in time with the music. The other red rows are for non-large enemies. The two grey rows are where the player character walks and where large enemies are placed. Enemies placed lower on the grid appear placed lower on the screen during gameplay. The currently selected enemy is rendered fully opaque to show that it is selected. </p>

<p>I will explain the rest of the program's features starting at the top with the "song" button and going clockwise.</p>

<ul>
    <li>
        Song selects what song/level to edit. Save saves the current song/level. Note selects what type of enemy/note will be placed when placing enemies.
    </li>
    <li>
        gridPosX and gridPosY show the coordinates of the selected enemy/note on the visible grid. Grid beat shows on what beat the enemy will be in front of the player character. Notes shows the number of enemies in the level.
    </li>
    <li>
        SelectedNote refers to the enemy/note type currently selected. Beat refers to the beat on which the enemy will be in front of the player character. Row refers to the row of the grid the enemy is in, and the lane it will spawn in during gameplay. SpawnBeatOff and SpawnBeat determines on which beat the enemy is created. Enemies are created off-screen to the right of the level.
    </li>
    <li>
        Under "Song Info" the song's name and BPM are displayed. The name is that of the current song/level and BPM refers to the speed of the song. The song's BPM can be edited by clicking the button with the text "BPM". Toreador is a placeholder song.
    </li>
    <li>
       The text on the top left corner displays more specific information about the song/level.  Of note here is SongPositionInSeconds and SongPositionInBeats. These show how far into the song the player is, measured in seconds and beats respectively.
    </li>
</ul>

<figure>
    <img src= '{{ page.image-folder }}FightcoreFig10.png' alt='Finished level editor with a pop-up displaying end beat.'/>
    <figcaption>Figure 7: Finished version of the level editing program, note the addition of new buttons at the top of the screen. A pop-up window for editing a selected enemy/note's EndBeat, explained below, is opened. It currently shows -100 for testing purposes.</figcaption>
</figure>

<p>
   EndBeat is for large enemies/sustained notes. Larger enemies take multiple hits. EndBeat determines on what beat the enemy will be defeated when hit continuously. 
</p>

<p>
    The four icons at the top of figure 10 display drop-down menus when clicked. These menus are used for setting the environment visuals for the song/level.
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
    <img src= '{{ page.image-folder }}FightcoreFig5.PNG' alt='Main menu.'/>
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