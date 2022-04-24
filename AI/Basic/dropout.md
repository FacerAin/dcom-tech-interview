## Dropout이란?
**일부 파라미터를 학습에 반영하지 않음으로써 모델을 일반화하는 방법**    
모델의 overfitting을 방지하기 위한 대표적인 방법입니다.

![image](https://user-images.githubusercontent.com/16442978/164978715-9bfc9e5c-fb5e-4ba7-b14a-61ea37603c2c.png)

## Dropout이 성능을 향상시키는 이유는?
1. **Co-adaption(동조 현상) 예방**  
Co-adaption이란 한 노드가 다른 노드에 의존하여 학습되는 방식을 의미합니다. 이때, 여러 노드에서 중복된 feature를 추출하여 학습의 효율성이 떨어질 수 있습니다.
Dropout은 학습마다 새로운 노드를 샘플링하므로, 각 노드가 meaningful feature를 학습할 수 있습니다.
2. **앙상블 효과**  
매 학습마다 다른 조합의 노드로 구성되기 때문에 앙상블 효과를 얻을 수 있습니다.
3. **오버피팅 방지**  


![image](https://user-images.githubusercontent.com/16442978/164978845-03c47a32-8b57-4ad1-8194-f218b6d69173.png)

## Dropout에 단점은 없나요?
1. Dropout의 Rate가 너무 높을 경우 underfitting이 발생할 수 있습니다.
2. 같은 모델 대비 학습 시간이 증가하게 됩니다.

## Reference
- [https://hanlue.tistory.com/23](https://hanlue.tistory.com/23)
