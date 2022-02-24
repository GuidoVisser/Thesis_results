# Thesis_results

## Homography and Noise in the video's

## Associating Scene effects to objects in dynamic scenes

#### Busy intersection with large background elements, occlusions, overlapping shadows and correlated movement
Dynamatte:
![kruispunt_rijks](imgs/dynamatte/kruispunt_rijks.gif)![kruispunt_rijks](imgs/omnimatte/kruispunt_rijks.gif)
Omnimatte:
![kruispunt_rijks](imgs/omnimatte/kruispunt_rijks.gif)

#### Bridge with dynamic background elements
Dynamatte:
![amsterdamse_brug](imgs/dynamatte/amsterdamse_brug.gif)
Omnimatte:
![amsterdamse_brug](imgs/omnimatte/amsterdamse_brug.gif)

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

### Failure case: Large camera movement
![scooter-black](imgs/dynamatte/scooter-black.gif)
![car-roundabout](imgs/dynamatte/car-roundabout.gif)



## Video Completion


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
![With regularization](imgs/dynamtte/amsterdamse_brug.gif)

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
