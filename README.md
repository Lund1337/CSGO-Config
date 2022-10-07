//LAUNCH OPTIONS
//
//+fps_max 0 -novid -tickrate 128 -high -threads 8 +fps_max 0 +cl_interp 0 +cl_interp_ratio 1 +rate 128000 +cl_updaterate 128 +cl_cmdrate 128 +mat_queue_mode 2 -freq 144 -refresh 144  -d3d9ex -nojoy -language bananagaming -exec autoexec
//
// cl_clanid 33900349 cheater
// cl_clanid 37972081 ferrari$peek
// cl_clanid 38732118 +strafe
// cl_clanid 38907786 cheater
// cl_clanid 39075102 fuckladders
// cl_clanid 39728278 thighs
// cl_clanid 38498740 very rare
// cl_clanid 40876850 distinct
// cl_clanid 42562526 root
// cl_clanid 42776289 (6)
// cl_clanid 42777634 ($)

echo *************************
echo CONFIG BY LUND#4846
echo *************************

//DEFAULT
cl_clanid 40876850
bind "w" "+forward"
bind "s" "+back"
bind "a" "+moveleft"
bind "d" "+moveright"
bind mwheelup "+jump"
sensitivity  "1"
bind f "+lookatweapon;r_cleardecals"
+cl_show_team_equipment	"1"

//BINDS
bind z +voicerecord
bindtoggle f2 voice_enable
bind f8 "quick prompt" 
bind f9 radio2 //Radio Menu
bind f10 radio //Offline Menu
bind f11 radio1 //Bot Menu
bind "MWHEELDOWN" "+jump"

//COMP
alias "nonulls" "bind w "+clfwd";bind s "+clback";bind a "+clleft";bind d "+clright";sensitivity 1;echo "no nulls(OFF)""
alias "nulls" "bind w "+mfwd";bind s "+mback";bind a "+mleft";bind d "+mright";sensitivity 5;echo "nulls (ON)""

alias +clfwd "+forward;cl_clanid 40876850"
alias +clback "+back;cl_clanid 40876850"
alias +clleft "+moveleft;cl_clanid 40876850"
alias +clright "+moveright;cl_clanid 40876850"
 
alias -clfwd "-forward"
alias -clback "-back"
alias -clleft "-moveleft"
alias -clright "-moveright"

//NULLS
alias checkfwd ""
alias checkback ""
alias checkleft ""
alias checkright ""

alias +mfwd "-back; +forward; alias checkfwd +forward;cl_clanid 40876850"
alias +mback "-forward; +back; alias checkback +back;cl_clanid 40876850"
alias +mleft "-moveright; +moveleft; alias checkleft +moveleft;cl_clanid 40876850"
alias +mright "-moveleft; +moveright; alias checkright +moveright;cl_clanid 40876850"
 
alias -mfwd "-forward; checkback; alias checkfwd"
alias -mback "-back; checkfwd; alias checkback"
alias -mleft "-moveleft; checkright; alias checkleft"
alias -mright "-moveright; checkleft; alias checkright"

//LJ BIND
alias +LJUMP "+duck; +jump; -forward; -back; +klook"
alias -LJUMP "-duck; -jump; -klook"
alias "lj" "bind space "+LJUMP"; echo "LJ (ON)""
alias "nolj" "bind space "+DJUMP"; echo "LJ (OFF)""

//DUCKJUMP
alias +DJUMP "+jump; +duck"
alias -DJUMP "-JUMP; -DUCK"
bind space "+DJUMP"

//AUTOWALK
alias "AUTOWALK" "walk1"
alias "walk1" "+forward;alias AUTOWALK walk2"
alias "walk2" "-forward;alias AUTOWALK walk1"
bind , "AUTOWALK"

//AUTODUCK
alias "AUTODUCK" "duck1"
alias "duck1" "+duck;alias AUTODUCK duck2"
alias "duck2" "-duck;alias AUTODUCK duck1"
bind . "AUTODUCK"

