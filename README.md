# Metro-Exodus-Gold-Edition-Max-Settings-Config
A config file I created using the gold edition of Metro Exodus that fixes alot of performance issues without decreasing any graphical options using dX11 API.


- Improved FPS
- Ultra settings with all settings maxed or enabled are capable on very low hardware @ 1080p (excluding hairworks)
- When looking at certain scenes - the train in volga - The FPS drops have been decreased and should be alot more bearable
- tweaked HDR and lighting to be more realistic and blur to be less annoying
- Made to be used in conjunction with The Ultra Realism Cine FX reshade preset created by Kycok_Xleba (http://sfx.thelazy.net/games/preset/11012/) after enabling the preset, I also enable Fidelity FX, you dont need to do this but it costs very little in resources.

Notes and other improvements that can be made:
- Disable fullscreen optimisations under compatibility mode
- Do Not run in ANY compatibility mode, it kills FPS... I used it as a fix for the dx12 bug where I couldnt get past the first screen. after this, it isnt needed, so turn it back off after the game starts up correctly
- I dont use any vsync, freesync or anything else, not even a frame limiter, but on higher end hardware feel free to limit fps, just know it isnt on by default

AMD Driver options under the game profile:
- Tesselation = AMD Optimized
- Freesync = Off
- Texture Quality = High
- everything else is disabled or left up to the game

- Also, open Task Manager and end the Radeon Host Application process, it uses CPU and has caused stuttering for me in the past



Testing Hardware:
AMD A10 6930P 2.6 ghz quad core APU w/ R5 iGpu and RX460 4GB GDDR5 dGPU, 500GB SATA drive and 2x8gb 2400mhz dual channel ram running Windows 10 21H1


Minimum Requirements:
Anything better than the above... I'll put my neck out and say that a Ryzen 5 3400G w/ Vega 11 iGPU could play Metro Exodus comfortably at 1080p using this config. Mainly because a vega 11 has twice the Time Spy score than the hardware mentioned above.


If your computer cant play the default settings, either go down to high settings or disable 'curves' in the reshade menu and this should give a decent FPS boost



INSTALL

Copy into your Metro Exodus file Directory where user.cfg is located. 

NOTE: if using any other edition, DO NOT just copy over the file. The enhanced edition will be different and have different features which you will lose when you do this. I've listed the changed lines below. Its safer if you manually make the changes to your config, here are the changes I made...

ggp_display_timing_pacing 0

ph_dbg_render_range 100. (make sure physx is enabled)

r_af_level 1

r_api 2

r_aspect_ratio_mode 0

r_blur_level 1

r_dx11_tess 1

r_enum_ssaa 14

r_exposure_control 0.

r_exposure_hdr 1.5

r_foliage_shadows 1

r_fullscreen on

r_fur 0

r_game_mblur_scale 0.75

r_hdr_max_luminance 900.

r_hdr_white_paper 150.

r_old_ambient_envlit 0.

r_quality_level 3

r_res_hor 1920

r_res_vert 1080

r_shading_rate 1.

r_shading_rate_dlisp 1.

r_taa_enabled 1

r_terr_displace_density 0

r_terr_displace_enable 0

r_vsync 0


Enjoy
