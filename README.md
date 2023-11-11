**암호 손동작 설정(set_motion.py, RunSetMotion.java)**
<p align="center">
  <img src="https://github.com/seungtoctoc/HandMotionPassword/assets/102455571/db67d573-1f5a-4ba3-bd8b-e2c3142c9687">
</p>

- 웹캠으로부터 손동작 정보 수집
- 파라미터로 받은 docName과 action을 이용해 파일 저장
- RunSetMotion.java : 스프링 환경에서 set_motion.py 실행<br><br>

**손동작 학습(train_motion.py, train.ipynb, RunTrainMotion.java)**
- 암호 해제 성공 여부 판단을 위한 모델 학습
- LSTM모델과 Dense레이어를 사용해 파일로 저장했던 3가지 손동작들 학습
- train.ipynb : 학습 완료 그래프 포함
- RunTrainMotion.java : 스프링 환경에서 train_motion.py 실행<br><br>

**암호 손동작 해제 판단(test_motion.py, RunTestMotion.java)**
- 웹캠으로부터 손동작 정보 수집
- 학습한 손동작들 중 하나인지 유사도 판단 (true 혹은 false 반환)
- RunTestMotion.java : 스프링 환경에서 test_motion.py 실행<br><br>