//VIEWMODEL
viewmodel_fov 68
viewmodel_offset_x 2.5
viewmodel_offset_y 0
viewmodel_offset_z -1.5
cl_righthand 1
viewmodel_presetpos 3
cl_viewmodel_shift_left_amt 1.5
cl_viewmodel_shift_right_amt 0.75
viewmodel_recoil 0;cl_bob_lower_amt 5
cl_bobamt_lat 0.4;cl_bobamt_vert 0.25

//CROSSHAIR
cl_crosshairalpha "255"
cl_crosshaircolor "4"
cl_crosshairdot "0"
cl_crosshair_t "0"
cl_crosshairgap "-2.5"
cl_crosshairsize "2"
cl_crosshairstyle "4"
cl_crosshairusealpha "1"
cl_crosshairthickness "0.5"
cl_fixedcrosshairgap "-2.5"
cl_crosshair_outlinethickness "0"
cl_crosshair_drawoutline "0"

//CROSSHAIR LINEUP SMOKE
bind "mouse5" "+crosshairsmoke"
alias "-crosshairsmoke" "cl_crosshairsize 2;cl_crosshairdot 0;cl_crosshairgap -2.5"
alias "+crosshairsmoke" "cl_crosshairsize 1337;cl_crosshairdot 1;cl_crosshairgap 10"

//JUMPTROW
alias "+jumpthrow" "+jump;-attack"
alias "-jumpthrow" "-jump"
bind "h" "+jumpthrow"

//RADAR & HUD
cl_radar_scale 0.4
cl_radar_icon_scale_min 0.1
cl_hud_radar_scale 1.2
cl_crosshair_sniper_width 1

//NETGRAPH WITH OPEN TAB
alias +netg "net_graph 1;+showscores"
alias -netg "net_graph 0;-showscores"
bind TAB "+netg"

//FPS
fps_max 0
fps_max_menu 0

//GAMESENSE ANIMATED TAG
alias "tagnl" "bind mwheelup "2001";cl_clanid "0";echo "TAG NL(ON)""
alias "taggs" "bind mwheelup "1001";cl_clanid "0";echo "TAG GS(ON)""
alias "tagoff" "bind mwheelup "+jump";cl_clanid "0";echo "TAG (OFF)""

alias "1001" "cl_clanid 39977687; bind "mwheelup" 1002; //g
alias "1002" "cl_clanid 39977699; bind "mwheelup" 1003; //ga
alias "1003" "cl_clanid 39977700; bind "mwheelup" 1004; //gam
alias "1004" "cl_clanid 39977705; bind "mwheelup" 1005; //game
alias "1005" "cl_clanid 39977711; bind "mwheelup" 1006; //games
alias "1006" "cl_clanid 39977712; bind "mwheelup" 1007; //gamese
alias "1007" "cl_clanid 39977715; bind "mwheelup" 1008; //gamesen
alias "1008" "cl_clanid 39977722; bind "mwheelup" 1009; //gamesens
alias "1009" "cl_clanid 35053740; bind "mwheelup" 1010; //gamesense
alias "1010" "cl_clanid 39977746; bind "mwheelup" 1011; //amesense
alias "1011" "cl_clanid 39977748; bind "mwheelup" 1012; //mesense
alias "1012" "cl_clanid 39977802; bind "mwheelup" 1013; //esense
alias "1013" "cl_clanid 39977803; bind "mwheelup" 1014; //sense
alias "1014" "cl_clanid 39977804; bind "mwheelup" 1015; //ense
alias "1015" "cl_clanid 39977805; bind "mwheelup" 1016; //nse
alias "1016" "cl_clanid 39977806; bind "mwheelup" 1017; //se
alias "1017" "cl_clanid 39977808; bind "mwheelup" 1018; //e
alias "1018" "cl_clanid 0; bind "mwheelup" "1001" //empty

