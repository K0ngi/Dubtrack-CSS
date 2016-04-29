/* main css for NB3 Dubtrack Room */
/* reliant on DemoZ css */

/* Imports */
@import url("https://netox005.github.io/Dubtrack/css/voteicons.css"); /* NB3 Vote Icons */
@import url("https://netox005.github.io/Dubtrack/css/chatright.css"); /* Chat completely to the right */
/* @import url("https://netox005.github.io/Dubtrack/css/videosmall.css"); Small video */
@import url("https://rawgit.com/Netox005/Dubtrack/master/css/videosmall.css"); /* Smaller video */
@import url("https://netox005.github.io/Dubtrack/css/skynet.css"); /* @netuxbot custom chat */
@import url("https://netox005.github.io/Dubtrack/css/phonefix.css"); /* Phone Fixes */
@import url("https://netox005.github.io/Dubtrack/css/animations.css"); /* Animations */
@import url("https://krdemoz.github.io/Dubtrack/css/BG-Free/Themes/theme_blue.css"); /* Replacement PlugDJ theme */

/* Video next to chat */
@media screen and (min-width: 72em) {
    #main-room .left_section { left: initial; right: 449px; }
    #main-room .left_section #main_player { border-radius: 0 0 0 1rem; }
}
/* Room size fix */
@media screen and (min-width: 72em) { #main-room .main-room-wrapper { min-height: 0; margin-bottom: 0; } }

/* User banned fix */
#chat .pusher-chat-widget-input p {
    text-align: center;
    font-weight: bold;
    color: #AB0000;
    cursor: default;
    -ms-user-select: none;
    -moz-user-select: none;
    -webkit-user-select: none;
    user-select: none;
    text-transform: uppercase;
}
#chat .pusher-chat-widget-input p::after { content: " (You can't send messages)"; text-transform: none; }

/* Add to playlist fixes */
#addToPlaylistFloatContainer .create-playlist-header .icon-close { position: absolute; top: 15px; right: 15px; }
#addToPlaylistFloatContainer .create-playlist-header .icon-close:hover { color: cyan; }
#addToPlaylistFloatContainer .create-playlist-input { background: #666A6B; border-bottom: 2px solid #878c8e; }
#addToPlaylistFloatContainer .create-playlist-input .playlist-input {
    width: calc(100% - 2.75rem);
    border-right: 1px solid #878C8E;
    border-bottom: none;
}
#addToPlaylistFloatContainer .create-playlist-input .icon-add { top: 4px; }
#addToPlaylistFloatContainer .playlist-list-action { padding-bottom: .5rem; margin-bottom: .75rem; max-height: 352px; }
#addToPlaylistFloatContainer .playlist-list-action li:last-of-type { border-bottom: 1px solid #878c8e; }

/* Room Update Window fixes */
#roomFormUpdate { top: 58px; width: 70rem; margin: 0; padding-right: 1px; border-radius: 0; }
#roomFormUpdate .modal-header h3 { margin: 0; text-align: center; }
#roomFormUpdate .modal-header, #roomFormUpdate .modal-footer { background: rgba(84,86,85,0.8); }

#roomFormUpdate .closebtn { color: white; top: .75rem; }
#roomFormUpdate .closebtn:hover::before { color: cyan; }

#roomFormUpdate .mid { overflow-y: scroll; height: calc(100vh - 58px - 56px - 83px); }

#roomFormUpdate .modal-footer { margin-top: 0; padding: .25rem 1rem; }
#roomFormUpdate .modal-footer button.btn { border: 2px solid #878c8e !important; padding: .5rem .75rem !important; line-height: 1; }

#roomFormUpdate .mid select { padding: 0; }
#roomFormUpdate .mid select option:not(selected) { color: black; }

/* Browser fixes */
#browser.animate { bottom: 3.5rem; padding-top: 110px; }
#browser .browser-content { border-radius: 0; }
span.close-browser { font-size: 1.125rem !important; padding-top: 1.2rem !important; }
span.close-browser:before { content: "\e903"; }

#browser .browser-content .browser-content-header .form .music-type-select .music-type-dropdown span { line-height: .8; }
#browser .browser-content .browser-content-header .form .music-type-select .music-type-dropdown span:hover { background: #6D6D6D;  }
#browser .browser-content .browser-content-header .form .music-type-select .icon-youtube { color: red; }
#browser .browser-content .browser-content-header .form .music-type-select .icon-soundcloud { color: orange; }

