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

## To run the project locally:
   > admin account : `admin@admin.com` and Password: `Passw@rd!123` (You can change it from `appsettings.json` before apply `update database`)

   > Make sure, dotnet core SDK & npm is installed in your machine.

- **Using VS2017**
     ``` 
       > git clone https://github.com/ritwickdey/Cake-Shop.git
       > cd Cake-Shop/
    ```
    - Now Open the `CakeShop.sln` through `VS2017`.
    - Open `appsettings.json` & change the connection string. (But wait! you may not need to change it as this the default connection string of `SQL Server Express` that comes with `Visual Studio`).
    - Hit `Ctrl+Shift+B` to build.
    - Open `Package Manager Console` from `Tools` and enter `update-database`.
    - Hit `Ctrl+F5` to run without debugging.

- **Using CLI**
    ```
        > git clone https://github.com/ritwickdey/Cake-Shop.git
        > cd Cake-Shop/Cake-Shop/
        > npm install
        > dotnet restore
        > set ASPNETCORE_ENVIRONMENT=Development
        > set ConnectionStrings:DefaultConnection="<YOUR CONNECTION STRING>"
        > npm i webpack -g
        > webpack --config webpack.config.js
        > npm run build
        > dotnet build 
        > dotnet ef database update
        > dotnet run 
    ```

## Sceenshots
![screenshot2](./screenshots/screenshot2.png)
![screenshot3](./screenshots/screenshot3.png)
![screenshot4](./screenshots/screenshot4.png)
![screenshot5](./screenshots/screenshot5.png)
![screenshot6](./screenshots/screenshot6.png)