//JOIN THESE GROUPS
//https://steamcommunity.com/groups/g_-
//https://steamcommunity.com/groups/ga_-
//https://steamcommunity.com/groups/gam_-
//https://steamcommunity.com/groups/game_-
//https://steamcommunity.com/groups/games_-ense
//https://steamcommunity.com/groups/gamese_-
//https://steamcommunity.com/groups/gamesen_-
//https://steamcommunity.com/groups/gamesens_-
//https://steamcommunity.com/groups/gameaimsense
//https://steamcommunity.com/groups/amesense_-
//https://steamcommunity.com/groups/mesense_-
//https://steamcommunity.com/groups/esense_-
//https://steamcommunity.com/groups/sense_-
//https://steamcommunity.com/groups/ense_-
//https://steamcommunity.com/groups/nse_-
//https://steamcommunity.com/groups/se_-
//https://steamcommunity.com/groups/e_-

//NEVERLOSE ANIMATED TAG
alias "2001" "cl_clanid 42636535; bind "mwheelup" 2002; //|
alias "2002" "cl_clanid 0; bind "mwheelup" 2003; //empty
alias "2003" "cl_clanid 42636547; bind "mwheelup" 2004; //N
alias "2004" "cl_clanid 42636547; bind "mwheelup" 2005; //N
alias "2005" "cl_clanid 42636551; bind "mwheelup" 2006; //N3
alias "2006" "cl_clanid 42636553; bind "mwheelup" 2007; //Ne
alias "2007" "cl_clanid 42636555; bind "mwheelup" 2008; //Ne\
alias "2008" "cl_clanid 42636557; bind "mwheelup" 2009; //Ne\/
alias "2009" "cl_clanid 42636559; bind "mwheelup" 2010; //Nev
alias "2010" "cl_clanid 42636562; bind "mwheelup" 2011; //Nev3
alias "2011" "cl_clanid 42636567; bind "mwheelup" 2012; //Neve
alias "2012" "cl_clanid 42636567; bind "mwheelup" 2013; //Neve|
alias "2013" "cl_clanid 42636600; bind "mwheelup" 2014; //Neve|2
alias "2014" "cl_clanid 42636605; bind "mwheelup" 2015; //Never|
alias "2015" "cl_clanid 42636606; bind "mwheelup" 2016; //Never|_
alias "2016" "cl_clanid 42636607; bind "mwheelup" 2017; //Neverl
alias "2017" "cl_clanid 42636608; bind "mwheelup" 2018; //Neverl0
alias "2018" "cl_clanid 42636610; bind "mwheelup" 2019; //Neverlo
alias "2019" "cl_clanid 42636611; bind "mwheelup" 2020; //Neverlo5
alias "2020" "cl_clanid 42636612; bind "mwheelup" 2021; //Neverlos
alias "2021" "cl_clanid 42636613; bind "mwheelup" 2022; //Neverlos3
alias "2022" "cl_clanid 42636615; bind "mwheelup" 2023; //Neverlose
alias "2023" "cl_clanid 42636828; bind "mwheelup" 2024; //Neverlose.
alias "2024" "cl_clanid 42636666; bind "mwheelup" 2025; //Neverlose.>
alias "2025" "cl_clanid 42636660; bind "mwheelup" 2026; //Neverlose.c>
alias "2026" "cl_clanid 42646846; bind "mwheelup" 2027; //Neverlose.cc
alias "2027" "cl_clanid 42636660; bind "mwheelup" 2028; //Neverlose.c>
alias "2028" "cl_clanid 42636666; bind "mwheelup" 2029; //Neverlose.>
alias "2029" "cl_clanid 42636828; bind "mwheelup" 2030; //Neverlose.
alias "2030" "cl_clanid 42636615; bind "mwheelup" 2031; //Neverlose
alias "2031" "cl_clanid 42636613; bind "mwheelup" 2032; //Neverlos3
alias "2032" "cl_clanid 42636612; bind "mwheelup" 2033; //Neverlos
alias "2033" "cl_clanid 42636734; bind "mwheelup" 2034; //Neverlo_
alias "2034" "cl_clanid 42636611; bind "mwheelup" 2035; //Neverlo5
alias "2035" "cl_clanid 42636610; bind "mwheelup" 2036; //Neverlo
alias "2036" "cl_clanid 42636716; bind "mwheelup" 2037; //Neverl_
alias "2037" "cl_clanid 42636720; bind "mwheelup" 2038; //Never|0
alias "2038" "cl_clanid 42636605; bind "mwheelup" 2039; //Never|
alias "2039" "cl_clanid 42636600; bind "mwheelup" 2040; //Neve|2
alias "2040" "cl_clanid 42636567; bind "mwheelup" 2041; //Neve|
alias "2041" "cl_clanid 42636567; bind "mwheelup" 2042; //Neve
alias "2042" "cl_clanid 42636562; bind "mwheelup" 2043; //Nev3
alias "2043" "cl_clanid 42636559; bind "mwheelup" 2044; //Nev
alias "2044" "cl_clanid 42636557; bind "mwheelup" 2045; //Ne\/
alias "2045" "cl_clanid 42636555; bind "mwheelup" 2046; //Ne\
alias "2046" "cl_clanid 42636553; bind "mwheelup" 2047; //Ne
alias "2047" "cl_clanid 42636551; bind "mwheelup" 2048; //N3
alias "2048" "cl_clanid 42636547; bind "mwheelup" 2049; //N
alias "2049" "cl_clanid 42636724; bind "mwheelup" 2050; //|\|
alias "2050" "cl_clanid 0; bind "mwheelup" "2001" //empty