/* Chat avatars fix */
/*#chat .chat-container .chat-messages .chat-main li .stream-item-content .image_row { border-radius: 10%; }*/
#chat .chat-container .chat-messages .chat-main li .stream-item-content .image_row > img {
    max-width: none;
    height: 100%;
    display: block;
    margin: auto;
}

/* Twitch Emotes (DubX) size fixes */
img.emoji.twitch-emoji[alt="fishmoley"] { min-width: 2.5rem; } /* fishmoley */
img.emoji.twitch-emoji[alt="yetiz"] { min-width: 3rem; } /* :yetiz: */
img.emoji.twitch-emoji[alt="lenny"] { min-width: 3.5rem; } /* :lenny: */
img.emoji.twitch-emoji[alt="firespeed"] { min-width: 4rem; } /* firespeed */
img.emoji.twitch-emoji[alt="shrug"] { min-width: 5rem; } /* :shrug: */
img.emoji.twitch-emoji[alt="angelthump"], img.emoji.twitch-emoji[alt="taxibro"] { min-width: 4.5rem; } /* :angelthump:, :taxibro: */

/* Profile fixes */
#profileMainSection { top: 3.4rem; min-height: initial; height: calc(100vh - 6.9rem); overflow-y: auto; }
#profileMainSection .profileWrapper { margin-top: 3rem; }
#profileMainSection #profileSidebar #followersEl { margin-bottom: 3rem; }

/* User banned/message deleted fix */
#chat .chat-container .chat-messages .chat-main li.deleted-message .stream-item-content .image_row > img { opacity: .01; }
#chat .chat-container .chat-messages .chat-main li.deleted-message .stream-item-content .image_row::before {
    content: "X";
    position: absolute;
    top: 3px;
    left: 13px;
    font-weight: 900;
    color: red;
    font-size: 1.5rem;
}

/* Other fixes */
.medium { top: 54px !important; } /* Background Fix */
.ps-container .ps-scrollbar-x, .ps-container .ps-scrollbar-y, .ps-container .ps-scrollbar-x-rail:hover .ps-scrollbar-x, .ps-container .ps-scrollbar-y-rail:hover .ps-scrollbar-y { background-color: #B1B1B1 } /* Scrollbars more visible */
#main-menu-left { top: 58px; height: calc(100% - 58px); padding-top: 3rem; } /* Left menu height fix */
#chat .chat-container .chat-messages .chat-main li:not([class^="user-"]) { padding-bottom: .5rem; min-height: initial; } /* No user messages height fix */
#chat .chat-container .chat-messages .chat-main li .activity-row .text img { display: block; } /* Chat images in new bar */
#chat .chat-options .chat-option-buttons span { -webkit-user-select: none; -moz-user-select: none; -ms-user-select: none; user-select: none; } /* No selection on chat options buttons */
@media screen and (min-width: 72em) {
    /* Fixed "Your playlists" title on browser */
    #browser .browser-content .browser-content-main .sidebar .title {
        text-align: center;
        margin-top: 3.5rem;
        padding: 1rem;
    }
    /* HD toggle position */
    #main-room .left_section #main_player .player_sharing .videoquality-el { top: -3px; }
}
#container-room-list .room-item.userRoom { border: 2px solid cadetblue; } /* User room with different color. */
time.timeago { /* Time ago on messages not selectable */
    cursor: default;
    -ms-user-select: none;
    -moz-user-select: none;
    -webkit-user-select: none;
    user-select: none;
}
#avatar-list p.dubs span { font-family: monospace; font-size: 1.2rem } /* User list dubs num position fix */
#chat .chat-main .system, #chat .chat-main .chat-system-loading { color: #0090CC !important; } /* Chat system message color fix */
img.emoji.twitch-emoji[alt="facepalm"] { background-color: white; } /* Facepalm coloring fix */
#chat .chat-container li.isDefault.current-chat-user a.username { color: gold !important; } /* Gold color on user if it's pleb */


/* Other fixes in phone mode */
@media screen and (max-width: 72em) {
    #browser .browser-content .browser-content-main .nano .loading { z-index: 1; } /* Loading not overlapping with buttons */
    #addToPlaylistFloatContainer { border-radius: 0; padding: .5rem 0; background: rgba(84, 86 , 85, .9); } /* Add to playlist fixes */
    #profileMainSection { top: 92px; max-height: calc(100vh - 203px); } /* Profile height fix */
}
