# Thesis_results

## Homography and Noise in the video's

## Associating Scene effects to objects in dynamic scenes

![amsterdamse_brug](imgs/amsterdamse_brug.gif)
![nescio_2](imgs/nescio_2.gif)
![ringdijk](imgs/ringdijk.gif)
![kruispunt_rijks](imgs/kruispunt_rijks.gif)
![raam_kruisend](imgs/raam_kruisend.gif)
![hockey](imgs/hockey.gif)
![dance-jump](imgs/dance-jump.gif)
![rollerblade](imgs/rollerblade.gif)

### Foreground scene effects can get reconstructed in background
![drift-chicane](imgs/drift-chicane.gif)
![flamingo](imgs/flamingo.gif)


### Failure case: Homography induced jitter in static background
![nescio_1](imgs/nescio_1.gif)

### Failure case: parallax with static foreground elements
![cows](imgs/cows.gif)

### Failure case: Large camera movement
![scooter-black](imgs/scooter-black.gif)
![car-roundabout](imgs/car-roundabout.gif)



## Video Completion


# Ablation Study
## Global Context Volume
### Figure X
With Global Context Volume
![With context](imgs/amsterdamse_brug.gif)

Without Global Context Volume
![With context](imgs/amsterdamse_brug_no_att.gif)

## Background Dynamics Regularization
### Figure X
With background dynamics regularization:
![With regularization](imgs/amsterdamse_brug.gif)

Without background dynamics regularization:
![Without regularization](imgs/no_reg.gif)

With only the difference term of the background dynamics regularization:
![With only correlation regularization](imgs/corr_reg.gif)

With only the correlation term of the background dynamics regularization:
![With only difference regularization](imgs/diff_reg.gif)

## Depth Reconstruction
### Figure X
With depth:
![Busy intersection with depth reconstruction](imgs/depth_kruispunt.gif)

Without depth:
![Busy intersection without depth reconstruction](imgs/kruispunt_rijks.gif)

### Figure X
With depth:
![Dike with depth reconstruction](imgs/depth_nescio.gif)

Without depth:
![Dike without depth reconstruction](imgs/nescio_2.gif)
