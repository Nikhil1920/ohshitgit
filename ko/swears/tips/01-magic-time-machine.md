---
tags: tip
title: 젠장, 뭔가 단단히 잘못됐는데, 다 뒤엎고 예전으로 돌리고 싶어!
id: magic-time-machine
order: 1
---

```git
git reflog
# git의 모든 브랜치에서 있었던
# 지금까지의 모든 기록을 볼 수 있다
# 각각 HEAD@{index} 형태로 index를 가지고 있으니,
# 잘못되기 전에 해당하는 index를 찾고
git reset HEAD@{index}
# 타임머신을 타자!
```

이 기능은 실수로 지운 파일을 되돌리거나, 뭔가 잘못 수정한 걸 되돌리거나, 실수로 머지한 걸 되돌리거나, 됐고 그냥 잘 작동했던 때로 돌아가고 싶을 때 사용하면 된다. 나는 개인적으로 `reflog`를 **엄청** 많이 사용하고, 당신들도 사용해볼 것을 아주 아주 아주 추천한다!