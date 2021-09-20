# L4D2-Autoexec
Just personal setting.  








echo;
echo "Exicing autoexec.cfg";


// =============
// Miscellaneous
// =============

//exec cjt.cfg
alias load_fonts "mat_setvideomode 1728 1080 1; mat_setvideomode 1728 1080 0"
load_fonts
bind o "say_team !tank;say_team !health;say_team !cur"
bind F3 "say_team wait"
bind F4 "say_team go"


cl_downloadfilter "all";		// Disables custom server content download. (Default: all)
cl_ideal_spec_mode "6";			// Sets the default spectator mode to free roam. (Default: 5)
cl_timeout "30";			// Disconnects from a server after 30 seconds of timeout. (Default: 60)
closecaption "1";			// Enables captioning. (Default: 0)
con_enable "1";				// Enables the console. (Default: 0)
dsp_enhance_stereo "1";			// Sets the audio quality to high. (Default: 0)
// gameinstructor_enable "0";		// Disables the game instructor. (Default: 1)
mat_grain_scale_override "0.0";		// Disables the film grain effect. (Default: 1.0)
mm_dedicated_search_maxping "80";	// Restricts public server searches to a maximum ping of 80. (Default: 150)
// sensitivity "3";			// Controls the in-game mouse sensitivity. (Default: 3)
spec_allowroaming "1";			// Allows free spectator roaming. (Default: 0)
voice_enable "1";			// Enables voice-ingame. (Default: 1)
voice_modenable "1";			// Enables voice-ingame. (Default: 1)
voice_scale "1";			// Sets the voice-ingame receive volume to the maximum. (Default: 0.7)


// ===================
// Connection Settings
// ===================

//cl_updaterate 100
//cl_cmdrate 100
//rate 100000
//cl_interp_ratio -1
//cl_lagcompensation 1
//cl_resend 4

		// Definition of the five different lerp options.
alias "lerp_0" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0;cl_interp_ratio -1;alias lerp_change lerp_16.7;echo Lerp set to 0 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0, cl_interp_ratio -1).";
alias "lerp_16.7" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0167;cl_interp_ratio -1;alias lerp_change lerp_33.4;echo Lerp set to 16.7 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0167, cl_interp_ratio -1).";
alias "lerp_33.4" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0334;cl_interp_ratio -1;alias lerp_change lerp_50.1;echo Lerp set to 33.4 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0334, cl_interp_ratio -1).";
alias "lerp_50.1" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0501;cl_interp_ratio -1;alias lerp_change lerp_66.7;echo Lerp set to 50.1 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0501, cl_interp_ratio -1).";
alias "lerp_66.7" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0667;cl_interp_ratio -1;alias lerp_change lerp_0;echo Lerp set to 66.7 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0667, cl_interp_ratio -1).";

lerp_0;	// Loading of one of the five different lerp options. Change the value here to use a different lerp.

		// Additional rates presets mainly for testing purposes and changing settings quickly via the console. You can normally ignore these, just use the above.
