# ARAE

## 목적
- 이 [페이퍼](https://arxiv.org/pdf/1706.04223.pdf)의 한국어 구현.
- NSMC dataset에서 긍부정이 뒤바뀐 텍스트를 생성하는 것이 목표.

## 결과는?
- ~~좋지 않았다...ㅠㅡㅠ~~
- 일단 GAN 학습이 불안정해서 고생했다.
  - mode collapse도 잘 해결이 안 됨.
- autoencoder가 [CLS] 토큰과 hidden state만 주어졌을 때 문장을 생성하는 능력이 너무 떨어져서 word-by-word 식으로 예측하도록 학습 방향을 바꾼 건 fluency 측면에서 어느 정도 유효했던 듯.

## references
- [official_code](https://github.com/jakezhaojb/ARAE)
- [tokenizer](https://github.com/Beomi/KcBERT)
- [NSMC_dataset](https://github.com/e9t/nsmc)
