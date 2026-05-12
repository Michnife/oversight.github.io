# BTP - Over Sight

## **1. Project context**

Over Sight is an experimental indoor reconnaissance system based on a compact drone designed to be manually deployed but partially autonomous.

The drone is physically launched by an operator into an enclosed indoor space (room, corridor, confined area). Once deployed, the system enters an autonomous stabilization phase, during which the drone maintains a stable position in the air without continuous human control.

The drone is not fully autonomous in navigation at this stage. Its purpose during the beta phase is not exploration, but short-duration observation and analysis from a stabilized position.

Once stabilized, the drone captures a 360° visual view of the environment using an onboard panoramic camera. This visual data is then processed directly on the embedded computing unit (Raspberry Pi) using computer vision and embedded AI models.

---

## **2. User role**

The following roles will be involved in beta testing.

Les rôles suivants seront impliqués dans les tests bêta.

| **Role Name** | **Description** |
| --- | --- |
| Operator / Opérateur | The operator is responsible for physically deploying the drone (launch), monitoring the video and AI feedback, and making decisions based on the information provided. The operator does **not** manually pilot the drone during the beta phase. |

---

## **3. Feature table**

The following features will be shown during the defense.

Les caractéristiques suivantes seront présentées lors de la défense.

| Feature ID | User role | Feature name | Detailed description |
| --- | --- | --- | --- |
| F1 | Operator | Site pairing | The operator can pair the drone with the site when launching the script to automatically link the drone to the platform. |
| F2 | Operator | Login | The operator can log in to the site using credentials. |
| F3 | Operator | Select drone | The operator can select a specific drone among multiple available drones. |
| F4 | Operator | Drone deployment | The operator can power on the drone and deploy it. |
| F5 | Everyone | Software startup | The drone automatically starts the AI software. |
| F6 | Everyone | Drone flight | The drone can maintain controlled flight for a short duration in an indoor environment. |
| F7 | Operator | Live video feedback | The operator has access to the drone’s real-time video stream via the site interface. |
| F8 | Everyone | Human presence detection | The embedded AI detects human silhouettes in the camera feed and differentiates them from non-human objects using a trained model (YOLO-based). |
| F9 | Everyone | Environment perception (LiDAR) | The drone uses LiDAR data to estimate distances and the spatial structure of the room, supporting basic environment understanding. |
| F10 | Everyone | Captured images | The drone can capture images of different faces and objects. |
| F11 | Operator | Previous flights | The operator has access to stored videos from previous drone flights. |
| F12 | Operator | Drone movements | The operator can move the drone via the interface. |
| F13 | Everyone | Showcase site | The site is clear and showcases all the work completed for the project. |

---

## **4. Success Criteria**

Define the metrics and conditions that determine if the beta version is successful.

Définir les indicateurs et les conditions permettant de déterminer si la version bêta est un succès.

| Feature ID | Key success criteria | Indicator / metric | Result |
| --- | --- | --- | --- |
| F1 | The drone is correctly paired with the site. | The drone appears on the site with a unique ID within 10 seconds after pairing. |  |
| F2 | An operator can log in using the moderator account. | 20 consecutive login attempts with 0 application-related failures. |  |
| F3 | All available drones are visible and selectable on the site. | All connected drones are listed and can be selected without error during 10 consecutive selection attempts. |  |
| F4 | The drone can be powered on successfully. | The drone powers on and reaches an operational state in less than 10 seconds. |  |
| F5 | The software starts automatically upon drone deployment. | The AI software launches automatically within 5 seconds after drone startup, without manual intervention. |  |
| F6 | The drone can fly autonomously and position itself at 180 cm above the ground. | The drone maintains a stable position at 180 ± 20 cm for more than 3 seconds. |  |
| F7 | The video stream is live on an external screen. | Live video stream with latency < 500 ms and frame rate ≥ 15 FPS. |  |
| F8 | Human presence is correctly detected. | Detection accuracy ≥ 80% in controlled indoor conditions. |  |
| F9 | The drone can map the room or environment where it is located. | Walls and room boundaries are detected with position error ≤ 20 cm in a controlled test environment. |  |
| F10 | The drone captures images of faces and objects and stores them on the site. | No duplicate face entries; object classification accuracy ≥ 80%. |  |
| F11 | Videos from previous flights are stored and accessible. | Recorded videos are accessible on the site with playback ≥ 15 FPS and no critical data loss. |  |
| F12 | The drone responds to movement commands issued via the interface. | The drone moves from point A to point B using only interface commands, with correct execution in 90% of attempts. |  |
| F13 | The site is accessible to all users and presents project information clearly. | Site availability ≥ 99% during beta testing and all main sections accessible without errors. |  |