학습 뭐가잘못됐는지 보기 위해..

## 시간의 흐름 순 ~
* 데이터 15000개 & 카테고리 191 : wellness 카테고리 합치고 감성말뭉치 발화 섞음
  - 정확도 구려서 데이터 탓인가 하고 감성말뭉치 데이터를 빼보기로 함.

* 데이터 안늘리고 카테고리 191: (8.10)
  - 1차 시도 : 역시나 정확도 구려서 다시 확인해봤더니 일부 삭제 안한 감성말뭉치 데이터가 있었음.


    큰 영향은 없을거라 생각했지만 일단 잘 대조해보기 위해 다시 삭제하고 2차시도로 넘어감.
    
  - 2차 시도 : EOR 에러가 남... 해결방법 찾아봐도 파이썬 재설치하라는 말밖에 없어서 그냥 한번 더 함
  - 3차 시도 : 에러는 없었으나 정확도 구림 🤔
