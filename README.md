## README
### 참고 사이트
[SHAP 모델 설명](https://moondol-ai.tistory.com/378)  
[SHAP 공식문서](https://shap-lrjball.readthedocs.io/en/latest/index.html)  

[python code 참조 - 1](https://moondol-ai.tistory.com/394)  
[python code 참조 - 2](https://data-newbie.tistory.com/433)

### 실행방법
1. conda 가상환경 생성
    - python : 3.9.17
2. pip 이용해서 해당 프로젝트의 requirements.txt 로 환경구축
    ```shell
    pip install -r requirements.txt
    ```
3. ./data 폴더에 Database.db 파일 넣을 것

### SHAP 모델이 지원하는 라이브러리
>  shap 은 model 라이브러리 version 에 크게 영향을 받지 않음

1. #### xgboost
    설치 version : 2.0.0 [최신 2023.10.15 기준]
    > - 1.x.x 버전에서도 잘 작동하는 것 확인  
    > - 아래 둘중 하나 설치
    ```shell
    pip install xgboost
    ```
    ```shell
    pip install xgboost==2.0.0
    ```
2. #### catboost  
    설치 version : 1.1.1
    > - shap 에서 기본적으로 catboost 1.2 지원하지만 설치 안되는 경우가 있음.  
    > - 1.2 이상 설치가 안되면 1.1.1 로 설치 진행
    ```shell
    pip install catboost=1.1.1
    ```
3. #### tensorflow [shap 모델에 test 해보지 않음]
    설치 version : 2.13.0
    ```shell
    pip install tensorflow==2.13.0
    ```

4. #### pytorch
    설치 version : 2.0.1 
    ```shell
    pip install torch==2.0.1
    ```