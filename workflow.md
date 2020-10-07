
![KakaoTalk_20200918_160511958](https://user-images.githubusercontent.com/55039857/95293019-9b221a80-08ad-11eb-862c-127d7b95724c.jpg)
+ 일반적으로 기능 개발을 하고 배포하기 때문에 merge 과정은 feature -> develop -> release -> master 브랜치 순으로 진행됩니다.
(hotfix는 경우에 따라 예외적으로 사용)
+ 먼저 새로운 기능은 새로운 feature 브랜치를 생성해 개발하되, 반드시 master 브랜치가 아닌 develop 브랜치에서 새로운 브랜치를 생성해 사용해야 합니다.
기능 개발이 완료되면 다시 develop 브랜치와 병합합니다. 
+ 실수로 master 브랜치와 병합하지 않도록 주의해야 합니다.
+ 마지막으로 release 브랜치에서 QA를 진행하고 문제가 없을 시 release 브랜치를 master 브랜치와 develop 브랜치로 각각 merge 하여 한 버전을 마무리합니다.


