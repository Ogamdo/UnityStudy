#Unity
#Game
#개념

Unitydml Component들
-컴포넌트 = 기능단위=클래스
	이들을 모아서 게임 오브젝트(태그, 단순히 이름역할)을 구성한다.

Class에서 생성자를 통해 객체를 만드는 것과는 대조적이다.


```C#
void start(){
Rigidbody ball = GetComponent<Rigidbody>();
}
```

위 코드는 정상작동한다 하지만  아래의 코드는 오류가 난다.

```C#
public class KickOff: MonoBehaviour
{
	Rigdibody ball = GetComponent<Rigidbody>();
void start(){

}
	
}
```

유니티 엔진이 돌아가야 Componet속성이 갖춰져서 일까?
