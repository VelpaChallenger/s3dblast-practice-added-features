# s3dblast-practice
IPS Patcher for the Sonic 3D Blast Practice ROM for the Sonic Speedrunning Community, as well as associated json file.

## Instructions 
### Via IPS Patcher.
1. Download the Lunar IPS Patcher.
2. Follow the instructions on https://fantasyanime.com/patching under How To Patch with Lunar IPS. You will need your own Sonic 3D Blast rom, it does not need to be unheaded.

Note: This will apply the patch to the ROM file you give. Make sure to keep a backup of your original rom file. 

### Via JSON
1. Visit https://beninswe.github.io/ROMPatcher/?patch=https://raw.githubusercontent.com/Chrezm/s3dblast-practice/main/Sonic%203D%20Blast%20(W)%20%5B!%5D%20Practice.json
2. Click "Browse" next to "ROM", and open your own copy of an unmodified Sonic 3D Blast ROM.
3. Click "Patch!".
4. A new link will appear. Click it download your patched ROM.

Note: This method does not require you download any files from this repository.

## Features
1. Start+A restarts the stage from the beginning, ignoring any checkpoints you have attained.
2. Start+(B+A) opens level select
3. Clearing a stage puts you back at the beginning of the stage after the score tally.
4. The lives display is replaced by the stage's frame counter. You have infinite lives.
5. The rings display is replaced by the stage's frame counter expressed in mss format. You still have whatever many rings you collected normally (and can still die if you get hit with 0 rings).
6. The "RINGS" text is replaced with some semitransparent tiles (to indicate the viewer it is no longer a rings display), except when you cling to a big ring checkpoint. At that point, it then
* Replaces the "RINGS" text with the amount of time it took you to make it from the previous checkpoint to the current one for three seconds (if you had previously clinged to another checkpoint earlier in the stage), and then
* Replaces the "RINGS" text with the amount of time it took you to make it from the start of the stage to the current checkpoint for three seconds, and then
* Goes back to the semitransparent tiles.
7. Whatever is currently being drawn instead of the "RINGS" text, it will flash if you have no rings. This is intentional, as it helps runners who may want to do a damage boost strat know if they have any rings.
