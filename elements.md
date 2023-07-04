---
title: Elements
feature_text: |
  A demo of Markdown and HTML includes
feature_image: 'https://picsum.photos/2560/600?image=873'
excerpt: A demo of Markdown and HTML includes
aside: true
published: true
---
##  **판다스 정리 part 1**

pd.Series(딕셔너리 데이터) = 딕셔너리를 시리즈(1차원 배열)로 변환

sr.index = 인덱스 배열

sr.values = 데이터 값 배열

pd.DataFrame(딕셔너리 데이터) = 딕셔너리를 데이터프레임(2차원 배열)로 변환

pd.DataFrame(2차원 배열, index = 행 인덱스 배열, columns = 열 이름 배열)로 지정 가능

df.index =[‘  ’, ‘  ’] = 인덱스의 이름 변경 가능 (열 이름(columns)도 가능)

df.rename(index = [] or columns = [], inplace = True) = 행 또는 열 이름의 일부를 선택하여 변경 가능 (단, 원본 객체를 직접 수정하는 것이 아니기 때문에 원본 객체를 수정하려면 inplace = True 를 써줘야 함)

df.drop(행 인덱스, axis = 0) = 행 삭제 (얘도 inplace = True)

df.drop(열 인덱스, axis = 1) = 열 삭제 (얘도 inplace = True)

df.loc[인덱스 이름] = 데이터 프레임의 행 데이터를 선택할 때 사용 (범위 끝 포함)

df.iloc[정수형 위치 인덱스] = (범위 끝 제외)

df[‘열 이름’] or df.열이름 = 열 데이터를 선택할 때 사용 (방법2는 열 이름이 문자열일 때 사용 가능)

df[[‘열1’, ‘열2’, ‘열3’]] = 열 데이터를 여러 개 선택

df.loc[행 인덱스, 열 이름] = 원소 선택 , df.loc[‘행 인덱스’, [‘열 이름’, ‘열이름’]]

df.iloc[행 번호, 열 번호] = 원소 선택

df.loc[‘행 이름’, ‘열 이름’:’열 이름’] = 슬라이싱으로도 가능

df.set_index(‘열 이름’, inplace = True) = 열을 새로운 인덱스로 지정

df[‘추가하려는 열 이름’] = 데이터 값

df.loc[‘새로운 행 이름’] = 데이터 값 (또는 배열) => 행을 추가

