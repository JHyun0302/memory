## Inflearn

<img src="https://github.com/JHyun0302/server/assets/60764632/24cec8a1-ddb4-42c4-8e5b-2ff8d8fe6f49"  width="600" height="300"/>

### 강의명 : [스프링 부트 - 핵심 원리와 활용](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81%EB%B6%80%ED%8A%B8-%ED%95%B5%EC%8B%AC%EC%9B%90%EB%A6%AC-%ED%99%9C%EC%9A%A9)

- 지식공유자 : 김영한

### 강의 내용

- 스프링 부트가 제공하는 5가지 핵심 기능
    1. 내장 서버
    2. 자동 라이브러리 관리
    3. 자동 구성
    4. 외부 설정
    5. 모니터링 & 관리 기능

    - 정리 : 자동 구성 라이브러리 만들기
        - `@ConditionalOnProperty(name = "memory", havingValue = "on")`
            - `memory=on` 이라는 환경 정보가 있을 때 라이브러리 적용 (= 스프링 빈 등록)
        - 자동 구성 대상 지정
            - `org.springframework.boot.autoconfigure.AutoConfiguration.imports`
                - 스프링 부트는 위의 파일 정보 읽어서 자동 구성으로 사용
        - 빌드
            - 명령어 : `./gradlew clean build`
            - 결과 : `build/libs/memory-v2.jar`