//JOIN THESE GROUPS
//https://steamcommunity.com/groups/nl1_
//https://steamcommunity.com/groups/nl2_
//https://steamcommunity.com/groups/nl3_
//https://steamcommunity.com/groups/nl4_
//https://steamcommunity.com/groups/nl5_
//https://steamcommunity.com/groups/nl6_
//https://steamcommunity.com/groups/nl7_
//https://steamcommunity.com/groups/nl8_
//https://steamcommunity.com/groups/nl9_
//https://steamcommunity.com/groups/nl10_
//https://steamcommunity.com/groups/nl11_
//https://steamcommunity.com/groups/n112_
//https://steamcommunity.com/groups/n113_
//https://steamcommunity.com/groups/n114_
//https://steamcommunity.com/groups/n115_
//https://steamcommunity.com/groups/nl16_
//https://steamcommunity.com/groups/nl17_
//https://steamcommunity.com/groups/nl18_
//https://steamcommunity.com/groups/nl19_
//https://steamcommunity.com/groups/nl20_
//https://steamcommunity.com/groups/nl21_
//https://steamcommunity.com/groups/nl22_
//https://steamcommunity.com/groups/nl23_
//https://steamcommunity.com/groups/nl24_
//https://steamcommunity.com/groups/nl25_
//https://steamcommunity.com/groups/nl26_
//https://steamcommunity.com/groups/nl27_

//CHATWHEEL
cl_radial_radio_tab_0_text_1 #Chatwheel_midplan
cl_radial_radio_tab_0_text_2 #Chatwheel_bplan
cl_radial_radio_tab_0_text_3 Throw from here";player_ping
cl_radial_radio_tab_0_text_4 #Chatwheel_negative
cl_radial_radio_tab_0_text_5 #Chatwheel_requestweapon    
cl_radial_radio_tab_0_text_6 #Chatwheel_affirmative
cl_radial_radio_tab_0_text_7 Area Clear";player_ping
cl_radial_radio_tab_0_text_8 #Chatwheel_aplan
cl_radial_radio_tab_0_text_1 #Chatwheel_midplan
cl_radial_radio_tab_0_text_2 #Chatwheel_bplan
cl_radial_radio_tab_0_text_3 Throw from here";player_ping
cl_radial_radio_tab_0_text_4 #Chatwheel_negative
cl_radial_radio_tab_0_text_5 #Chatwheel_requestweapon    
cl_radial_radio_tab_0_text_6 #Chatwheel_affirmative
cl_radial_radio_tab_0_text_7 Area Clear";player_ping
cl_radial_radio_tab_0_text_8 #Chatwheel_aplan

//SAVE CONFIG
echo "LOADING..."
echo *************************
echo "CONFIG LOADED"
echo *************************
host_writeconfig