alias "rd" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.1;cl_interp_ratio 2;echo Shitty default rates providing lerp 100 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.1, cl_interp_ratio 2) set.";
alias "rd+" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.1;cl_interp_ratio -1;echo Improved default rates while still providing shitty lerp 100 (rate 30000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.1, cl_interp_ratio -1) set.";
alias "rc1" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0667;cl_interp_ratio -1;echo Custom rates preset #1 providing lerp 66.7 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0667, cl_interp_ratio -1) set.";
alias "rc2" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0334;cl_interp_ratio -1;echo Custom rates preset #2 providing lerp 33.4 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0334, cl_interp_ratio -1) set.";
alias "rc3" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0;cl_interp_ratio 1-;echo Custom rates preset #3 providing lerp 0 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0, cl_interp_ratio -1) set.";
alias "rc4" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0334;cl_interp_ratio -1;echo Custom rates preset #4 providing lerp 33.4 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0334, cl_interp_ratio -1) set.";
alias "rc5" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0167;cl_interp_ratio -1;echo Custom rates preset #5 providing lerp 16.7 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0167, cl_interp_ratio -1) set.";
alias "rc6" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0;cl_interp_ratio -1;echo Custom rates preset #6 providing lerp 0 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0, cl_interp_ratio -1) set.";
alias "rc7" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.02;cl_interp_ratio -1;echo Custom rates preset #7 providing lerp 20 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.02, cl_interp_ratio -1) set.";
alias "rc8" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.01;cl_interp_ratio -1;echo Custom rates preset #8 providing lerp 10 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.01, cl_interp_ratio -1) set.";
alias "rc9" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0;cl_interp_ratio -1;echo Custom rates preset #9 providing lerp 0 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0, cl_interp_ratio -1) set.";
alias "rc10" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0667;cl_interp_ratio -1;echo Custom rates preset #10 providing lerp 66.7 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0667, cl_interp_ratio -1) set.";
alias "rc11" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0501;cl_interp_ratio -1;echo Custom rates preset #11 providing lerp 50.1 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0501, cl_interp_ratio -1) set.";
alias "rc12" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0334;cl_interp_ratio -1;echo Custom rates preset #12 providing lerp 33.4 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0334, cl_interp_ratio -1) set.";
alias "rc13" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0167;cl_interp_ratio -1;echo Custom rates preset #13 providing lerp 16.7 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0167, cl_interp_ratio -1) set.";
alias "rc14" "rate 100000;cl_cmdrate 100;cl_updaterate 100;cl_interp 0.0;cl_interp_ratio -1;echo Custom rates preset #14 providing lerp 0 (rate 100000, cl_cmdrate 100, cl_updaterate 100, cl_interp 0.0, cl_interp_ratio -1) set.";


//Crosshair


cl_crosshair_dynamic "0"
cl_crosshair_thickness "2"
cl_crosshair_red "255"
cl_crosshair_blue "0"
cl_crosshair_green "255"


//Sound


dsp_enhance_stereo 1
dsp_slow_cpu 1
snd_async_fullyasync 1
snd_digital_surround 1
snd_legacy_surround 0
snd_mix_async 1
snd_prefetch_common 1
snd_pitchquality 1
snd_spatialize_roundrobin 1


//Anti-Cheat


c_thirdpersonshoulder "0"   
cl_thirdpersonshoulder "0"  

//Visuals


cl_viewmodelfovsurvivor "90"




//Performance


func_break_max_pieces "0"
cl_phys_timescale "1.0"  
cl_bobup "0"
cl_forcepreload "1"
cl_detail_max_sway "0"
cl_predictweapons "1"
cl_detail_avoid_force "0"
cl_detail_avoid_radius "0"
cl_detail_avoid_recover_speed "0"
cl_detail_max_sway "0"
cl_lagcompensation "1"
cl_observercrosshair "1"
r_ambientfraction "0.2"
r_cheapwaterend "1"
r_cheapwaterstart "1"
r_dynamic "0"
r_eyemove  "0"
r_eyesize "0"
r_eyeshift_x "0"
r_eyeshift_y "0"
r_eyeshift_z "0"
r_PhysPropStaticLighting "0"
r_radiosity "4"
mat_bloom_scalefactor_scalar "0"
mat_monitorgamma "1.6"
mat_monitorgamma_tv_enabled "1"
mat_viewportscale "1"
props_break_max_pieces "0"
props_break_max_pieces_perframe "0"
muzzleflash_light "1"
adsp_debug "0"


