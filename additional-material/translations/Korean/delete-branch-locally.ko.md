# 이 문서는 로컬 저장소에서 브랜치를 삭제하는법을 제공합니다.

브랜치 이름을 실수로 잘못 입력했을대 유용합니다.

이것은 *3*가지 방법으로 할 수 있습니다.

```
git branch -D <브랜치 이름>
```

```
git branch --delete --force <브랜치 이름>  # 위에 -D와 동일합니다.
```

```
git branch --delete  <브랜치 이름>         # unmerge 에러
```

-D는 --delete --force를 의미하며, 브랜치가 병합(merge)되지 않았더라도 강제로 삭제합니다. 하지만 -d 또는 --delete 옵션을 사용하면 브랜치의 병합(merge) 상태에 따라 오류가 발생할 수 있습니다... 