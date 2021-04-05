# LikeLion_EDA

멋쟁이 사자처럼 EDA 공유 코드입니다.  

This is test branch for using colab with data.

---

### 데이터 설명
**Case**  
환자들 데이터
> case_id : 7자리로 이루어짐. case_id = region_code(5) + case_number(2)  
> province : 지역(특별시, 광역시, 도)
> city : 지역(시, 군, 구)  
> group : 집단 감염 여부  
> infection_case : 감염 집단 이름, etc 값도 존재한다.  
> confirmed :  누적 수  
> latitude : 위도  
> longitude : 경도  

**PatientInfo**    
환자 별 역학 조사 데이터
> patient_id : 10자리로 이루어짐. patient_id = region_code(5) + patient_number(5)  
> global_num : Busan은 global_num이 존재하지 않는다.  
> sex : 성별  
> birth_year :  생년  
> age  :  나이(0s, 10s, 20s 등으로 표현)  
> country : 소속 국가  
> province : 지역(특별시, 광역시, 도 기준)  
> city : 지역(시, 군, 구)  
> disease : 기저 질환 여부  
> infection_case : 감염 집단 이름  
> infection_order : 감염 순서  
> infected_by : 해당 환자를 감염시킨 환자의 id  
> contact_number : 접촉 수  
> symptom_onset_date : 증상 발생일  
> confirmed_date : 감염 확정 일자  
> released_date : 격리 해제 일자  
> deceased_date : 사망 일자  
> state : 상태  

**PatientRoute**  
환자들 경로 분석 데이터
> patient_id  
> global_number  
> date : YYYY-MM-DD  
> province :  지역(특별시, 광역시, 도 기준)  
> city : 지역(시, 군, 구)  
> latitude : 위도  
> longitude : 경도  

**Policy**  
정책 적용 데이터
> policy_id  
> country : Korea  
> type : 적용 분야(기술, 사회, 교육 등)
> gov_policy : 적용 정책 명
> detail : 상세 내용  
> start_date : 정책 시작일  
> end_date : 정책 종료일  

**Region**
지역 별 위치 및 통계 데이터  
> code : 지역 코드  
> province : 지역(특별시, 광역시, 도)  
> city : 지역(시, 군, 구)  
> latitude : 위도  
> longitude : 경도  
> elementary_school_count : 초등학교 수  
> kindergarten_count : 유치원 수  
> university_count : 대학 수  
> academy_ratio : 학원 비율  
> elderly_population_ratio : 노인 인구 비율  
> elderly_alone_ratio : 독거노인 가구 비율  
> nursing_home_count : 요양원 수  

**SearchTrend**  
검색된 키워드 트렌드  
> date : YYYY-MM-DD  
> cold : 감기 검색량  
> flu  : 독감 검색량  
> pneumonia : 폐렴 검색량  
> coronavirus : 코로나 바이러스 검색량  

**SeoulFloating**  
> date : YYYY-MM-DD  
> hour : 시간(0~23)  
> birth_year : 나이(0, 10, 20 ...)  
> sex : 성별  
> province : 지역(특별시, 광역시, 도 기준)  
> city : 지역(시, 군, 구)  
> fp_num : 유동 인구 수  

**Time**  
COVID-19 시계열 데이터  
> date : YYYY-MM-DD  
> time : 시간(0, 16만 존재)  
> test : 누적 검진 수  
> negative : 음성 누적 수  
> confirmed : 양성 누적 수  
> released : 격리 해제 누적 수  
> deceased : 사망 누적 수  

**TimeAge**  
COVID-19 시계열 데이터(나잇대 별 누적 환자 수 및 사망 수)  
> date : YYYY-MM-DD  
> time : 시간(0만 존재)  
> age : 나이(0s, 10s, 20s 등으로 표기)  
> confirmed : 확진자 누적 수  
> deceased : 사망자 누적 수  

**TimeGender**  
COVID-19 시계열 데이터(성별 별 누적 환자 수 및 사망 수)  
> date : YYYY-MM-DD  
> time : 시간(0만 존재)  
> sex : 성별  
> confirmed : 확진자 누적 수  
> deceased : 사망자 누적 수  

**TimeProvince**  
COVID-19 시계열 데이터(province 별 누적 환자 수 및 사망 수)  
> date : YYYY-MM-DD  
> time : 시간(0, 16만 존재)  
> province : 지역(특별시, 광역시, 도 기준)  
> confirmed : 확진자 누적 수  
> released : 격리 해제 누적 수  
> deceased : 사망 누적 수  

**Weather**  
지역별 기상자료  
> code : 지역 코드  
> province : 지역(특별시, 광역시, 도 기준)  
> date : YYYY-MM-DD  
> avg_temp : 평균 온도  
> min_temp : 최저 온도  
> max_temp : 최고 온도  
> precipitation : 일일 강수량  
> max_wind_speed : 최대 풍속  
> most_wind_direction : 가장 빈번한 바람 방향  
> avg_relative_humidity : 평균 상대 습도  

