## Low Compute - High FPS BGS Algorithm

**Description:** Current BGS algorithms tend to work at slow FPS with different background update methodologies. This can be a problem for low-edge devices to compute the updates on high resolution images or when the FPS requirement is high on the edge system for sensitive applications. To make the algorithm work at high FPS along with the object detectors and classification networks running on the same device, I developed an algorithm and named is ***Grid Temporal Median*** which ran at 62 FPS on edge devices with one instance and 16FPS with five instances. The results of the algorithm showed below are profiled on *Intel(R) Celeron CPU N3350 @ 1.10GHz.*



| Width/Height | 1 instance(ms) | 3 instances(ms) | 4 instances(ms) | 5 instances(ms) |
| ------------ | -------------- | --------------- | --------------- | --------------- |
| 320          | 16.99          | 37.38           | 43.87           | 59.14           |
| 608          | 33.91          | 82.12           | 110.75          | 138.70          |

