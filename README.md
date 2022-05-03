# NLP_Analysis_of_Lyrics_Trend_and_WordCloud
# 빌보드(1964~2015) 노래 가사 분석에 따른 시대별 트렌드 파악 & 워드클라우드 추출
This project is the solo term project of the NLP course.

## Team(팀구성)
김예빈
Myself

This is the solo term project.
개인 프로젝트로 진행합니다.

### Description(작품 설명)
1. 빌보드 가사 데이터 셋을 통해 시대별로 노래를 분류합니다.
Classify the songs using the billboard lyrics dataset.
  * 빌보드 가사 데이터 셋이 유효하게 동작하지 않는다면 빌보드의 차트와 곡 정보만 표시된 데이터를 가져옵니다.
    If the dataset is invalid, using other dataset(billboard chart, song information).
  * 해당 데이터를 바탕으로 노래 가사를 따로 크롤링 등의 방법으로 수집하여 저장합니다. 
    Base on the other dataset, store songs' lyrics using crawling.
2. 1964~2015년도의 빌보드 차트와 유효한 가사가 데이터셋으로 주어지면 60s, 70s, 80s, 90s, 00s, 10s로 시대별로 분류합니다. 
Classify the songs by the era(decades).

3. 분류된 노래의 가사를 word2vec을 이용해 분석하여 각 시대마다 많이 쓰인 가사를 추출합니다. 
Analysis the lyrics using word2vec, and extract the most frequent lyrics.

4. 추출된 가사는 각 시대의 트렌드를 반영한다고 볼 수 있습니다.
We can find the lyrics extracted can reflect the trend of the times. 

5. 시대별로 추출된 가사를 워드클라우드로 만들어 시각화합니다.
Visualize the every eras' lyrics as wordcloud.

6. 워드클라우드만 보고 그 시대의 감성의 트렌드를 파악하고자 하는 것이 이 작품의 목표입니다.
The purpose of this project is find the sentiment trend of the eras by just watching the 'wordcloud'.

### Dataset
Using the Kaggle Dataset, but there are valid datasets no longer.
The title or dataset can be changed.
kaggle에서 제공하는 데이터셋을 활용할 예정이지만, 적절한 데이터셋이 더는 제공되지 않아 프로젝트 주제를 변경하거나 크롤링을 통한 데이터셋으로 바뀔 수 있습니다.

https://www.kaggle.com/datasets/dhruvildave/billboard-the-hot-100-songs
https://www.kaggle.com/datasets/deepshah16/song-lyrics-dataset
https://raw.githubusercontent.com/walkerkq/musiclyrics/master/billboard_lyrics_1964-2015.csv
