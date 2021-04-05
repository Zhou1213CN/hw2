## Project 2

#### Zheng Zhou, Zehua Zhang

The implementations are in our code.

#### F0 Comparison

| Algo                                      | Time Elapsed | Estimation |
| ----------------------------------------- | ------------ | ---------- |
| ExactF0                                   | 656s         | 7406649    |
| BJKST Sketch (Width: 600 Depth:5) Locally | 59s          | 7348413    |
| BJKST Sketch (Width: 600 Depth:5) GCP     | 48s          | 7491803    |

Collaborated with Jessica's group, we determine the smallest width that satisfies at least 95% probability of success of getting a estimated F0 between +/- 20% of exact F0 to be 500. (The code is comment out)

Our BJKST runs faster than ExactF0 and achieves a good estimation of F0

#### F2 Comparison

| Algo                                   | Time Elapsed | Estimation   |
| -------------------------------------- | ------------ | ------------ |
| ExactF2 Local                          | 231s         | 8567966130   |
| ExactF2 GCP                            | 72s          | 8567966130   |
| Tug-of-War Local (Width :10. Depth: 3) | 156s         | 7722146282.8 |
| Tug-of-War GCP(Width :10. Depth: 3)    | 78s          | 9089863981.2 |

For ToW F2 estimate, we are getting a estimation that is so far the closest estimate to exact F0. It is also within 0.1689 Standard deviation from the true F2. So it will be a good estimator.

The local running time for ToW is a little bit faster than running ExactF2 locally.

