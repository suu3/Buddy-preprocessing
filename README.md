학습 뭐가잘못됐는지 보기 위해..  
## 학습 시킬 때 주의할 점
* wellness.py 안 카테고리 수 수정
  
## 시간의 흐름 순 ~
* 데이터 15000개 & 카테고리 191 : wellness 카테고리 합치고 감성말뭉치 발화 섞음
  - 정확도 구려서(0.4😱) 데이터 탓인가 하고 감성말뭉치 데이터를 빼보기로 함. (레포지토리 생성 전이라 ipynb 파일 X)

* 데이터 안늘리고 카테고리 191: (8.10)
  - 1차 시도 : 역시나 정확도 구려서 다시 확인해봤더니 일부 삭제 안한 감성말뭉치 데이터가 있었음.  
     큰 영향은 없을거라 생각했지만 일단 잘 대조해보기 위해 다시 삭제하고 2차시도로 넘어감.
    
  - 2차 시도 : EOR 에러가 남... 해결방법 찾아봐도 파이썬 재설치하라는 말밖에 없어서 그냥 한번 더 함
  - 3차 시도 : 에러는 없었으나 정확도 구림 🤔
    > ### 3차시도 후 원인 분석
    >  1. ~~수동으로 전처리하다가 일부 카테고리가 밀렸는데 놓친 게 남아있었다.~~
    >  2. 모호함에 너무 많은 데이터가 들어갔다.
    >  3. 카테고리별 데이터 개수가 천차만별이다
    >     
    >      -> 하지만 이걸로 정확도가 이렇게까지 낮게 ..? 🤔

  - 4차 시도(8.12) : 1번(a.)을 수정하고 학습 -> 역시 원인이 아니었다.  
     > 더 이상 계속해보는건 무의미하므로 원데이터에서 카테고리 수를 줄여본다.  
     > (처음부터 카테고리 조금씩 줄여나갈걸 빨리하겠다고... 후회 중 😂😂)  
     > ### 현재 원인 2(b.)번 예상
  
* 데이터 안늘리고 카테고리 310: (8.12)
  - 이번에도 안되면 내 문제이므로 오리지널 데이터 돌려서 비교해본다.  
     
  - 남편 등등은 지우기로 했지만 데이터가 많이 빠지면 또 비교가 힘들 것 같아서 일단은.. 냅뒀다.     
  새 공포증 등등은 데이터 수가 적어서 삭제. 
    
    > ### 결과
    > what??? 1.7??? 왜 카테고리를 줄이고 데이터를 늘릴수록 정확도가 거지같은거지 🥶  
    > 내 문제일 확률이 있으므로 오리지널 데이터로 돌려본다
  
* 오리지널 데이터 (8.13)  
  학습돌려보려는데 google drive 파일 업로드가 안됨  
  진짜 개빡치는군