cl_glow_ghost_infected_r "1.00"                                 // COLOR OF INFECTED GHOST:                     "WHITE"
cl_glow_ghost_infected_g "1.00"                                 // Only Survivor View
cl_glow_ghost_infected_b "1.00"                                 // -
cl_glow_infected_r "0.00"                                       // COLOR OF INFECTED TEAM MATE:                 "BLUE"
cl_glow_infected_g "0.25"                                       // Only Infected View
cl_glow_infected_b "1.00"                                       // -
cl_glow_survivor_r "0.00"                                       // COLOR OF SURVIVOR TEAM MATE:                 "BLUE"
cl_glow_survivor_g "0.25"                                       // Only Survivor View
cl_glow_survivor_b "1.00"                                       // -
cl_glow_survivor_health_high_r "0.00"                           // COLOR OF SURVIVORS WITH HIGH HEALTH:         "GREEN"
cl_glow_survivor_health_high_g "1.00"                           // Only Infected View
cl_glow_survivor_health_high_b "0.00"                           // -
cl_glow_survivor_health_med_r "1.00"                            // COLOR OF SURVIVORS WITH MEDIUM HEALTH:       "YELLOW"
cl_glow_survivor_health_med_g "0.75"                            // Only Infected View
cl_glow_survivor_health_med_b "0.00"                            // -
cl_glow_survivor_health_low_r "1.00"                            // COLOR OF SURVIVORS WITH LOW HEALTH:          "ORANGE"
cl_glow_survivor_health_low_g "0.25"                            // Only Infected View
cl_glow_survivor_health_low_b "0.00"                            // -
cl_glow_survivor_health_crit_r "1.00"                           // COLOR OF SURVIVOR WHEN INCAPACITATED:        "RED"
cl_glow_survivor_health_crit_g "0.00"                           // Only Infected View
cl_glow_survivor_health_crit_b "0.00"                           // -
cl_glow_survivor_hurt_r "1.00"                                  // COLOR OF SURVIVOR WHEN INCAPACITATED:        "RED"
cl_glow_survivor_hurt_g "0.00"                                  // Only Survivor View
cl_glow_survivor_hurt_b "0.00"                                  // -
cl_glow_survivor_vomit_r "0.50"                                 // COLOR OF SURVIVORS WHEN PUKED:               "PURPLE"
cl_glow_survivor_vomit_g "0.00"                                 // Only Infected View
cl_glow_survivor_vomit_b "1.00"                                 // -
cl_glow_infected_vomit_r "0.50"                                 // COLOR OF SURVIVORS WHEN PUKED:               "PURPLE"
cl_glow_infected_vomit_g "0.00"                                 // Only Infected View
cl_glow_infected_vomit_b "1.00"                                 // -
cl_glow_item_r "1.00"                                           // COLOR OF ITEMS IN RANGE:                     "ORANGE"
cl_glow_item_g "0.25"                                           // Both Survivor & Infected View
cl_glow_item_b "0.00"                                           // -
cl_glow_item_far_r "1.00"                                       // COLOR OF ITEMS OUT OF RANGE:                 "ORANGE"
cl_glow_item_far_g "0.25"                                       // Both Survivor & Infected View
cl_glow_item_far_b "0.00"                                       // -
cl_glow_thirdstrike_item_r "1.00"                               // COLOR OF ITEMS WHILE BLACK & WHITE:          "ORANGE"
cl_glow_thirdstrike_item_g "0.25"                               // Only Survivor View
cl_glow_thirdstrike_item_b "0.00"                               // -


// Misc


cl_predict "1"
cl_predictweapons "1"
cl_showpluginmessages "0"
con_enable "1"


// =====================
// Scoreboard & Netgraph
// =====================

net_graph 1


// ============================
// Force Dedicated Lobby Server
// ============================

	// These are some European confogl servers that you can force from a lobby with the appropriate console command (pixie, l4d2tv or pwg). While these are normally used by random people,
	// keep in mind nevertheless that just because you are able to connect to a server, it does not automatically mean that you are also allowed to use it for matches,
	// so use these at your own discretion. Also, the IPs might not be correct anymore after some time if the owners change servers.


// ===================
// Server Status Check
// ===================

	// The server status check script is split up into multiple aliases because it is too long for a single alias.
alias "server_status_check" "server_status_check_1";
alias "server_status_check_1" "toggleconsole;wait 50;echo;echo;wait 5;echo ================================================================================;wait 5;echo;wait 5;server_status_check_2";
alias "server_status_check_2" "status;wait 50;echo;server_status_check_3";
alias "server_status_check_3" "sv_minrate;sv_maxrate;sv_mincmdrate;sv_maxcmdrate;help sv_minupdaterate;help sv_maxupdaterate;help sv_client_min_interp_ratio;help sv_client_max_interp_ratio;echo;server_status_check_4";
alias "server_status_check_4" "meta list;wait 50;echo;wait 5;server_status_check_5";
alias "server_status_check_5" "sm plugins;sm plugins 11;sm plugins 22;sm plugins 33;sm plugins 44;sm plugins 55;sm plugins 66;sm plugins 77;sm plugins 88;sm plugins 99;wait 50;echo;wait 5;server_status_check_6";
alias "server_status_check_6" "confogl_clientsettings;wait 50;echo;server_status_check_7";
alias "server_status_check_7" "confogl_cvardiff;wait 50;echo;wait 5;server_status_check_8";
alias "server_status_check_8" "echo ================================================================================;wait 5;echo;echo";


