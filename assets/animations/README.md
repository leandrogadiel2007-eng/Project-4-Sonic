# KinemIQ CC0 animation bank

Source: https://github.com/Kinemiq/free-game-animations

Download KinemIQ_Free_Animations_CC0_GLB.zip from the upstream Releases page when available. Extract into this directory. The upstream README describes 35 clips on a 66-bone humanoid skeleton, CC0 1.0, derived from Quaternius Universal Animation Library.

The current game uses procedural meshes, not skinned models. Its AnimationMixer controllers use locally authored placeholder clips. Retarget imported GLB clips in Blender to the final Sonic and Metal Sonic skeletons, export each character with animations, then replace the placeholder controllers using GLTFLoader and AnimationMixer on the skinned scene.

State mapping: idle → idle; run → run; dodge → roll; counter → jab/cross/hook; hit → hit reaction; defeat → death. Hover, homing, spin, boost and shield need custom adaptations. No external binary assets are included yet.
