# NLP_Analysis_of_Lyrics_Trend_and_WordCloud 
이 프로젝트는 자연어처리 수업의 1인 기말 프로젝트입니다.<br>
This project is the solo term project of the NLP course.

### Project Title
빌보드(1964~2015) 노래 가사 분석에 따른 시대별 트렌드 파악 & 워드클라우드 추출 <br>
NLP_Analysis_of_Lyrics_Trend_and_WordCloud 

### Team(팀구성)
김예빈
Myself

개인 프로젝트로 진행합니다.

### Purpose(목적)
1964~2015년도까지의 모든 빌보드 Top100 가사를 분석하는 것이 목표입니다. <br>
분석이란 해당 시대의 특징을 밝히는 것부터 nlp를 통해 관찰할 수 있는 것들을 포함하며 이 프로젝트에서는 특히, 그 시대의 특징을 알아내고자 합니다.<br>
또한, nlp의 tf-idf, word2vec 등을 이용하여 가사들의 분포나 빈도, 관계를 알아내고자 합니다.<br>

### Description(작품 설명)
1. 빌보드 가사 데이터 셋을 가져옵니다<br>
Classify the songs using the billboard lyrics dataset.
  ~~* 빌보드 가사 데이터 셋이 유효하게 동작하지 않는다면 빌보드의 차트와 곡 정보만 표시된 데이터를 가져옵니다.<br>
    If the dataset is invalid, using other dataset(billboard chart, song information).~~
  ~~* 해당 데이터를 바탕으로 노래 가사를 따로 크롤링 등의 방법으로 수집하여 저장합니다. <br>
    Base on the other dataset, store songs' lyrics using crawling.~~
    * 추출된 가사는 각 시대의 트렌드를 반영한다고 볼 수 있습니다.<br>
    We can find the lyrics extracted can reflect the trend of the times. 

2. 1964~2015년도의 빌보드 차트와 유효한 가사가 데이터셋으로 주어지면 60s, 70s, 80s, 90s, 00s, 10s로 시대별로 분류합니다. <br>
Classify the songs by the era(decades).

3. 데이터를 전처리합니다.<br>
Preprocessing the data.

4. 데이터의 TF-IDF를 구합니다.<br>
Get the TF-IDF of billboard data.

5. TF-IDF에 따라 클러스터링을 진행하고 해당 결과를 시각화하여 데이터 분포를 확인합니다.<br>
Clustering with the TF-IDF, visualize the result.

6. word2vec을 이용하여 클러스터링을 진행하고 결과를 시각화하여 벡터화된 시대별 데이터를 분석합니다.<br>
Clustering with the word2vec, visualize the result.

7. TF-IDF를 이용하여 시대별로 추출된 가사를 각각 단어의 빈도에 따라 워드클라우드로 만듭니다.<br>
Visualize the every eras' lyrics as wordcloud using TF-IDF.

8. 워드클라우드만 보고 그 시대의 감성의 트렌드를 파악하고자 하는 것이 이 작품의 목표입니다.<br>
The purpose of this project is find the sentiment trend of the eras by just watching the 'wordcloud'.

### Result

#### Clustering Analysis Plot

