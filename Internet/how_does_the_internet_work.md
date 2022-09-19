# 🌍인터넷은 어떻게 동작할까?

인터넷은 웹의 핵심적인 기술이다. 인터넷의 가장 기본적인 것은 컴퓨터들이 서로 통신 가능한 거대한 네트워크라는 것이다.

### 단순 네트워크

두 개의 컴퓨터가 통신이 필요할 때 우리는 다른 컴퓨터와 물리적으로(이더넷 케이블) 또는 무선으로(WiFi, Bluetooth)으로 연결되어야 한다.

![](https://github.com/ingyeomnote/TIL/blob/main/Internet/images/network_01.png?raw=true)

위의 네트워크는 2대의 컴퓨터로 제한되지 않고 원하는 만큼의 컴퓨터를 연결할 수 있다. 하지만, 10대를 연결한 다고 가정하면 각 컴퓨터끼리 연결할(10*9)/2 = 45개의 케이블이 필요하게 된다. 이를 그물형 접속형태(mesh topology)라고도 한다.


![](https://github.com/ingyeomnote/TIL/blob/main/Internet/images/network_02.png?raw=true)

이러한 문제를 해결하기 위해 네트워크의 각 컴퓨터는 라우터라고 하는 특수한 소형 컴퓨터에 연결된다. 이 라우터는 생각보다 간단한 작업을 하는데, 그냥 컴퓨터에서 보낸 데이터가 올바른 대상 컴퓨터에 잘 전달하게 해주는 것이다. 예를 들어 컴퓨터 B에게 메시지를 보내려면 컴퓨터 A는 먼저 메시지를 라우터에 전송하고, 그 다음 라우터가 메시지를 컴퓨터 B에게 전달한다. 이 때, 라우터는 메시지가 다른 컴퓨터에 가지 않도록 제어한다.

![](https://github.com/ingyeomnote/TIL/blob/main/Internet/images/network_03.png?raw=true)


https://mungto.tistory.com/300#%EB%8B%A8%EC%88%9C_%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC