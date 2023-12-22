# Cake Shop

ASP.NET Core(멀티 페이지 응용 프로그램)로 구축된 샘플 케이크 가게 웹 사이트

![screenshot1](./screenshots/screenshot1.png)

## APP/코드 기능
- 관리자만 케이크 생성/편집/삭제 및 주문 관리를 수행할 수 있습니다.
- 일반 사용자는 케이크를 사고 주문을 볼 수 있을 뿐입니다.
- 쿠키를 이용한 카트 시스템 관리.
- 클라이언트 측과 서버 측의 검증,
- 쿠키 기반 인증 및 승인 - 세션 없음
- '사용자 이름' 또는 '이메일'을 통해 로그인합니다.
- 응답 UI
- 리포지토리 패턴
- 애플리케이션 아키텍처는 ORM(Entity Framework) 형태로 분리됩니다

## 프레임워크 / 라이브러리
- ASP.NET Core 2.0 *(백엔드)*
- Razard View Engine *(마크업 생성용)*
- 엔티티 프레임워크 핵심*(ORM)*
- ASP.NET ID *(쿠키 기반 인증 및 인증 - 세션 아님)*
- AutoMapper *(도메인 모델 & DTO로 매핑하는 경우)*
- jQuery & Boot 4단계

## 프로젝트를 로컬로 실행하려면:
> admin account : 'admin@admin.com ', Passw@rd!123' ('update database' 적용 전에 'appsetings.json'에서 변경 가능)

> 기계에 닷넷 코어 SDK & npm이 설치되어 있는지 확인합니다.

- **VS2017 사용**
```
- 이제 'VS2017'을 통해 '케이크샵.sln'을 오픈합니다.
- 'appsetsettings.json'을 열고 연결 문자열을 변경합니다. (그러나 잠시만요! 'Visual Studio'와 함께 제공되는 'SQL Server Express'의 기본 연결 문자열이므로 변경할 필요가 없을 수도 있습니다.).
- Ctrl+Shift+B를 눌러 빌드합니다.
- Tools에서 Package Manager Console을 열고 update-database를 입력합니다.
- 디버깅 없이 실행하려면 'Ctrl+F5'를 누르십시오.

- **Using CLI**
    ```
        Shop.git
>cd 케이크숍/ 케이크숍/
> npm 설치
> 닷넷 복원
> set ASPNET CORE_ENRVORY= 개발
> set Connection String:DefaultConnection="<YOUR CONNection STRING>"
> npmi 웹팩 -g
> webpack --config webpack.config.js
> npm run build
>닷넷 빌드
> dotnetef 데이터베이스 업데이트
>도트넷 런
    ```

## Sceenshots
![screenshot2](./screenshots/screenshot2.png)
![screenshot3](./screenshots/screenshot3.png)
![screenshot4](./screenshots/screenshot4.png)
![screenshot5](./screenshots/screenshot5.png)
![screenshot6](./screenshots/screenshot6.png)
