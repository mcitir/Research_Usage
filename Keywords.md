## Research Fields via Keyworkds

- Motion Primatives (MP)

### Scenarios
- Automated Overtaking

### Techniques 
- Mixed reality (MR) Simulation


#### Perception

##### Lidar

###### Classical Approach

Preprocessing:

Range-Based Filtering
![image](https://user-images.githubusercontent.com/35730346/138560476-66da28c3-9913-4dc2-a6f7-83923e42e2cd.png)

Angle-Based Filtering
![image](https://user-images.githubusercontent.com/35730346/138560461-f5710881-be98-44ca-960c-660f07e6d65c.png)

Downsampling: Distill point cloud into a representative set of points
![image](https://user-images.githubusercontent.com/35730346/138560526-58bce45d-10af-48d2-a1d8-5f4f31962ccf.png)

Fusing Point Clouds
![image](https://user-images.githubusercontent.com/35730346/138560547-26f1f54d-95f3-4bd1-badc-a150b4e54b17.png)

Ground Filtering Approaches:
 - Curvature/Normals -> Moosman et al (expensive, slow)
 - Fit a big fat plane to the scene -> RANSAC (fast, nondeterministic, maybe not the best e.i road drainage)
 - Rays*/Columns in depth image -> Petroskaya & Thrun/Bogoslavskyi, Tier4, Cho et al (Super Fast, possible accuracy issues, relies on high vertical resolution)
 - Factor Graphs
 - Voxels based methods etc.
 - (***Note:** Autoware.auto uses ray-based ground filtering because it is fast and deterministic)

Clustering/Segmentation Algorithms:
 - Euclidean Clustering

###### Deep Learning Approach
#### Localization
[Coordinate Frames of Self Driving Car](https://ros.org/reps/rep-0105.html)
### Methods
#### Artifical Intelligence
- Hierarchical Reinforcement Learning
- Semi-Markov decision process (SMDP)
