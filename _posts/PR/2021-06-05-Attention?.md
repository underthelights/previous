## Ablation study for Transformer Architecture

### Papers

- [Are Pre-trained Convolutions Better than Pre-trained Transformers?](https://arxiv.org/pdf/2105.03322.pdf)
- [Pay Attention to MLPs](https://arxiv.org/pdf/2105.08050.pdf)
- [MLP Mixer](https://arxiv.org/pdf/2105.01601.pdf)
- [FNet: Mixing Tokens with Fourier Transforms](https://arxiv.org/pdf/2105.03824.pdf?fbclid=IwAR0CeMAz0v-EJTEUwYZLz9SuVeeKVYGXJFyQIWVnaXhJsvryLQzcWLfIKiA)

### thoughts

- 논문들은 읽어보시면 되고, 간단하게 말하면 attention구조가 생각보다 별 필요가 없다는 연구들입니다.
- 한편 이에 대조되는 연구들도 최근에 보입니다. 대표적으로 DINO가 있겠죠. 
  - [DINO](https://arxiv.org/pdf/2104.14294.pdf?fbclid=IwAR1l4SbTTYMpYujnN9SQGnKn0WCDcHzpsIgU9WM6KUABj8BZ6Adu1MnE-s0)
  - 요즘 같은 Tr구조로 SOTA찍는 판에서(...) 흥미롭게 읽을만 합니다.

- 제 생각엔 일단 "그럼에도 불구하고" 여전히 attention 구조들은 상당히 좋습니다. MHA는 사실 잘 생각해보면 다소 어색한 gaussian, 즉 엄밀히 말하면 "hand-crafted" kernel matrix가 들어간 (물론 정확히 gaussian kernel은 아니지만, 뭐 무슨 뜻인지 다들 아시겠죠) feedforward layer입니다. 
  - 여기서 이 kernel 자체가 무엇일지는 사실상 생각보다 크리티컬 하지 않다는 연구들은 원래는 그렇게 놀랍지 않아야합니다. Fnet이나 gMLP 같은 경우 pre-norm + residualness는 여전히 유지하고 있기 때문이죠. Performer 같은 접근 방법은 이걸 굳이 다시 gaussian으로 approximate하려 했습니다. 
  - 비슷한 맥락으로 하필 gaussian은 low-rank스럽게 (당연히 그 자체로 low rank는 아닙니다 ㅋㅎ) 유지해진다는 특징이 있기에 좋았던걸수도 있습니다(그만큼 VC dim이 줄어드니까요). 
- 요지는, 최근의 연구들은 attention 말고도 좋은게 있나느걸 제안해주지, 이 선택 자체가 한심하다는걸 말해주는건 절대 아닌 것 같습니다.
- 그래도 앞으로 연구들이 attention구조를 잘 generalize하는 방향으로 가는건 확실해 보일 것 같습니다. 아예 $$S^n$$ 이 아닌 다른 공간들을 생각하는 케이스들도 점점 많아집니다.

- 그리고 마지막으로, 어느 정도는 이제 구조가 문제는 아니다라는 말을 해주는 것 같기도 합니다. 정말 지금 있는 기술로 만들 수 있는 가장 좋은 모델이랑 가장 멍청한 모델 (MLP) 를 가져와도 같은 방법론을 써도 차이가 안난다면 저희는 이제 일반적인 Representation learning (SSL이나 multitask RL) 같은거에 더 집중해야 할 차례가 아닌가 싶습니다. 물론 아니나 다를까 이런 연구들이 지금 제일 활발하긴 합니다.

