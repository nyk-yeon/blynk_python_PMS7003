

# Blynk python PMS7003예제 for 라즈베리파이

**라즈베리파이**에서 사용되는 **Blynk python 버전**의 **PMS7003 데이터 수신**예제 코드입니다.  
Blynk python 구성품 키트 정보는 아래 페이지를 참고 해 주세요  
-준비 중  


## menual

사용자  매뉴얼 입니다.  

- 제품 구성 및 조립 방법 등이 자세히 설명되어 있습니다.  
-준비 중  

## 사용 전 필수 라이브러리

https://github.com/vshymanskyy/blynk-library-python  
위 라이브러리를 필수로 설치해 주셔야 합니다.   

라즈베리파이에서 위 라이브러리 설치 시 아래 명령으로 실행해야 합니다.   
>(python3 사용)  
>``sudo pip3 install blynk-library-python``

## bly_PMS7003.py
  
blynk 연결을 위한 **사용자 토큰**을 아래 *YourAuthToken*에 입력하고  
``BLYNK_AUTH =  'YourAuthToken'``  
  
 **시리얼 설정(#USE PORT)** 부분(하단 코드 참고)을 연결 방식에 맞춰 수정해준 뒤   
```
# UART / USB Serial
USB0 =  '/dev/ttyUSB0' # USB 사용시 / USB0이 아닌경우 변경 
UART =  '/dev/ttyAMA0' # UART 사용시  
  
# USE PORT  
SERIAL_PORT = UART  #연결방식에 맞춰 변경
  
#serial setting  
ser = serial.Serial(SERIAL_PORT, Speed, timeout = 1)  
```  
``sudo puthon3 bly_PMS7003.py``  
위 명령어로 실행해 주시면 됩니다.

## PMS7003.py
PMS7003 먼지센서의 Python 용 라이브러리 입니다.
https://github.com/eleparts/PMS7003
위 링크를 참고해 주시면 됩니다.

