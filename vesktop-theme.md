/**
 * @name system24 (Spotify Dark Edition - Avatar Fix - For Disocrd)
 * @description a tui-style discord theme with spotify-inspired colors and fixed user avatar.
 * @author refact0r (mod by Willnux)
 * @version 2.3.0
 */

/* 1. IMPORTING THE BASE THEME */
@import url('https://refact0r.github.io/system24/build/system24.css');

body {
    --font: 'DM Mono'; 
    --code-font: 'DM Mono'; 
    font-weight: 300; 
    letter-spacing: -0.05ch; 

    /* sizes */
    --gap: 12px; 
    --divider-thickness: 4px; 
    --border-thickness: 2px; 
    --border-hover-transition: 0.2s ease; 

    /* animation/transition options */
    --animations: on; 
    --list-item-transition: 0.2s ease; 
    --dms-icon-svg-transition: 0.4s ease; 

    /* top bar options */
    --top-bar-height: var(--gap); 
    --top-bar-button-position: titlebar; 
    --top-bar-title-position: off; 
    --subtle-top-bar-title: off; 

    /* window controls */
    --custom-window-controls: off; 
    --window-control-size: 14px; 

    /* dms button options */
    --custom-dms-icon: off;
    --dms-icon-svg-url: url(''); 
    --dms-icon-svg-size: 90%; 
    --dms-icon-color-before: var(--icon-subtle); 
    --dms-icon-color-after: var(--white); 
    --custom-dms-background: off; 
    --dms-background-image-url: url(''); 
    --dms-background-image-size: cover; 
    --dms-background-color: transparent; 

    /* background image options */
    --background-image: off; 
    --background-image-url: url(''); 

    /* transparency/blur options */
    --transparency-tweaks: off; 
    --remove-bg-layer: off; 
    --panel-blur: off; 
    --blur-amount: 12px; 
    --bg-floating: var(--bg-3); 

    /* other options */
    --small-user-panel: on; 

    /* unrounding options */
    --unrounding: on; 

    /* styling options */
    --custom-spotify-bar: on; 
    --ascii-titles: on; 
    --ascii-loader: system24; 

    /* panel labels */
    --panel-labels: on; 
    --label-color: var(--green-2); 
    --label-font-weight: 500; 
}

/* 2. theme Spotify for Discord */
:root {
    --colors: on; 

    /* text colors */
    --text-0: #000000; 
    --text-1: #ffffff; 
    --text-2: #ffffff; 
    --text-3: #b3b3b3; 
    --text-4: #a7a7a7; 
    --text-5: #535353; 

    /* background and dark colors */
    --bg-1: #282828; 
    --bg-2: #181818; 
    --bg-3: #000000; 
    --bg-4: #121212; 
    
    --hover: hsla(141, 73%, 42%, 0.1); 
    --active: hsla(141, 73%, 42%, 0.2); 
    --active-2: hsla(141, 73%, 42%, 0.3); 
    --message-hover: hsla(0, 0%, 100%, 0.05); 

    /* accent colors */
    --accent-1: var(--green-2); 
    --accent-2: var(--green-2); 
    --accent-3: var(--green-3); 
    --accent-4: var(--green-4); 
    --accent-5: var(--green-5); 
    --accent-new: var(--green-2); 
    
    --mention: linear-gradient(to right, rgba(29, 185, 84, 0.1) 40%, transparent); 
    --mention-hover: linear-gradient(to right, rgba(29, 185, 84, 0.15) 40%, transparent); 

    /* status indicator colors */
    --online: #1db954; 
    --dnd: #e91429; 
    --idle: #ffa42b; 
    --streaming: #1db954; 
    --offline: #727272; 

    /* border colors */
    --border-light: #282828; 
    --border: #333333; 
    --border-hover: var(--green-2); 
    --button-border: rgba(255, 255, 255, 0.1); 

    /* Spotify Greens Palette */
    --green-1: hsl(141, 73%, 52%);
    --green-2: #1db954; 
    --green-3: #1ed760; 
    --green-4: #179443; 
    --green-5: #117033;

    /* Keep others for compatibility, but neutralized */
    --red-1: #e91429; --red-2: #e91429;
    --blue-1: #4d91ff; --blue-2: #4d91ff;
    --yellow-1: #ffa42b; --yellow-2: #ffa42b;
    --purple-1: var(--green-2); --purple-2: var(--green-2);
}

/* =========================================================
   3. FIX (Icon Discord msj direct)
   ========================================================= */

.tutorialContainer-2jwoS5 .homeIcon-t5ZfO3,
.tutorialContainer-2jwoS5 .foreignIcon-1_AbGj {
    display: none !important;
}

.tutorialContainer-2jwoS5 .childWrapper-1j_1ub {
    background-image: url('https://cdn.discordapp.com/avatars/508863359777505290/a_66f443584d4128f6d78207f2.png') !important;
    background-size: cover !important;
    background-position: center !important;
    background-repeat: no-repeat !important;
    border-radius: 0 !important;
    background-color: transparent !important;
}

.tutorialContainer-2jwoS5:hover .childWrapper-1j_1ub {
    box-shadow: 0 0 0 2px var(--green-2) !important;
}
