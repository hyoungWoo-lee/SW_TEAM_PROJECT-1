# Git workflow

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


![KakaoTalk_20200918_160511958](https://user-images.githubusercontent.com/55039857/95293019-9b221a80-08ad-11eb-862c-127d7b95724c.jpg)
+ 일반적으로 기능 개발을 하고 배포하기 때문에 merge 과정은 feature -> develop -> release -> master 브랜치 순으로 진행됩니다.
(hotfix는 경우에 따라 예외적으로 사용)
+ 먼저 새로운 기능은 새로운 feature 브랜치를 생성해 개발하되, 반드시 master 브랜치가 아닌 develop 브랜치에서 새로운 브랜치를 생성해 사용해야 합니다.
기능 개발이 완료되면 다시 develop 브랜치와 병합합니다. 
+ 실수로 master 브랜치와 병합하지 않도록 주의해야 합니다.
+ 마지막으로 release 브랜치에서 QA를 진행하고 문제가 없을 시 release 브랜치를 master 브랜치와 develop 브랜치로 각각 merge 하여 한 버전을 마무리합니다.

First, we use these branches:
1. master : Branch where the sources to be released or released are stored, (managed by attaching tags)
2. hotfix : Branch for fixing critial bugs in the released version
3. release : Branch where the sources are stored, which are ready to be released after QA 
4. develop : Branch where the overall development is in progress
5. feature : Branch where functional unit development is in progress

Generally, merge process proceeds in the order of this : feature -> develop -> release -> master (hotfix branch is used as an exception)
First, a new feature is developed by creating a new 'feature' branch. It must be came from the develop branch, not the master branch.
And when the feature development is done, It must be merged with the develop branch again. Be careful not to merge with the master branch.
Finally, QA will be proceeded in the release branch. And if there is no problem, the release branch will be is merged into the master branch and the develop branch, 
respectively, to finish the one version.
