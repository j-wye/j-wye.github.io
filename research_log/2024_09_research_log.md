#### 2024-08-28
- Holistic Control에 대해서 공부 시작
- DDPG or TD3 네크워크를 사용해 학습 진행
    - 성능이 좋고, 최신 알고리즘이라 간단하게 설정
    - 아직 RL에 대해서 잘 모르므로, 이것에 대해서 공부를 시작하기 위해 간략하게 설정

#### 2024-08-29
- *IRIS 연구주제 선정됨*
- 연구주제와 연구과정에 대해서 확실하게 설정하고 진행하기 위해서 생각하는 과정
- 연구과정을 통해 이루고자하는 목표는 결국 ***<U>Manipulator Arm의 end effector가 발사체를 잡아서 원래 위치로 되돌아오는 것</U>***
    - **<span style="color:red">Holistic Control</span>** 을 사용하는 이유 : 발사되는 발사체의 속도가 Manipulator Arm의 Maximum Angular Velocity보다 빠르게 설정해 Manipulator Arm의 Rotation만으로는 Object Tracking이 불가능하도록 속도를 설정할 예정.
    - 따라서 이 문제를 해결하기 위해서는 mobile base와 manipulator arm이 서로 협력하면서 움직여야 하므로 Holistic Control이 필수적
    - Holistic Control based Object Tracking이 성공적으로 진행되고 다음 단계는 발사체를 manipulator arm을 사용해 pick and place task를 수행하기 위해서 발사체를 향해 움직임
    - 발사체를 방 밖으로(시야에서 사라지도록) 향하도록 발사할 것, 이를 통해 시야에서 tracking하던 object를 사라지도록 함
    - 사라진 object의 expected trajectory를 Prediction하는 **<span style="color:red">Trajectory Prediction</span>** 을 진행
    - 실시간으로 들어오는 Environment Inforamtion를 사용해 expected trajectory를 지속적으로 수정하면서 발사체의 expected position을 결정하고 해당 위치로 이동하도록 **<span style="red">Nav2</span>** 를 사용해 path planning을 진행하며 최적 경로를 생성하며 움직이도록 함
- 연구주제의 Key는 **Holistic Control & Trajectory Prediction의 통합**
- 논문 제목으로는 다음과 같이 후보 2개를 선정
    - **<span style="color:violet">Robust Holistic Control-Based Trajectory Prediction in Mobile Manipulation System</span>**
    - **<span style="color:violet">Integrating Trajectory Prediction with Holistic Control in Mobile Manipulation System</span>**