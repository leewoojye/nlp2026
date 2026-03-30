# 자연어처리 강의 과제 및 실습을 위해:

본 강의에서는 파이썬을 사용한다. 파이썬 버전은 최소 3.12 이상인지 확인해 주기 바란다.
파이썬을 처음 설치해야 하는 경우, 컴퓨터에 최소 3GB의 여유 공간을 확보한 후 (https://www.anaconda.com/download/)에서 Anaconda의 최신 파이썬 버전(기본)을 설치하는 것이 가장 간단한 방법이며, 모든 운영체제에서 작동한다.

Anaconda 설치를 마쳤으면, Anaconda Prompt를 열고 다음과 같은 절차를 따라 환경을 설정한다.

## 1. env.yml에 명시된 의존성과 함께 가상환경을 생성(가상환경명: hw1):
    conda env create -f env.yml

## 2. 새로운 가상환경 활성화하여 hw1으로 들어간다:
    conda activate hw1
    
## 3. 생성된 가상환경을 Jupyter Notebook에서 사용할 수 있도록 IPython kernel을 설치: 
 
    python -m ipykernel install --user --name hw1

## 4. 과제가 저장된 디렉터리에서 Anaconda Prompt를 열어 Jupyter Notebook을 실행한 후 과제 노트북을 선택하여 실행:

    jupyter notebook word_vectors.ipynb  
    또는  
    jupyter notebook 실행 후 파일 선택(더블 클릭)  
    
## 5. 사용하고 있는 가상환경을 `hw1`으로 변경하기 위해, 메뉴 바에서 "Kernel" 선택 -> "Change Kernel ..." -> hw1 선택.

## 가상환경 사용을 중단하려면, Anaconda Prompt에서 다음과 같이 명령 실행:
    conda deactivate