// =======================
// Thirdperson View & Zoom
// =======================

cam_ideallag "0";			// Third person camera adjustments to allow better look & aiming.
cam_idealyaw "0";			//
cam_idealdelta "4";			//
cam_idealpitch "0";			//
c_thirdpersonshoulderaimdist "720";	//
c_thirdpersonshoulderdist "40";		//
c_thirdpersonshoulderheight "10";	//
c_thirdpersonshoulderoffset "0";	//

alias "thirdperson_defaultzoom" "thirdperson_zoom_100";
alias "thirdperson_on" "firstperson;thirdpersonshoulder;bind mwheelup thirdperson_zoom_in;bind mwheeldown thirdperson_zoom_out;thirdperson_defaultzoom;alias thirdperson_toggle thirdperson_off";
alias "thirdperson_off" "firstperson;bind mwheelup invprev;bind mwheeldown invnext;alias thirdperson_toggle thirdperson_on";

alias "thirdperson_zoom_30" "cam_idealdist 30;alias thirdperson_zoom_in thirdperson_zoom_30;alias thirdperson_zoom_out thirdperson_zoom_35";
alias "thirdperson_zoom_35" "cam_idealdist 35;alias thirdperson_zoom_in thirdperson_zoom_30;alias thirdperson_zoom_out thirdperson_zoom_40";
alias "thirdperson_zoom_40" "cam_idealdist 40;alias thirdperson_zoom_in thirdperson_zoom_35;alias thirdperson_zoom_out thirdperson_zoom_45";
alias "thirdperson_zoom_45" "cam_idealdist 45;alias thirdperson_zoom_in thirdperson_zoom_40;alias thirdperson_zoom_out thirdperson_zoom_50";
alias "thirdperson_zoom_50" "cam_idealdist 50;alias thirdperson_zoom_in thirdperson_zoom_45;alias thirdperson_zoom_out thirdperson_zoom_55";
alias "thirdperson_zoom_55" "cam_idealdist 55;alias thirdperson_zoom_in thirdperson_zoom_50;alias thirdperson_zoom_out thirdperson_zoom_60";
alias "thirdperson_zoom_60" "cam_idealdist 60;alias thirdperson_zoom_in thirdperson_zoom_55;alias thirdperson_zoom_out thirdperson_zoom_65";
alias "thirdperson_zoom_65" "cam_idealdist 65;alias thirdperson_zoom_in thirdperson_zoom_60;alias thirdperson_zoom_out thirdperson_zoom_70";
alias "thirdperson_zoom_70" "cam_idealdist 70;alias thirdperson_zoom_in thirdperson_zoom_65;alias thirdperson_zoom_out thirdperson_zoom_75";
alias "thirdperson_zoom_75" "cam_idealdist 75;alias thirdperson_zoom_in thirdperson_zoom_70;alias thirdperson_zoom_out thirdperson_zoom_80";
alias "thirdperson_zoom_80" "cam_idealdist 80;alias thirdperson_zoom_in thirdperson_zoom_75;alias thirdperson_zoom_out thirdperson_zoom_85";
alias "thirdperson_zoom_85" "cam_idealdist 85;alias thirdperson_zoom_in thirdperson_zoom_80;alias thirdperson_zoom_out thirdperson_zoom_90";
alias "thirdperson_zoom_90" "cam_idealdist 90;alias thirdperson_zoom_in thirdperson_zoom_85;alias thirdperson_zoom_out thirdperson_zoom_95";
alias "thirdperson_zoom_95" "cam_idealdist 95;alias thirdperson_zoom_in thirdperson_zoom_90;alias thirdperson_zoom_out thirdperson_zoom_100";
alias "thirdperson_zoom_100" "cam_idealdist 100;alias thirdperson_zoom_in thirdperson_zoom_95;alias thirdperson_zoom_out thirdperson_zoom_105";
alias "thirdperson_zoom_105" "cam_idealdist 105;alias thirdperson_zoom_in thirdperson_zoom_100;alias thirdperson_zoom_out thirdperson_zoom_110";
alias "thirdperson_zoom_110" "cam_idealdist 110;alias thirdperson_zoom_in thirdperson_zoom_105;alias thirdperson_zoom_out thirdperson_zoom_115";
alias "thirdperson_zoom_115" "cam_idealdist 115;alias thirdperson_zoom_in thirdperson_zoom_110;alias thirdperson_zoom_out thirdperson_zoom_120";
alias "thirdperson_zoom_120" "cam_idealdist 120;alias thirdperson_zoom_in thirdperson_zoom_115;alias thirdperson_zoom_out thirdperson_zoom_125";
alias "thirdperson_zoom_125" "cam_idealdist 135;alias thirdperson_zoom_in thirdperson_zoom_120;alias thirdperson_zoom_out thirdperson_zoom_130";
alias "thirdperson_zoom_130" "cam_idealdist 130;alias thirdperson_zoom_in thirdperson_zoom_125;alias thirdperson_zoom_out thirdperson_zoom_135";
alias "thirdperson_zoom_135" "cam_idealdist 135;alias thirdperson_zoom_in thirdperson_zoom_130;alias thirdperson_zoom_out thirdperson_zoom_140";
alias "thirdperson_zoom_140" "cam_idealdist 140;alias thirdperson_zoom_in thirdperson_zoom_135;alias thirdperson_zoom_out thirdperson_zoom_145";
alias "thirdperson_zoom_145" "cam_idealdist 145;alias thirdperson_zoom_in thirdperson_zoom_140;alias thirdperson_zoom_out thirdperson_zoom_150";
alias "thirdperson_zoom_150" "cam_idealdist 150;alias thirdperson_zoom_in thirdperson_zoom_145;alias thirdperson_zoom_out thirdperson_zoom_155";
alias "thirdperson_zoom_155" "cam_idealdist 155;alias thirdperson_zoom_in thirdperson_zoom_150;alias thirdperson_zoom_out thirdperson_zoom_160";
alias "thirdperson_zoom_160" "cam_idealdist 160;alias thirdperson_zoom_in thirdperson_zoom_155;alias thirdperson_zoom_out thirdperson_zoom_165";
alias "thirdperson_zoom_165" "cam_idealdist 165;alias thirdperson_zoom_in thirdperson_zoom_160;alias thirdperson_zoom_out thirdperson_zoom_170";
alias "thirdperson_zoom_170" "cam_idealdist 170;alias thirdperson_zoom_in thirdperson_zoom_165;alias thirdperson_zoom_out thirdperson_zoom_175";
alias "thirdperson_zoom_175" "cam_idealdist 175;alias thirdperson_zoom_in thirdperson_zoom_170;alias thirdperson_zoom_out thirdperson_zoom_180";
alias "thirdperson_zoom_180" "cam_idealdist 180;alias thirdperson_zoom_in thirdperson_zoom_175;alias thirdperson_zoom_out thirdperson_zoom_185";
alias "thirdperson_zoom_185" "cam_idealdist 185;alias thirdperson_zoom_in thirdperson_zoom_180;alias thirdperson_zoom_out thirdperson_zoom_190";
alias "thirdperson_zoom_190" "cam_idealdist 190;alias thirdperson_zoom_in thirdperson_zoom_185;alias thirdperson_zoom_out thirdperson_zoom_195";
alias "thirdperson_zoom_195" "cam_idealdist 195;alias thirdperson_zoom_in thirdperson_zoom_190;alias thirdperson_zoom_out thirdperson_zoom_200";
alias "thirdperson_zoom_200" "cam_idealdist 200;alias thirdperson_zoom_in thirdperson_zoom_195;alias thirdperson_zoom_out thirdperson_zoom_200";

