## 시간의 흐름 순 (2021-2)
📌 https://github.com/School-is-hard/Chatbot_Buddy  
정확도 올리려고 전처리 했던 기록. colab pro 결제가 필요하다는 점(달에 만삼천원정도 나온다..) & 학기 마무리되면서 멈춤.  

## 여태까지 정확도 정리
|Original(5000,359)|Data 5000 Category 310|Data 5000 Category 191|Data 15000 Category 191|Data 19458 Category 150|
|:----------------:|:--------------------:|:--------------------:|:---------------------:|:---------------------:|
|        40%       |         37.6%        |         46.6%        |          51.4%        |          53.9%        |
  
  카테고리를 약 50% 줄이거나 데이터를 3배로 늘려야 정확도가 겨우 5%가 올라간다는 것을 알 수 있었음.  
  (정확도 올리기 어렵구나..)  
  
  ### 계획
  > ~~1.  카테고리 그대로 두고 데이터를 손본 뒤 학습한다. (카테고리 일부 밀린 것 존재)~~ </br>
  > ~~2.  데이터를 일부 늘린 뒤 학습한다. (20000 목표)~~ </br>
  > ~~3.  카테고리를 더 줄인다. (150 목표)~~ </br>
  > 4.  에포크를 늘린다. 최적의 에포크를 찾는다 </br>
  > 5.  자연스러운 대화를 위한 카테고리를 10개 이내로 추가


## ** 카테고리 그대로 두고 데이터를 손본 뒤 학습한다.
   > 데이터가 많아진만큼 하나하나 정제하기엔 무리가 있는 것 같다.  
   > 대표적인 발화 위주로 크게크게 수 그냥 오래 매진하진 말아야겠음.
## data 16239 Category 186 : 51.2%
> 자꾸 에포크 41에서 멈춰서 오래 걸렸음 ㅠ
> 오래걸린거치고 성과 없음 ㅡㅡ 고작 데이터 천개늘리고 카테고리 5개 줄인 걸로는 차이가 안보이는 듯
## data 19458 Category 150 : 53.9%
> batch size랑 에포크를 조정해봤는데 colab 런타임 연결 방지로 setInterval 사용해도 자꾸 로봇입니까가 뜨거나 연결이 끊어져서 애먹음
> 일단 batch size랑 에포크 그대로 두고 정확도 3퍼 오른듯. 에포크를 늘려봐야지

## 📌사용 언어 모델
WellnessConversation-LanguageModel: https://github.com/nawnoes/WellnessConversation-LanguageModel
