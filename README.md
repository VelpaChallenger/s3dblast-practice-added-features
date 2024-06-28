# s3dblast-practice-added-features

Fork from Chrezm's version. I am adding the following features:

- You can use all of the features below *at any time*. No matter if you are receiving damage, in a 'cutscene '(like the running/loop sequence at the beginning of Green Grove 1), grabbing a ring, etc., you can still restart, change the HUD mode, go to the Level Select screen, etc. This is specially helpful for levels where you can get hit very easily while practicing (for example, Gene Gadget Act 1).
- When you start the game, you are immediately taken to the Level Select screen. This way, you don't even have to skip the initial cutscenes and then pause the game and press B to go to the Level Select screen. You are taken immediately.

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
2. Start+B opens level select
3. Clearing a stage puts you back at the beginning of the stage after the score tally.
4. Start+C changes between one of three HUD display modes
* Mode 1 replaces the lives display with the stage's frame counter, and the number of rings display with the stage frame counter expressed in MSS format.
* Mode 2 replaces the lives display with the stage's frame counter, but the number of rings display still shows the number of rings.
* Mode 3 replaces the lives display with the stage's frame counter in MSS format, but the number of rings display still shows the number of rings.
5. Regardless of what the lives display says, you have infinite lives.
6. Regardless of what the number of rings display says, you still have whatever many rings you collected normally (and can still die if you get hit with 0 rings).
7. The "RINGS" text is replaced with some semitransparent tiles (to indicate the viewer it is no longer a rings display), except when you cling to a big ring checkpoint. At that point, it then
* Replaces the "RINGS" text with the amount of time it took you to make it from the previous checkpoint to the current one for three seconds (if you had previously clinged to another checkpoint earlier in the stage), and then
* Replaces the "RINGS" text with the amount of time it took you to make it from the start of the stage to the current checkpoint for three seconds, and then
* Goes back to the semitransparent tiles.
8. Whatever is currently being drawn instead of the "RINGS" text, it will flash if you have no rings. This is intentional, as it helps runners who may want to do a damage boost strat know if they have any rings.
