from pathlib import Path
dir_path = Path('C:/myPyAI/code/st/text_app.py')
dir_path.mkdir(parents=True, exist_ok=True)
print("{0} 디렉토리 존재 여부: {1}".format(dir_path,dir_path.exists()))
%%writefile C:/myPyAI/code/st/text_app.py
    
import streamlit as st
import numpy as np
import pandas as pd

from PIL import Image




st.title("[가로등 종합 관리 솔루션]")
st.header("")
st.header("")



st.subheader(" 대구광역시 가로등 데이터 + 인공위성 데이터")


def load_html_file(file_path):
    with open(file_path, 'r', encoding='utf-8') as f:
        html = f.read()
    return html


# HTML 파일 경로 설정
html_file_path = "C:/Users/junhyeong/Downloads/circled_lightmap_with_brightness.html"  # 여기에 실제 파일 경로를 입력하세요.

# HTML 파일을 불러온 후 출력
html_content = load_html_file(html_file_path)
st.components.v1.html(html_content, width=800, height=600)


tab1, tab2, tab3 = st.tabs(['Tab A' , 'Tab B', 'Tab C'])

with tab1:
  #tab A 를 누르면 표시될 내용
  image_url = "https://blogger.googleusercontent.com/img/a/AVvXsEhMryj65ZL7O7KGjWQCAaEd9zd_Zl3d3GPhL4aOKiL_Nrh6qAXpI-NlPHoOUXAimA8896ZfKyEQ1McXDZRAjUj72ALPmfeuC1E9bnZpVkl0voM6LnHoplzMHtJSYEX1kz2w348M1iOcE5flDYBzlD7T2fYByRb6kzQ4lbyQPQSD5gEKt3qvLaC5hKIXaYU"
  st.image(image_url, width=500, caption=None)

with tab2:
  #tab B를 누르면 표시될 내용 
  image_url = "https://blogger.googleusercontent.com/img/a/AVvXsEgibPR0VQ_bi-IPIxhbh1CEJDjTVJ-pBMPKXI5_UYUq5DtlKHPFcdkep4CL_ECYD_aT-u1FuNey2H6mY38QBHHECaaku3nET9iE6vcmf-R2XM0yxAs8YQPQbg9huDDk_D0lZaKTaQOfPJf5UVLQkQeS0pUGi3J9q4sm8Z9qPlKtabTT6whe2u-oQ4EqfWY"
  st.image(image_url, width=500, caption=None)

with tab3:
  #tab B를 누르면 표시될 내용 
  image_url = "https://blogger.googleusercontent.com/img/a/AVvXsEh_Jv3XsgxbCtdGeqV-iJcGXxYuNTh37QS2vdi57JvQEjU92pFEd4jHztuNsCH5k_Ym1J3Xs2tccKKGHtJvaMW2Zyv3CuyCqla_Sa3NJ0uU5YwL2AJdLznAZlu3v_-KfiTch1_8_k4DdQTcP7HlD1PqxEHSY6YvlOJ2dJWZYL8FzaOr819KtZZLFAkyhiI"
  st.image(image_url, width=500, caption=None)



#-----------------------------------------------------------------------

col1,col2 = st.columns([3,3])
# 공간을 2:3 으로 분할하여 col1과 col2라는 이름을 가진 컬럼을 생성합니다.  

with col1 :
  # column 1 에 담을 내용
  st.subheader('대구공공시설관리공단')
with col2 :
  # column 2 에 담을 내용
  st.subheader('가로등 관리')
  st.checkbox('자동차 전용도로와 12m 이상 도로에 설치된 가로등')


# with 구문 말고 다르게 사용 가능 
col1.text('지방공기업법과 대구공공시설관리공단 설치 조례에')
col1.text('의하여 공공시설을 관리 운영함으로써 시민의 편익도모와 복리증진')
col2.checkbox('절연저항이 불량한 지중선을 정비하고 노후 가로등 교체') 
#=>위에 with col2: 안의 내용과 같은 기능을합니다
    
#----------------------------
    
#st.sidebar는 

st.sidebar.title('WEAREALL : 우리는 전부')
st.sidebar.header("<가로등 정비 솔루션 POC>")

