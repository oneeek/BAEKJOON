## Simultaneous Optimization of Traffic Signal Control and Vehicle Platooning Scheme Based on Connected and Automated Vehicle (CAV) Technology

```python
#클래스를 사용한 교차로 제어 코드를 간략하게 보여줄 수 있도록 수정한 코드입니다.
class IntersectionControl:
    def __init__(self, inter_ID, phase_ID):
        self.inter_ID = inter_ID #교차로 ID
        self.phase_ID = phase_ID #신호현시 ID List
        self.red_sec = 3 #빨간불 지속시간
        self.SUMO_CMD = #시뮬레이션 작동을 위한 변수

    #신호 설정
    def set_signal(self, phase_ID, phase_sec):
        traci.trafficlight.setPhase(self.inter_ID, phase_ID)
        traci.trafficlight.setPhaseDuration(self.inter_ID, phase_sec)

    #신호 적용
    def start_signal(self, phase_ID, phase_sec):
        self.set_signal(phase_ID, phase_sec)
        for i in range(phase_sec + self.red_sec):
            traci.simulationStep()

    #시뮬레이션 작동
    def start_sim(self, phase_sec):
        traci.start(self.SUMO_CMD)
        for s in range(len(self.phase_ID)):
            self.start_signal(self.phase_ID[s], phase_sec[s])
        traci.close()

```
