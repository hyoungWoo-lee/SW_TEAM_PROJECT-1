# Git workflow
---
![gitwork](https://user-images.githubusercontent.com/31719859/95296918-8eed8b80-08b4-11eb-9b30-cab185ef1e37.jpg)
5명의 팀원으로 구성된 팀으로, 아래와 같이 작업을 진행합니다.

+ 각자 자신이 fork해온 repo에서 작업합니다.
+ 작업이 끝나면 팀 repo에 pull request를 보냅니다.
+ merge 권한은 팀장에게 있습니다.
우선 다음과 같은 브랜치를 사용합니다.
1. master branch : 배포되었거나 배포될 소스가 저장되는 브랜치(태그를 달아서 관리)
2. hotfix branch : 배포된 버전에 생긴 버그를 긴급히 수정하는 브랜치
3. release branch : 배포될 준비가 되어 QA가 예정된 소스를 저장하는 브랜치
4. develop branch : 전반적인 개발이 진행되는 브랜치
5. feature branch : 기능 단위 개발이 진행되는 브랜치