alias "thirdperson_toggle" "thirdperson_on";


// =======================
// Demo Playback Timescale
// =======================

alias "demo_timescale_binds_on" "bind mwheelup demo_timescale_up;bind mwheeldown demo_timescale_down;bind mouse3 demo_timescale_1;alias demo_timescale_binds_toggle demo_timescale_binds_off;demo_timescale_1;echo Demo playback timescale binds turned ON.";
alias "demo_timescale_binds_off" "bind mwheelup invprev;bind mwheeldown invnext;bind mouse3 +zoom;alias demo_timescale_binds_toggle demo_timescale_binds_on;demo_timescale_1;echo Demo playback timescale binds turned OFF.";

alias "demo_timescale_75" "demo_timescale 75;alias demo_timescale_up demo_timescale_75;alias demo_timescale_down demo_timescale_50";
alias "demo_timescale_50" "demo_timescale 50;alias demo_timescale_up demo_timescale_75;alias demo_timescale_down demo_timescale_25";
alias "demo_timescale_25" "demo_timescale 25;alias demo_timescale_up demo_timescale_50;alias demo_timescale_down demo_timescale_10";
alias "demo_timescale_10" "demo_timescale 10;alias demo_timescale_up demo_timescale_25;alias demo_timescale_down demo_timescale_7.5";
alias "demo_timescale_7.5" "demo_timescale 7.5;alias demo_timescale_up demo_timescale_10;alias demo_timescale_down demo_timescale_5";
alias "demo_timescale_5" "demo_timescale 5;alias demo_timescale_up demo_timescale_7.5;alias demo_timescale_down demo_timescale_4";
alias "demo_timescale_4" "demo_timescale 4;alias demo_timescale_up demo_timescale_5;alias demo_timescale_down demo_timescale_3";
alias "demo_timescale_3" "demo_timescale 3;alias demo_timescale_up demo_timescale_4;alias demo_timescale_down demo_timescale_2";
alias "demo_timescale_2" "demo_timescale 2;alias demo_timescale_up demo_timescale_3;alias demo_timescale_down demo_timescale_1.75";
alias "demo_timescale_1.75" "demo_timescale 1.75;alias demo_timescale_up demo_timescale_2;alias demo_timescale_down demo_timescale_1.5";
alias "demo_timescale_1.5" "demo_timescale 1.5;alias demo_timescale_up demo_timescale_1.75;alias demo_timescale_down demo_timescale_1.25";
alias "demo_timescale_1.25" "demo_timescale 1.25;alias demo_timescale_up demo_timescale_1.5;alias demo_timescale_down demo_timescale_1";
alias "demo_timescale_1" "demo_timescale 1;alias demo_timescale_up demo_timescale_1.25;alias demo_timescale_down demo_timescale_0.75";
alias "demo_timescale_0.75" "demo_timescale 0.75;alias demo_timescale_up demo_timescale_1;alias demo_timescale_down demo_timescale_0.5";
alias "demo_timescale_0.5" "demo_timescale 0.5;alias demo_timescale_up demo_timescale_0.75;alias demo_timescale_down demo_timescale_0.25";
alias "demo_timescale_0.25" "demo_timescale 0.25;alias demo_timescale_up demo_timescale_0.5;alias demo_timescale_down demo_timescale_0.125";
alias "demo_timescale_0.125" "demo_timescale 0.125;alias demo_timescale_up demo_timescale_0.25;alias demo_timescale_down demo_timescale_0.05";
alias "demo_timescale_0.05" "demo_timescale 0.05;alias demo_timescale_up demo_timescale_0.125;alias demo_timescale_down demo_timescale_0.01";
alias "demo_timescale_0.01" "demo_timescale 0.01;alias demo_timescale_up demo_timescale_0.05;alias demo_timescale_down demo_timescale_0.001";
alias "demo_timescale_0.001" "demo_timescale 0.001;alias demo_timescale_up demo_timescale_0.01;alias demo_timescale_down demo_timescale_0.001";

alias "demo_timescale_binds_toggle" "demo_timescale_binds_on";



echo;
echo;
echo;
echo;