# 사이드바에 체크박스, 버튼등 추가할 수 있습니다! 
tab1, tab2= st.sidebar.tabs(['Tab A' , 'Tab B'])

with tab1:
  #tab A 를 누르면 표시될 내용
  image_url = "https://blogger.googleusercontent.com/img/a/AVvXsEhN4019BLBDsgYTzFZjdXBlYJdgiq0aBCcwaph8nsdSkyeooMzyVIldqYgjbkP2ybSdYJ_Mu6UAbsOpjkcktn5WjhqtWclymvlvrDc5KvluRCx6Zoqb8wCovuOQt9E92DNVEXhtFEzmIGWOVjbpGsk2YeyGUZR_AYxI4Cksz_Tl_iT4Y3ypcqY5MdHAgEI"
  st.image(image_url, width=250, caption=None)

with tab2:
  #tab B를 누르면 표시될 내용 
  image_url = "https://blogger.googleusercontent.com/img/a/AVvXsEgibPR0VQ_bi-IPIxhbh1CEJDjTVJ-pBMPKXI5_UYUq5DtlKHPFcdkep4CL_ECYD_aT-u1FuNey2H6mY38QBHHECaaku3nET9iE6vcmf-R2XM0yxAs8YQPQbg9huDDk_D0lZaKTaQOfPJf5UVLQkQeS0pUGi3J9q4sm8Z9qPlKtabTT6whe2u-oQ4EqfWY"
  st.image(image_url, width=250, caption=None)
    

#------------------------------------------------------------------------

st.header("")
st.header("")





from typing import Any
from typing import cast

st.subheader("대구시 가로등 데이터")

#입력창
usr_text=st.text_input('가로등 위치', value="입력", max_chars=None)
#숫자입력
st.number_input('가로등 관리 번호',min_value=None, max_value=None, value=1000000,step=None)
#날자 입력
st.date_input('탐지 날짜',value=None,min_value=None,max_value=None)
st.date_input('위성 이미지 날짜',value=None,min_value=None,max_value=None)

from io import BytesIO
folder='C:/myPyAI/data/'
with open(folder + "가로등 고장_Data.txt", encoding='utf-8') as text_file:
    text_data=text_file.read()
st.download_button(label='고장 DB 생성',
                   data = text_data,
                   file_name="가로등_고장 Data.txt"
)

st.header("")
st.header("")



st.header("")
st.header("")
st.header("")

 
# uploaded_file = st.file_uploader("CSV 파일을 선택하세요", type='csv')

# if uploaded_file is not None:

#    st.dataframe(uploaded_file)


#def main():
#  df = pd.read_csv('"/바탕 화면/대구공공시설관리공단_가로등시스템 고장등관리_20230825.csv"', encoding='utf-8')
#st.dataframe(df)


#st.dataframe(df, height=300)


#df = pd.DataFrame(data={
#    '가로등 번호':['a','b','c'],
#})
#st.write(df)
#st.dataframe(df)
#st.table(df)



#csv_file_path = '/바탕 화면/대구공공시설관리공단_가로등시스템 고장등관리_20230825.csv'
# CSV 파일을 데이터 프레임으로 읽습니다.
## 문자열로 데이터 타입을 설정하고 CSV 파일을 읽습니다.
#def main():
#    df = pd.read_csv(csv_file_path, dtype=str)


# 데이터 프레임 내용을 확인합니다.
#print(df)

def main() :

    language = ['남구', '수성구', '달성군', '동구', '북구', '달서구', '중구', '서구']
    st.multiselect('구청을 선택하세요. 복수 선택 가능', language)
    

if __name__ == "__main__" :
    main()

def main() :
    df = pd.read_csv("C:\myPyAI\data\대구공공시설관리공단_가로등시스템 고장등관리_20230825.csv", encoding='utf-8')

    with st.expander('데이터프레임 보기') :
        st.dataframe(df)

if __name__ == "__main__" :
    main()
  

#--------------------------------------    
def load_html_file(file_path):
    with open(file_path, 'r', encoding='utf-8') as f:
        html = f.read()
    return html
