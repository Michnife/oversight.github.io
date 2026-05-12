# Benchmark Over Sight

- Run ID: `20260305_235536`
- Date: `2026-03-05 23:57:18`
- OS: `Linux-6.11.9-100.fc39.x86_64-x86_64-with-glibc2.38`
- Python: `3.12.7`

> Note CPU: `psutil` peut afficher >100% car c'est la somme sur plusieurs cœurs.

## Résultats

| IA | FPS avg | FPS min | FPS max | CPU avg (%) | RAM avg (MB) | Log |
|----|--------:|--------:|--------:|------------:|-------------:|-----|
| Face Tracking | 19.78 | 3.01 | 23.83 | 862.28 | 87.21 | `face_tracking.log` |
| Face Recognition | 21.93 | 3.27 | 115.41 | 165.67 | 479.29 | `face_recognition.log` |
| YOLO Objects | 28.04 | 2.60 | 57.31 | 575.32 | 569.02 | `yolo_objects.log` |
| YOLO Pose | 28.69 | 2.63 | 50.09 | 588.52 | 560.95 | `yolo_pose.log` |
| Shape + Face | 12.93 | 2.60 | 41.48 | 276.03 | 929.80 | `shape_face.log` |
| Combined Recognition | 5.20 | 2.09 | 29340.14 | 361.89 | 1174.13 | `combined_recognition.log` |
| Hand Recognition | 216.11 | 2.55 | 22738.64 | 172.46 | 746.68 | `hand_recognition.log` |

## Charts

![FPS avg](plots/fps_avg.png)

![CPU avg](plots/cpu_avg.png)

![RAM avg](plots/ram_avg.png)
