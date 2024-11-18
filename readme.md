[ENG](#ENG)   
[한국어](#한국어)

## ENG
# News-Title Topic Classification in Data-Centric View Project

In this project, we aim to enhance the performance of sentence topic classification through data preprocessing without modifying the model.   
We improved the dataset quality by removing stopwords, punctuations (',', '!', '$', '(', ')', '*', '%', '@'), and duplicated words. Additionally, to address data imbalance, we employed various data augmentation techniques, including Easy Data Augmentation, Back Translation with the T5 model, chatGPT, data crawling, and utilization of Open Government Data(https://www.data.go.kr/en/index.do). Furthermore, we tackled label errors by removing or relabeling data with high error probabilities. The text perturbation cleaning process involved preprocessing original articles and replacing them with modified data. We re-labeled existing data to resolve label errors using the 'bash1130/bert-base-finetuned-ynat' model, fine-tuned with the KLUE-YNAT dataset.


## 한국어
# level2_nlp_datacentric-nlp-13

## ✅ 목차
[1. 정보](##-📜-정보) > [2. 진행 과정](##-진행-과정) > [3. 팀원](##-팀원) > [4. 역할](##-역할) > [5. 디렉토리 구조](##-%EB%94%94%EB%A0%89%ED%86%A0%EB%A6%AC-%EA%B5%AC%EC%A1%B0) > [6. 프로젝트 구성](##-프로젝트-구성)

➡️ [랩업 리포트 보기](https://docs.google.com/document/d/1uA5vxG0wrwAiOJLM7RKzawpjKWJ0YfSN0XgTKUeqoFg/edit?usp=sharing)
<br>

## 📜 정보
- 주제 : 부스트캠프 5기 Level 2 프로젝트 - 주제 분류 프로젝트(Data Centric TC)
- 프로젝트 기간 : 2023년 5월 22일 ~ 2023년 6월 1일
- 프로젝트 내용 : 모델을 수정하지 않고 데이터 가공을 통해 모델의 문장 주제 분류 성능을 향상

<br>

## 🗓️ 진행 과정


<br>

## 👨🏼‍💻 팀원

<table>
    <tr height="160px">
        <td align="center" width="150px">
            <a href="https://github.com/Yunhee000"><img height="120px" width="120px" src="https://avatars.githubusercontent.com/Yunhee000"/></a>
            <br/>
            <a href="https://github.com/Yunhee000"><strong>김윤희</strong></a>
            <br />
        </td>
        <td align="center" width="150px">
            <a href="https://github.com/8804who"><img height="120px" width="120px" src="https://avatars.githubusercontent.com/8804who"/></a>
            <br/>
            <a href="https://github.com/8804who"><strong>김주성</strong></a>
            <br />
        </td>
        <td align="center" width="150px">
            <a href="https://github.com/ella0106"><img height="120px" width="120px" src="https://avatars.githubusercontent.com/ella0106"/></a>
            <br/>
            <a href="https://github.com/ella0106"><strong>박지연</strong></a>
            <br />
        </td>
        <td align="center" width="150px">
            <a href="https://github.com/bom1215"><img height="120px" width="120px" src="https://avatars.githubusercontent.com/bom1215"/></a>
            <br/>
            <a href="https://github.com/bom1215"><strong>이준범</strong></a>
            <br />
        </td>
        <td align="center" width="150px">
            <a href="https://github.com/alicehjjung"><img height="120px" width="120px" src="https://avatars.githubusercontent.com/alicehjjung"/></a>
            <br/>
            <a href="https://github.com/alicehjjung"><strong>정효정</strong></a>
            <br />
        </td>
    </tr>
</table>
<br>

## 🧑🏻‍🔧 역할

| 이름 | 역할 |
| :----: | --- |
| **김윤희** | 데이터 증강(EDA,역번역) |
| **김주성** | 깃헙 기본 세팅, 데이터 크롤링 |
| **박지연** | 데이터 증강(EDA, 공공데이터 추가), 데이터 전처리(키워드 추출)  |
| **이준범** | 데이터 크롤링, 데이터 클리닝(Text perturbation, Label Error)  |
| **정효정** | 데이터 증강(chatGPT 이용), 데이터 전처리(불용어 및 특수문자 제거,한자->한글 변환), 텍스트 relabeling |

<br>

## 📁 디렉토리 구조

```bash
code
┣ Data_Augmentation
┃ ┣ confusionMatrix.ipynb
┃ ┣ data_augmentation.py
┃ ┣ eda_aug.py
┃ ┣ news_crawler.py
┃ ┗ sample.ipynb
┣ Data_Cleaning
┃ ┣ find_noise.py
┃ ┣ get_original_text.py
┃ ┣ preprocess.ipynb
┃ ┣ reLabeling.ipynb
┃ ┗ word_cloud.ipynb
┗ utils
┃ ┣ analyze_tools.py
┃ ┣ clean_lab.py
┃ ┗ get_keywords.py
Exploratory_Data_Analysis
┣ EDA_JHJ.ipynb
┗ EDA_KJS.ipynb
```
<br>

## ⚙️ 프로젝트 구성
