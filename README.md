## 브랜치 목적
추후 도입하고 싶은 기능을 위해 기술을 간단하게 사용해봤다.

&nbsp;

### 추후 도입하고 싶은 기능
사용자를 가입하지 않은 사용자/가입한 사용자로 나누어서 <br/>
가입하지 않은 사용자에게는 시스템이 제공하는 소지품 알림 기능만 제공하고<br/>
가입한 사용자에게는 어떤 기후에서 어떤 소지품을 등록할 것인지<br/>
소지품을 새로 만들어서 등록할 수 있는 기능<br/>

기본적인 기능은 간단하기 때문에 회원가입/로그인 기능이 꼭 필요한지 의문이 들었고<br/>
가입을 하지 않아도 기능이 어느정도 제공되었으면 좋겠다는 생각이 들어서 사용해보았다.<br/>

&nbsp;

### 사용 기술
- Spring Security
- JWT 토큰 방식 인증
- Spring JPA

&nbsp;


### 사용 후기
인증된 사용자와 인증되지 않은 사용자에 따라 접근 권한을 분리하는 것은 충분히 가능할 것으로 보인다.<br/>
다만 사용자 입장에서 소지품 확인 페이지를 확인한다는 로직은 둘 다 똑같은데 <br/>
인증된 사용자의 경우 커스텀 소지품 기능을 추가하는 기능을 어떤 방식으로 덧붙일지 고민이다.<br/>
일단 지금 생각나는 방법은 이렇다.<br/>

1. url을 아예 다르게 만들어서 프론트에서 인증된 사용자와 인증되지 않은 사용자를 다르게 요청하도록 한다
2. 백엔드 로직에서 인증된 사용자의 경우 추가 로직을 실행하도록 한다

일단 이 프로젝트의 구조가 명확히 잡히고 나서 나머지를 고려하는 것이 좋을 것 같아서<br/>
bring-XXX 첫번째 개발을 끝내고 나서 고민해보기로 했다.
