# Thesis_results






## Associating Scene effects to objects in dynamic scenes


#### Figure 1 
Dynamatte:
![scooter-black](imgs/dynamatte/scooter-black.gif)
Omnimatte:
![scooter-black](imgs/omnimatte/scooter-black.gif)
Comparison between Omnimatte and Dynamatte on a scene with dynamic traffic in the background. Omnimatte reconstructs this traffic in the foreground layer and Dynamatte reconstructs it in the background.

#### Figure 2
Dynamatte:
![amsterdamse_brug](imgs/dynamatte/amsterdamse_brug.gif)
Omnimatte:
![amsterdamse_brug](imgs/omnimatte/amsterdamse_brug.gif)
The reconstruction of a scene with two cyclists. On the left are dynamic background elements in the form of people doing a sports class, another cyclist and cars upon the bridge. Dynamatte partially reconstructs the dynamic scene elements in the background layer, whereas Omnimatte reconstructs all dynamic elements divided over the foreground object layers.
Omnimatte also reconstructs parts of the bike stands in the foreground layer due to errors in the homography estimation of the scene.

#### Figure 3
Dynamatte:
![kruispunt_rijks](imgs/dynamatte/kruispunt_rijks.gif)
Omnimatte:
![kruispunt_rijks](imgs/omnimatte/kruispunt_rijks.gif)
Busy intersection with large background elements, occlusions, overlapping shadows and correlated movement.

## Figure 4

![](imgs/homography_demos/homography_kruispunt_rijks.gif)  |  ![](imgs/homography_demos/noise_homography_kruispunt.gif)
:-------------------------:|:-------------------------:
Homography stabilization |  Homography-based sampling

The bad homography estimation of the video causes misalignment between the noise input and the scene.

#### Figure 5
Dynamatte:
![nescio_2](imgs/dynamatte/nescio_2.gif)
Omnimatte:
![nescio_2](imgs/omnimatte/nescio_2.gif)
The reconstruction of Omnimatte and Dynamatte on a noisy video.

## Figure 6
![](imgs/homography_demos/homography_nescio_2.gif)  |  ![](imgs/nescio_2_noise.gif)
:-------------------------:|:-------------------------:
Homography stabilization | After stabilization the video is still noisy

## Figure 7
#### Figure 7a
Dynamatte:
![ringdijk](imgs/dynamatte/ringdijk.gif)
Omnimatte:
![ringdijk](imgs/omnimatte/ringdijk.gif)

#### Figure 7b
Dynamatte:
![nescio_1](imgs/dynamatte/nescio_1.gif)
Omnimatte:
![nescio_1](imgs/omnimatte/nescio_1.gif)

#### Figure 7c
Dynamatte:
![drift-chicane](imgs/dynamatte/drift-chicane.gif)
Omnimatte:
![drift-chicane](imgs/omnimatte/drift-chicane.gif)

## Figure 8
![nescio_1](imgs/homography_demos/homography_nescio_1.gif) | ![nescio_1](imgs/homography_demos/noise_homography_nescio_1.gif)
:-------------------------:|:-------------------------:
Homography stabilization | The input and video are misaligned.

## Figure 9
Dynamatte:
![raam_kruisend](imgs/dynamatte/raam_kruisend.gif)
Omnimatte:
![raam_kruisend](imgs/omnimatte/raam_kruisend.gif)
Two foreground objects that occlude each other. Reflections of both foreground objects out-of-frame objects in the background

Dynamatte:
![hockey](imgs/dynamatte/hockey.gif)
Omnimatte:
![hockey](imgs/omnimatte/hockey.gif)
A street hockey player. The puck is correctly associated to the foreground layer by both Omnimatte and Dynamatte. There are some dynamic elements in the background.

Dynamatte:
![dance-jump](imgs/dynamatte/dance-jump.gif)
Omnimatte:
![dance-jump](imgs/omnimatte/dance-jump.gif)
A dancer that is partially occluded by reeds in the foreground. There are some moving people in the background.

Dynamatte:
![rollerblade](imgs/dynamatte/rollerblade.gif)
Omnimatte:
![rollerblade](imgs/omnimatte/rollerblade.gif)
A person on rollerblades jumping. This is a simple scene with no dynamic background elements and not a lot of noise or depth. Both Omnimatte and Dynamatte perform well.

Dynamatte:
![flamingo](imgs/dynamatte/flamingo.gif)
Omnimatte
![flamingo](imgs/omnimatte/flamingo.gif)
A flamingo in the water. Omnimatte removes the ripples and reflection in the water better that Dynamatte.

## Video Completion

#### Busy intersection with large background elements, occlusions, overlapping shadows and correlated movement
![kruispunt_rijks](imgs/video_completion/vc_kruispunt_rijks.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### Bridge with dynamic background elements
![amsterdamse_brug](imgs/video_completion/vc_amsterdamse_brug.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### Bike path with depth and dynamic background elements
![nescio_2](imgs/video_completion/vc_nescio_2.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### cyclist whose shadow overlaps with reeds
![ringdijk](imgs/video_completion/vc_ringdijk.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

### DAVIS video's
#### 'Hockey': some small dynamic elements in the background
![hockey](imgs/video_completion/vc_hockey.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### 'Dance-jump': Dynamic elements in the background and reed occluding the foreground object
![dance-jump](imgs/video_completion/vc_dance-jump.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### 'Rollerblade': Fully static scene
![rollerblade](imgs/video_completion/vc_rollerblade.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### 'drift-chicane': smoke caused by foreground object and a haze of smoke in the foreground
![drift-chicane](imgs/video_completion/vc_drift-chicane.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### 'Flamingo': Ripples in the water caused by foreground object
![flamingo](imgs/video_completion/vc_flamingo.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### 'Cows': The pole in the foreground causes the shadow of the cow to be reconstructed in background
![cows](imgs/video_completion/vc_cows.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### 'Scooter-black': large camera movement with traffic in the background
![scooter-black](imgs/video_completion/vc_scooter-black.gif)
Ground Truth	Dynamatte	Omnimatte	FGVC	Onion Peel

#### 'Car-roundabout': large camera movement with traffic in the background
![car-roundabout](imgs/video_completion/vc_car-roundabout.gif)

# Ablation Study
## Global Context Volume
### Figure X
With Global Context Volume
![With context](imgs/dynamatte/amsterdamse_brug.gif)

Without Global Context Volume
![With context](imgs/ablations/amsterdamse_brug_no_att.gif)

## Background Dynamics Regularization
### Figure X
With background dynamics regularization:
![With regularization](imgs/dynamatte/amsterdamse_brug.gif)

Without background dynamics regularization:
![Without regularization](imgs/ablations/no_reg.gif)

With only the difference term of the background dynamics regularization:
![With only correlation regularization](imgs/ablations/corr_reg.gif)

With only the correlation term of the background dynamics regularization:
![With only difference regularization](imgs/ablations/diff_reg.gif)

## Depth Reconstruction
### Figure X
With depth:
![Busy intersection with depth reconstruction](imgs/ablations/depth_kruispunt.gif)

Without depth:
![Busy intersection without depth reconstruction](imgs/dynamatte/kruispunt_rijks.gif)

### Figure X
With depth:
![Dike with depth reconstruction](imgs/ablations/depth_nescio.gif)

Without depth:
![Dike without depth reconstruction](imgs/dynamatte/nescio_2.gif)
