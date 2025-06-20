

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
Get the tox from my patreon at https://www.patreon.com/water__shed

### Tips
- alt + hover over params to see help, where it exists 
- CHOP array expects channels as follows: [tx,ty,tz,radius]


### Examples
Example splat model can be downloaded from https://www.dropbox.com/scl/fi/nv952xgspe4me2g20opdk/gs_wood_sculpture_outside_av.ply?rlkey=unwqpqgh9wf5pnoc399up74nj&dl=0


See video at ___


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
