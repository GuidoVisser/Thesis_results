# Thesis_results

## Homography and Noise in the video's

## Associating Scene effects to objects in dynamic scenes

![amsterdamse_brug](imgs/dynamatte/amsterdamse_brug.gif)
![nescio_2](imgs/dynamatte/nescio_2.gif)
![ringdijk](imgs/dynamatte/ringdijk.gif)
![kruispunt_rijks](imgs/dynamatte/kruispunt_rijks.gif)
![raam_kruisend](imgs/dynamatte/aam_kruisend.gif)
![hockey](imgs/dynamatte/hockey.gif)
![dance-jump](imgs/dynamatte/dance-jump.gif)
![rollerblade](imgs/dynamatte/rollerblade.gif)

### Foreground scene effects can get reconstructed in background
![drift-chicane](imgs/dynamatte/drift-chicane.gif)
![flamingo](imgs/dynamatte/flamingo.gif)


### Failure case: Homography induced jitter in static background
![nescio_1](imgs/dynamatte/nescio_1.gif)

### Failure case: parallax with static foreground elements
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
