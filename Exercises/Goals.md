### 실습을 위한 atlas, R server
ATLAS: http://zarathuohdsi.ap-northeast-2.elasticbeanstalk.com/
Rstudio server: http://rstudio.zarathuohdsi.ap-northeast-2.elasticbeanstalk.com/

Rstudio server에서 ConnectionDetails.R 파일 열면 DB 접속 정보가 있습니다.
- 두 번째의 postgresql 접속정보는 쓸 일 없습니다. 지워주셔도 됩니다.
- 데이터베이스는 두 종류로 23m 이 더 큰 데이터입니다. 대부분은 100k 데이터로 충분하고, 희귀케이스인 경우 23m 을 이용하면 됩니다.

참고로 이 환경은 AWS와 연계된 https://github.com/OHDSI/OHDSIonAWS 로 만들었습니다. 

### 목표1) ATLAS에서 연구 설계한 후, R에서 실행하여 결과 확인하기(shiny 웹으로 나옴) 
### 목표2) ATLAS에서 코호트만 설계한 후 나머지는 R에서 직접 분석하기.
