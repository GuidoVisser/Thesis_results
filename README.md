# Thesis_results

## Homography and Noise in the video's

![](imgs/homography_demos/homography_nescio_2.gif)  |  ![](imgs/homography_demos/homography_kruispunt_rijks.gif)
:-------------------------:|:-------------------------:
Noisy video             |  Busy intersection




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

#### Busy intersection with large background elements, occlusions, overlapping shadows and correlated movement
Dynamatte:
![kruispunt_rijks](imgs/dynamatte/kruispunt_rijks.gif)
Omnimatte:
![kruispunt_rijks](imgs/omnimatte/kruispunt_rijks.gif)

#### Bike path with depth and dynamic background elements
Dynamatte:
![nescio_2](imgs/dynamatte/nescio_2.gif)
Omnimatte:
![nescio_2](imgs/omnimatte/nescio_2.gif)

#### cyclist whose shadow overlaps with reeds
Dynamatte:
![ringdijk](imgs/dynamatte/ringdijk.gif)
Omnimatte:
![ringdijk](imgs/omnimatte/ringdijk.gif)

#### Two foreground objects that occlude each other. Reflections of both foreground objects out-of-frame objects in the background
Dynamatte:
![raam_kruisend](imgs/dynamatte/raam_kruisend.gif)
Omnimatte:
![raam_kruisend](imgs/omnimatte/raam_kruisend.gif)

#### DAVIS video's
#### 'Hockey': some small dynamic elements in the background
Dynamatte:
![hockey](imgs/dynamatte/hockey.gif)
Omnimatte:
![hockey](imgs/omnimatte/hockey.gif)


#### 'Dance-jump': Dynamic elements in the background and reed occluding the foreground object
Dynamatte:
![dance-jump](imgs/dynamatte/dance-jump.gif)
Omnimatte:
![dance-jump](imgs/omnimatte/dance-jump.gif)

#### 'Rollerblade': Fully static scene
Dynamatte:
![rollerblade](imgs/dynamatte/rollerblade.gif)
Omnimatte:
![rollerblade](imgs/omnimatte/rollerblade.gif)

### Foreground scene effects can get reconstructed in background

#### 'drift-chicane': smoke caused by foreground object and a haze of smoke in the foreground
Dynamatte:
![drift-chicane](imgs/dynamatte/drift-chicane.gif)
Omnimatte:
![drift-chicane](imgs/omnimatte/drift-chicane.gif)

#### 'Flamingo': Ripples in the water caused by foreground object
Dynamatte:
![flamingo](imgs/dynamatte/flamingo.gif)
Omnimatte
![flamingo](imgs/omnimatte/flamingo.gif)

### Failure case: Homography induced jitter in static background
![nescio_1](imgs/dynamatte/nescio_1.gif)

### Failure case: parallax with static foreground elements
#### 'Cows': The pole in the foreground causes the shadow of the cow to be reconstructed in background
Dynamatte:
![cows](imgs/dynamatte/cows.gif)

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
