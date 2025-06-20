

# Gaussian Splat Particle System in TouchDesigner 

Created by Lake Heckaman
As seen in: 
- https://www.lakeheckaman.com/work/pollination
- https://www.lakeheckaman.com/work/still-life
- https://www.instagram.com/reel/DDuoEsZtFnA

## Features 
- WORKS ON MAC
- Apply turbulence to splats to dissolve the scene
- Send each splat back to 'home location' from anywhere 
- Render splat as point cloud or particle system 
- Fade between point cloud and particle system via: 
    - Turbulence
    - Distance to point 
    - Effector Array (CHOPs)
    - Uniformly
    - Distance between splat and 'home location'
- Optionally draw splat depth in separate buffer 
- Optionally draw splat velocity in separate buffer 
- Bounding Volumes (box, sphere)
- Toggle sorting for optimization 
- Optional render upscaling 

#### Coming 
- Color correction 
- Nearest Neighbor Calculation
- Relighting 

## Usage 
1. Get the tox from my patreon at https://www.patreon.com/water__shed
2. Drag and drop the .tox into your project file
3. Update the splat .ply file path parameter to your splat file
4. Reset the component with the Reset parameter or your preferred hot key

- See video tutorial here: https://youtu.be/wPw0OLlZ4sE
- setting Array and Distance from Center mode to `dissolve` will freeze all splats at the start, only allowing them to move after they are affected by the distance or array of effectors (turb should be nonzero to see this)
- setting Array and Distance to `splat` or `point` will apply turbulence globally, so the whole splat will start to move if `turbAmp>0`
- There is a parameter for 'mix to splat at home', which wil determine if all splats are rendered at full size when close to their initial position

### Tips
- this pipeline can get pretty heavy at high resolutions, and at any resolution the splat files take up a decent bit of GPU memory, so be careful and save often
- alt + hover over params to see help, where it exists 
- make sure you have a splat .ply file, not all .ply files are splats (export as gaussian splat from luma, for example)
- use SuperSplat to edit splats and then export again to re-import to TD 


### Examples
Example splat model (created by myself) can be downloaded from https://www.dropbox.com/scl/fi/nv952xgspe4me2g20opdk/gs_wood_sculpture_outside_av.ply?rlkey=unwqpqgh9wf5pnoc399up74nj&dl=0

## LICENSE 
This project is licensed under a Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License (CC BY-NC-ND 4.0).

You may:
- View and use this software for personal and non-commercial purposes
- Share the original, unmodified software while giving appropriate credit

You may not:
- Use this software for commercial purposes
- Modify or create derivative works
- Redistribute modified versions

To use this for commercial purposes please contact me at hello@lakeheckaman.com

For full license details, see: https://creativecommons.org/licenses/by-nc-nd/4.0/
