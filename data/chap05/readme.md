# 5장. 다층 퍼셉트론 모델 구조 : 꽃 이미지 분류 신경망
5장에서는 예제 실습을 위해 캐글의 꽃 분류 데이터셋 파일들과 1장, 2장, 3장의 데이터 파일들을 이용합니다.<br/>
꽃 분류 데이터셋 파일들은 캐글 사이트에서 직접 다운로드 받아야 합니다.<br/>
또한 1장, 2장, 3장의 데이터가 각 단원 폴더에 준비되어 있지 않으면 오류가 발생합니다.

## 캐글 사이트에서 꽃 분류 데이터셋 다운받기
깃허브 용량 관계상 꽃 분류 데이터셋은 여기 수록하지 못하며 따라서 사용자별로 각자 다운로드받아야 합니다.<br/><br/>
꽃 분류 데이터셋 접근 경로는 https://www.kaggle.com/alxmamaev/flowers-recognition 입니다.<br/>
데이터 다운로드를 위해서는 먼저 캐글 사이트에 회원가입과 로그인(Sign in)을 해야 합니다.<br/>
캐글에 로그인된 상태에서 위의 경로에 접근해 'Download (225 MB)' 버튼을 클릭하면 flowers.zip 압축파일을 다운로드받을 수 있고
압축을 풀면 맨 위에 flowers 폴더가 만들어지며 그 안에 다섯 가지 꽃 이름(daisy,  dandelion,  rose,  sunflower,  tulip)의 서브 폴더들이 생깁니다.
각 서브폴더에는 폴더 별로 734개에서 1055개까지 총 4326개의 jpg 이미지 파일들이 있습니다.
<br/><br/>
실험을 위해서는 flowers 폴더가 /data/chap05 폴더 밑에 오면 됩니다.

## 이전 단원 데이터 폴더에서 가져와 이용하는 데이터 파일
아래의 파일들도 준비되어 있어야 오류 없이 실습이 수행됩니다.<br/><br/>
/data/chap01/abalone.csv<br/>
/data/chap02/pulsar_stars.csv<br/>
/data/chap03/faults.csv<br/>