##### 1960s
![data60s_cluster_plot](https://user-images.githubusercontent.com/49120917/170030218-eb9510ec-6026-4942-af15-b72ab33b2f83.png)
![data60s_SSE_cluster_center_plot](https://user-images.githubusercontent.com/49120917/170030222-e24ff033-7d01-4051-b10b-31f7fe691d62.png)

##### 1970s
![data70s_cluster_plot](https://user-images.githubusercontent.com/49120917/170030227-13ba8145-42a2-4fd1-a7bc-c4d76c2a6c8e.png)
![data70s_SSE_cluster_center_plot](https://user-images.githubusercontent.com/49120917/170030229-873552d8-afbd-42e9-ae79-bdbeaf115a22.png)

##### 1980s
![data80s_cluster_plot](https://user-images.githubusercontent.com/49120917/170030234-a2bd5ea6-386e-411d-96a0-afc46ca1bffa.png)
![data80s_SSE_cluster_center_plot](https://user-images.githubusercontent.com/49120917/170030235-59c46bcb-a87c-4bcf-9349-61564acf0e91.png)

##### 1990s
![data90s_cluster_plot](https://user-images.githubusercontent.com/49120917/170030239-92e78f92-0a18-4d8c-b543-8be833438e05.png)
![data90s_SSE_cluster_center_plot](https://user-images.githubusercontent.com/49120917/170030241-a1f5379c-6d54-4f0b-a7b4-f8e7e361b5a0.png)

##### 2000s
![data00s_cluster_plot](https://user-images.githubusercontent.com/49120917/170030193-238120b4-2cc2-4d65-a568-d06d848456a3.png)
![data00s_SSE_cluster_center_plot](https://user-images.githubusercontent.com/49120917/170030202-522b7f18-152e-4768-8e09-8af9cda9ee0d.png)

##### 2010s
![data10s_cluster_plot](https://user-images.githubusercontent.com/49120917/170030208-c893aef8-ec24-47bb-a794-22cc8a0677ec.png)
![data10s_SSE_cluster_center_plot](https://user-images.githubusercontent.com/49120917/170030212-13347e8d-9be6-416d-aaf8-a43a09af3a7a.png)


#### Word2vec Visualization

##### 1960s
![word2vec_60s](https://user-images.githubusercontent.com/49120917/170039905-06577422-6f95-4e46-a664-8a4b2efa1e8f.png)
##### 1970s
![word2vec_70s](https://user-images.githubusercontent.com/49120917/170039915-f6b38a70-01ce-4227-b8e9-388b6136f7bb.png)
##### 1980s
![word2vec_80s](https://user-images.githubusercontent.com/49120917/170039922-f79ace20-eb90-49b5-a3cc-c7dae6dd6fa3.png)
##### 1990s
![word2vec_90s](https://user-images.githubusercontent.com/49120917/170039933-56c40afd-343f-4380-88d1-21aac9d6f4f1.png)
##### 2000s
![word2vec_00s](https://user-images.githubusercontent.com/49120917/170039873-fe8867a0-eb4c-4081-b049-ddb24f53176e.png)
##### 2010s
![word2vec_10s](https://user-images.githubusercontent.com/49120917/170039900-918d5e0e-3576-4c33-81a2-365d74c99c21.png)

#### WordCloud Using TF-IDF
![data60s_tfidf_wordcloud](https://user-images.githubusercontent.com/49120917/170029969-066d7b85-9fc2-4253-bb52-b365712ad145.png)
![data70s_tfidf_wordcloud](https://user-images.githubusercontent.com/49120917/170029973-55a7a683-c68a-4194-a0a9-e9957b2262d4.png)
![data80s_tfidf_wordcloud](https://user-images.githubusercontent.com/49120917/170029975-cab70d7a-f516-4803-9cd0-5796d9ee1b0a.png)
![data90s_tfidf_wordcloud](https://user-images.githubusercontent.com/49120917/170029976-f8e44c2b-30ad-4e0d-b9b9-4940e7a24cdc.png)
![data00s_tfidf_wordcloud](https://user-images.githubusercontent.com/49120917/170029951-447fe050-2e4f-4a8b-bf99-237e50ff7e23.png)
![data10s_tfidf_wordcloud](https://user-images.githubusercontent.com/49120917/170029964-b17b9950-fdc0-4c9a-92e8-cc500f6820b4.png)


### 결론 Conclusion
tfidf를 이용해 클러스터링을 한 결과 그래프를 관찰하면 60s~80s는 몰려있는 경향을 보이며 그 이후는 좀 더 다양하게 퍼져있는 것을 볼 수 있다. <br>
SSE를 이용해서 최적 elbow를 구하고자 했지만 그래프들이 선형을 그리거나 너무 왔다갔다 하는 경향을 보여 이를 이용하지 않고 그냥 임의의 개수를 이용해 클러스터링을 진행하였다.<br>
데이터가 너무 많았기 때문에 20개의 클러스터로 분류했다.<br>
하지만 조금이나마 elbow에 가까운 값을 이용했어야 했는데 이를 이용하지 않고 그냥 클러스터 개수를 나눠서 그런지 성능이 매우 좋다고는 하기 어렵다.<br>

word2vec을 이용해 클러스터링한 결과를 보게 되면 각 시대별로 단어들의 관계를 시각적으로 볼 수 있다. 어떤 단어들 간에 더 관계가 있는 단어인지는 실행한 결과나 첨부한 이미지를 보면 쉽게 확인할 수 있다. 각 시대별로 어떤 단어들이 같이 쓰인 것이 많은지 확인할 수 있는데 재밌는 것은 style을 각 시대별로 출력한 결과다. 각 시대마다 같이 쓰인 단어가 모두 다르며 특히, 2010년대에는 style과 가장 연관있는 단어로 gangnam, oppa 등이 나온다. 강남스타일 노래 가사가 나온 것이다. 물론 이걸 가사로 학습시키면서 우리가 아는 일반적인 word2vec과는 답이 다르게 나올 수 있지만 가사들 간 얼마나 가까운지를 확인하는 기능은 잘 이뤄지고 있는 것으로 판단된다.

tf-idf를 이용해 wordcloud를 만든 결과를 보면 전체적으로 love, like 와 같은 긍정적인 감정이 주를 이룬다. 그런데 여기서 재밌는 것은 00s, 10s의 wordcloud를 자세히 보면 nigga, bitch, fuck 과 같은 욕설들이 보인다. <br>
분명 사랑과 같은 긍정적인 감정이 주인 것은 맞지만 시대가 변해가면서 2000년대에 들어설수록 사람들은 자기 감정에 보다 더 솔직해지고 직설적인 화법이 유행하기 시작했음을 알 수 있다.<br>

10s의 경우 2010~2015년의 빌보드 차트를 분석한 결과이기 때문에 현재와 약 7년 간의 공백이 존재한다. 

7년 간의 공백이 존재하지만 위의 결과로 이 공백 기간을 추측하고 앞으로의 가사 추세도 예측해 볼 수 있다. wordcloud에서 추측한 정서와 유사하게 요즘 나오는 노래 중에는 대놓고 욕설이 들어간 노래들이 매우 많은데 이를 통해 공백 기간에는 가사에 더 많은 욕설이 포함될 것을 추측할 수 있다. 또한, 빌보드에서 장기 석권을 이룬 BTS의 dynamite를 생각해보면 코로나 시기를 겪으면서 위로가 되는 노래가 유행을 타기도 했다. 지금까지 분석한 wordcloud의 가사에는 긍정적인 감정의 단어가 주를 이뤘다면 앞으로는 긍정과 부정이 주가 없이 유사한 비율로 이뤄질 것으로 예측된다.


### Dataset
kaggle에서 제공하는 데이터셋을 활용할 예정이지만, 적절한 데이터셋이 더는 제공되지 않아 프로젝트 주제를 변경하거나 크롤링을 통한 데이터셋으로 바뀔 수 있습니다.<br>
Using the Kaggle Dataset, but there are valid datasets no longer.
The title or dataset can be changed.

https://www.kaggle.com/datasets/dhruvildave/billboard-the-hot-100-songs

https://www.kaggle.com/datasets/deepshah16/song-lyrics-dataset

https://raw.githubusercontent.com/walkerkq/musiclyrics/master/billboard_lyrics_1964-2015.csv

### Reference
https://can-do.tistory.com/138?category=804018
https://github.com/Madhakee01/WordCloud-Generator/blob/main/word_cloud_gen.ipynb
https://www.kaggle.com/code/jbencina/clustering-documents-with-tfidf-and-kmeans/notebook
