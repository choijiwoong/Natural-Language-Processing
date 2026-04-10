## 01-01 코랩과 아나콘다
- 아나콘다 설치
아나콘다 설치 후 아래 명령어 이용하여 아나콘다 파이썬 패키지 다운. 설치 과정에서 3.13 파이썬이 설치됐는데 텐서플로우는 3.12까지만 지원함. 
pyenv같은거로 버전 switch 해야할듯. 
gemini물어보니 conda에서 가상환경 만들라고 함.

conda create -n tf_env pyton=3.12
conda activate tf_env
pip install tensorflow

conda update -n base conda
conda update -all

- 코랩은 익숙하니 패스

## 01-02 필요한 기본 패키지 설치
- nltk
pip install nltk # 사실 아나콘다 설치 시 기본으로 설치됨.
제대로 nltk사용하기 위해서 
ipython
import nltk
nltk.__version__
확인 후  '3.9.2'
nltk.download() 
로 nltk data를 추가적으로 설치해두자.

- konlpy
한국어 자연어 처리를 위한 형태소 분석기 패키지
pip install konlpy
ipython
import konlpy
konlpy.__version__
확인 하자. '0.6.0'

- jpype
java와 python을 연결해주는 JPype설치해야한다.
직접 파이썬 버전과 OS를 보고(https://github.com/jpype-project/jpype/releases) 알맞은 버전을 설치하자.
pip install jpype1-1.7.0-cp312-cp312-win_amd64.whl
까지 완료.

## 01-03 머신 러닝 워크플로우
