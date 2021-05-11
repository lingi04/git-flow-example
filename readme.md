# git-flow 설명
## branch 설명
* master : 제품으로 출시될 수 있는 브랜치
* develop : 다음 출시 버전을 개발하는 브랜치
* feature : 기능을 개발하는 브랜치
* release : 이번 출시 버전을 준비하는 브랜치
* hotfix : 출시 버전에서 발생한 버그를 수정 하는 브랜치

## git flow 사용 방법
### step1
1. develop 브랜치에서 feature branch를 생성 한다.
```
git co -b feature/step1-step2-and-step3
```
### step2
1. feature를 개발하고 커밋한다.
### step3
1. develop 브랜치에 머지 한다.
    * 머지 옵션은 트리를 깔끔하게 유지하기 위해 `squash merge`를 했음.
```
# master에 머지
git merge feature/step1-step2-and-step3 --squash
```
