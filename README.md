# 파닉스 교육 게임
일반적인 게임은 아니지만, 처음으로 혼자 온전한 프로젝트를 완성한 교육 게임

# 기본적인 구조
![image](https://github.com/DWBoo/PhonicsGame/assets/147593910/3bcec62e-6b6e-45e2-a452-1dc0c9e5d049)</br>
최상위 오브젝트 하나에 모든 페이지가 포함되어 있으며, 하나의 프리팹으로 저장 후 사용
![image](https://github.com/DWBoo/PhonicsGame/assets/147593910/37119766-8ce1-4aef-8eec-84717b237387)</br>
모든 페이지는 Page 클래스를 상속하여 Open과 Close 메소드를 용도에 맞게 정의하고 이전 페이지로 이동할 수 있도록 모든 페이지의 참조는 AppManager에 Page로 업캐스팅하여 Stack에서 관리

# 콘텐츠 다운로드
![image](https://github.com/DWBoo/PhonicsGame/assets/147593910/a7fb6c66-ebf5-4cd4-a621-bf682e951fde)</br>
선택 한 나이와 주제에 맞게 게임 콘텐츠 다운로드 여부를 검사 후 게임 진행</br>
# 기본적인 게임 구조
![image](https://github.com/DWBoo/PhonicsGame/assets/147593910/4d91e788-3eec-4085-b288-f40be44959c3)</br>
![image](https://github.com/DWBoo/PhonicsGame/assets/147593910/ee0910b3-797d-4656-9cfd-97e381cb0d0f)</br>
JSON으로 미리 주제와 게임 별로 문제가 정의되어 있다.
Addressable에도 콘텐츠가 문제 혹은 정답과 동일한 이름으로 관리를 하고 있기에 현재 해당하는 문제를 그대로 이름으로 사용하여 다운로드 받은 콘텐츠에서 해당 콘텐츠를 불러와 사용
![image](https://github.com/DWBoo/PhonicsGame/assets/147593910/73720aaa-af34-4f9a-a08f-18c8b8dd2d6d)
버튼 또한 문제들의 이름으로 되어있기에 JSON의 데이터를 기반으로 현재 문제 및 정답 리소스를 사용하며 그 데이터를 기반으로 같은지를 비교하여 정답을 판단
