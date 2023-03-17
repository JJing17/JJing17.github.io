# Zenen Diode
## preview

### 역방향 절연파괴  
 Reverse bias에서 miner carrier에 의한 일정한 전류가 흐른다.($\cong$ 0에 수렴)  
 그러나 소재에 가한 역전압이 증가하면, 결과적으로 brackdown이 일어나고, 급격하게 큰 전류가 발생하게 된다. 크게는 `Zener effect`과 `Avalanche Effect` 이 있다.  
<img width="615" alt="ㅇㅇ" src="https://user-images.githubusercontent.com/98220775/225536504-3b41fe0e-1e96-4b16-ad23-23754c87e529.png">

#### Zener effect
<img width="646" alt="ㅇ" src="https://user-images.githubusercontent.com/98220775/225536502-8af872aa-e546-4732-bb43-a231864ee3d3.png">

 pn접합에서 공핍영역에서는 전자나 hole을 잃은 원자들이 있어, diffenetion current에 의해 약하게 연결된 carrier들을 제공한다. 이 영역에서 강한 전자장은 공유결합에서 남아있는 전자들 분리하는 충분한 에너지를 제공한다.  
 일단 자유로워지면 전자는 전자장에 의해 가속되어 접합의 n영역으로 이동한다. 이 효과는 약 $10^6V/m$의 전자장의 크기를 발생한다. 적절한 전압은 높은 전자장을 발생시키기 위해 좁은 공핍 연결이 필요하다.![brakedown_graph](https://user-images.githubusercontent.com/98220775/225528890-4be1e808-9fed-4d16-975e-b12e185dbafb.png)

 Reverse Bias에서 공핍영역은 Capacitor와 비슷하다고 볼 수 있기 때문에 Capacitor의 식을 이용하면  
 $$
 C_jo={\sqrt {\epsilon q N_a N_d \over 2V_0 \times (N_A+N_B)}}
 $$
 라는 식을 도출 할 수 있고 식에 따르면 접합의 양쪽에서 높은 농도로 도핑이 형성되어 있음을 알 수 있다 ($C_j0$가 커질수록 공핍 영역을 쉽게 뛰어넘을수 있음으로) `Zener effect`라고 불리는 이러한 형태의 항복은 3V~8V의 Reverse bias voltage에서 발생한다. 하지만 전압이 너무 과하게 흐르면 위 그래프처럼 `Avalanche ffect`에 의해 diode가 파괴될 수 있다.
 ##### reference : Microelectronics_2nd_edition_Behzad Razavi_p42 
 ##### image reference : https://electric-lab.tistory.com/425 
### Zener Diode work as Voltage Regulation
  Zener diode의 대표적인 역할은 voltage regulation이다. 아래의 그림으로 보면 Zener diode가 reverse biasing이 되어 있는데 이로 인해 일종의 저항으로 표현이 가능하다.
 
 <img width="831" alt="zener circuit" src="https://user-images.githubusercontent.com/98220775/225535414-936dbf3d-369b-451a-a288-f5f026f9e834.png">
 ##### reference : Microelectronics_2nd_edition_Behzad Razavi_p86 
