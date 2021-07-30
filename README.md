# mobile-invitation-2107
demo: https://csslick.github.io/mobile-invitation-2107/  

## 모바일 청첩장 프로젝트
1. 자료조사 및 시안제작(XD)
2. 구현
	- 전화걸기
	- 갤러리
	- 지도
	- 앱 호출 및 지도 연결(API 활용)
3. 포트폴리오 구성 후반작업
	- PC용 페이지에서 보기(목업프레임)
	- Mobile


## 앱 링크 관련 SDK 추가 및 실행 방법
1. 카카오
```
    <!-- kakao API 추가 -->
    <script src="//developers.kakao.com/sdk/js/kakao.min.js"></script>
    <script>
      var app_key = '앱키';

      Kakao.init(app_key);

      // 모바일 카카오네비 앱 실행
      function kakao_navi() {
      
        if (is_pc == '1') {
          alert('모바일 기기 전용 기능입니다')
        }

        Kakao.Navi.start({
          name: '김포웨딩홀', // 목적지
          x: 126.70317468513564,  // 위도
          y: 37.63051488108245,  // 경도
          coordType: 'wgs84'
        });
        return false;
	
      }
    </script>  
```


2. 티맵
```
  <a 
    href="https://apis.openapi.sk.com/tmap/app/routes?appKey=앱키&name=목적지명&lon=위도값&lat=경도값"
  >
    <img src="images/tmap-icon.png" alt="티맵">
  </a>
```
- API 홈페이지 https://openapi.sk.com/ 


