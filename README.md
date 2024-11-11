#  주제 : 자율주행/ADAS - Path Planning & Control

<table width=80%>
  <tr><td><b>프로젝트 기간</b></td><td><b>프로젝트원</b></td><td><b>수행 역할</b></td>
  </tr>
  <tr><td>2024.10.15 - 2024.10.30</td><td>김도훈, 김성진, 김진우, 전민홍, 전지환, 조섭근, 조영욱</td><td>Global Path Planning, Mission/Mode Control, Optimal Trajectory Planning</td>
  </tr>
</table>
<br/>

## 프로젝트 소개
Detection Data와 Localization 정보를 기반으로 Planning과 Control을 하여 주어진 시뮬레이션 환경에서 4가지 미션을 수행하는 프로젝트<br><br>
<img src="https://github.com/user-attachments/assets/db77e071-a570-49e5-aec3-dc25d3a6dd1e" width="50%" height="50%"> <br><br>

## SW Architecture
<img src="https://github.com/user-attachments/assets/d59c6265-b80b-4905-93d9-b4a2863b9e30" width="79%" height="79%"><br><br>

MATLAB, Simulink<br>
<img src="https://github.com/user-attachments/assets/79e8b57b-ceee-4dc7-a2c6-ecab1ebd8f14" width="80%" height="80%">



## 1️⃣ Global Path Planning
Global Path Planning을 위한 경로 탐색 알고리즘 비교 후 A star 알고리즘 적용<br><br>
<img src="https://github.com/user-attachments/assets/fb25a0ac-b8d4-413f-bd17-0048b65ffc73" width="40%" height="40%">

## 2️⃣ Driving
<table>
  <tr>
    <td width=45%>
    [Local Path Planning]<br>
    1. Catesian to Frenet Frame<br>
    2. Make Path List<br> 
    3. Make Obstacle List<br>
    4. Decision Path<br>
    5. Frenet to Catesian Frame<br>
    6. Catesian to GlobalFrame<br><br>
    <br>[Driving Control]<br>
    1. PD Speed Control<br>
    2. Pure Pursuit Steering Control<br></td>
    <td>
    <img src="https://github.com/user-attachments/assets/dbe79140-e5d9-492e-b744-44bad299327b" width="95%" height="95%" align="center">
    </td>
  </tr>

  <tr>
    <td width=45%>
      [Collision Check]<br>
      1. Euclidean Distance-Based Check <br>
      2. Separating Axis Theorem (SAT) <br>
    </td>
    <td>
    <img src="https://github.com/user-attachments/assets/fcb19292-3abd-41d6-980b-72ba20774f39" width="80%" height="80%" align="center">
    </td>
  </tr>
</table>

## 3️⃣ Parking
<img src="https://github.com/user-attachments/assets/90c29945-feaf-4cf2-99a7-958797673dd1" width="40%" height="40%">


## 시연영상
https://youtu.be/TwMqGNApJog
