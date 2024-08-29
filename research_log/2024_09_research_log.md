#### 2024-08-28
- Holistic Control에 대해서 공부 시작
- DDPG or TD3 네크워크를 사용해 학습 진행
    - 성능이 좋고, 최신 알고리즘이라 간단하게 설정
    - 아직 RL에 대해서 잘 모르므로, 이것에 대해서 공부를 시작하기 위해 간략하게 설정

#### 2024-08-29
- IRIS 연구주제 선정됨
- 연구주제와 연구과정에 대해서 확실하게 설정하고 진행하기 위해서 생각하는 과정
- 연구과정을 통해 이루고자하는 목표는 결국 ***<span style="color:black">Manipulator Arm의 end effector가 발사체를 잡아서 원래 위치로 되돌아오는 것</span>***
    - **Holistic Control을 사용하는 이유** : 발사되는 발사체의 속도가 Manipulator Arm의 Maximum Angular Velocity보다 빠르게 설정해 Manipulator Arm의 Rotation만으로는 Object Tracking이 불가능하도록 속도를 설정할 예정.
    - 따라서 이 문제를 해결하기 위해서는 mobile base와 manipulator arm이 서로 협력하면서 움직여야 하므로 Holistic Control이 필수적
    - 그리고