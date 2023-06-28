# HTML/CSS 프로젝트



## Project Info

- 프로젝트 조 : 10조 - 팀명 : 겁나 십조
- 프로젝트 팀원 : 이재호(조장), 장효윤(조원), 김남진(조원), 백상호(조원, 스크럼마스터)
- 프로젝트 주제 : 마켓칼리
- 배포주소 : //

<br><br>

---
## 결과물
<br><br>



--- 

## 프로젝트를 하며 좋았던 점
<br>

이재호
> 멋사에서 처음 진행한 프로젝트였지만 좋은 팀원분들을 만나 덕분에 프로젝트를 잘 진행하였습니다. 프로젝트를 하며 좋았던 점 몇 가지를 이야기 하자면 협업하는 과정에서 github를 사용하여 풀리퀘스트를 하고 공통 저장소에 merge하는 작업방법을 알 수 있어서 좋았고, 이를 pull로 당겨와 작업브랜치에 merge 하는 과정에서 발생하는 충돌을 해결해나가는 과정을 경험해볼 수 있어서 좋았습니다. 또한 문제 상황에 놓였을 때 팀원분들의 도움을 받거나 반대로 팀원분들이 도움이 필요할 때 제가 도와드릴 수 있는 부분에서 도움을 드리며 서로 잘 상호작용이 이루어져서 좋았습니다.

<br><br>

## 프로젝트를 하며 힘들었던 점
<br>

이재호
> 아무래도 처음하는 프로젝트이다 보니 구체적인 계획을 세우지 못하였고 실행해나가는 과정에서 많은 이슈들이 생겨서 예상했던 시간을 초과하는 등 일정에 차질이 생기기도 하였고, 팀원들마다 프로젝트 진행도가 달라서 일정을 컨트롤 하고 알맞게 계획을 재조정 하는 일이 어려웠습니다. 그리고 마크업 구조를 작성할 때 최대한 시맨틱하게 마크업을 하는 것과 웹 접근성을 많이 고려하며 작성하려고 노력하였지만 해당 작업을 하며 자세히 모르는 부분이 많아서 관련 정보나 예시를 찾아보다보니 생각보다 많은 시간이 소요되어서 힘들었습니다.
<br>

---
<br>

### HTML

---

<details>
<summary>공통 헤더</summary>
<div markdown="1">

```
<header>

    <div class="headerContainer">
      <!-- 서치박스 영역 -->
      <div class="searchContainer">

        <!-- logo css에서 백그라운드 이미지 처리-->
        <div class="logoContainer">
          <h1 aria-label="마켓칼리">
            <a href="/" class="logoKarly">
              <span class="a11y">마켓컬리</span>
            </a>
          </h1>


          <div class="switchContainer">
            <a href="/" class="market__link">마켓칼리</a>
            <span class="divider" aria-hidden="true">|</span>
            <a href="/" class="beauty__link">뷰티칼리</a>
          </div>

        </div>

        <!-- 검색 영역 -->
        <div class="formContainer">
          <form action="/" class="searchForm" method="post">
            <label for="search">검색어</label>
            <input type="search" id="search" class="searchForm__input" aria-label="검색창" required aria-required="true"
              placeholder="검색어를 입력해주세요" />

            <button type="submit" class="searchIcon search__button" aria-label="검색"></button>
          </form>

        </div>



        <!-- 아이콘 영역 -->
        <ul class="memberIcon" aria-label="멤버서비스 링크 아이콘">
          <li><a href="/" class="locationIcon"><span class="a11y">배송지 설정</span></a></li>
          <li><a href="/" class="heartIcon"><span class="a11y">찜하기</span></a></li>
          <li><a href="/" class="blackCart__Icon"><span class="a11y">장바구니</span></a></li>
        </ul>
      </div>


      <h2 class="a11y">HeaderNavigation</h2>
      <!-- 네비게이션 영역 -->
      <nav class="nav">
        <!-- 햄버거 버튼 카테고리 -->
        <button type="button" class="nav__button">카테고리</button>
        <ul class="nav__list" aria-label="네비게이션 주요 메뉴">
          <li><a href="/">신상품</a></li>
          <li><a href="../views/productList.html">베스트</a></li>
          <li><a href="/">알뜰쇼핑</a></li>
          <li><a href="/">특가/혜택</a></li>
        </ul>

        <a href="/" class="nav__link">
          <span class="link__color">샛별&#183;낮 </span>배송안내
        </a>
      </nav>

      <!-- 회원가입 영역 -->
      <ul class="memberOnly" aria-label="멤버서비스">
        <li class="memberOnly__list">
          <!-- <span class="divider" aria-hidden="true">ㅣ</span> -->
          <a href="/" class="member__signUp">회원가입</a>
        </li>
        <li class="memberOnly__list">
          <span class="divider" aria-hidden="true">ㅣ</span>
          <a href="/" class="member__signIn">로그인</a>
        </li>
        <li class="memberOnly__list">
          <span class="divider" aria-hidden="true">ㅣ</span>
          <a href="/" class="member__cusCenter">고객센터</a>

        </li>
      </ul>

    </div>


    <div class="headerBanner" aria-label="헤더 배너">
      <a class="headerBanner__link" href="/">지금 가입하고 인기상품 <span class="bold">100원</span>에 받아가세요!</a>
      <button type="button" class="cancelIcon headerBanner__button" aria-label="닫기"></button>

    </div>
  </header>

```

</div>
</details>

<br>

<details>
<summary>공통 푸터</summary>
<div markdown="1">

```
<footer aria-label="푸터">

    <h2 class="a11y">Footer</h2>

    <div class="footerTop">
      <div class="footerInfo">
        <div class="customerService">
          <h3 class="happyCenter">고객행복센터</h3>

          <!-- 기타 문의 -->

          <dl class="numberInquiry">
            <dt class="a11y">전화문의</dt>
            <dd class="centerNumber">1644-1107</dd>
            <dd class="centerTime">월~토요일 오전 7시 ~ 오후 6시</dd>
          </dl>

          <dl class="kakaoInquiry">
            <dt class="a11y">카카오톡 문의</dt>

            <dd>월~토요일
              <span class="dividerCustomer" aria-hidden="true">|</span>
              오전 7시 ~ 오후 6시<br />

              일/공휴일
              <span class="dividerCustomer" aria-hidden="true">|</span>
              오전 7시 ~ 오후 1시
            </dd>
            <dd>
              <button type="button" class="inquiryButton">카카오톡 문의</button>
            </dd>
          </dl>

          <dl class="oneononeInquiry">
            <dt class="a11y">일대일 문의</dt>

            <dd>365일<br />고객센터 운영시간에 순차적으로 답변드리겠습니다.</dd>
            <dd>
              <button type="button" class="inquiryButton" aria-label="일대일 문의 버튼">1:1 문의</button>
            </dd>
          </dl>

          <dl class="bulkInquiry">
            <dt class="a11y">대량주문 문의</dt>

            <dd>월~금요일
              <span class="dividerCustomer" aria-hidden="true">|</span>
              오전 9시 ~ 오후 6시<br />
              점심시간
              <span class="dividerCustomer" aria-hidden="true">|</span>
              낮 12시 ~ 오후 1시
            </dd>
            <dd>
              <button type="button" class="inquiryButton">대량주문 문의</button>
            </dd>
          </dl>


          <!-- 이메일 문의 -->
          <address class="nonMember" aria-label="비회원 문의 영역">
            비회원 문의 : <span class="primary">help@karlycorp.com</span><br />
            비회원 대량주문 문의 : <span class="primary">help@karlycorp.com</span>
          </address>

        </div>
        <div class="about">
          <ul class="about__nav" aria-label="칼리 관련 정보 링크">
            <li><a href="/">칼리소개</a></li>
            <li><a href="/">칼리소개영상</a></li>
            <li><a href="/">인재채용</a></li>
            <li><a href="/">이용약관</a></li>
            <li><a href="/">개인정보처리방침</a></li>
            <li><a href="/">이용안내</a></li>
          </ul>
          <address class="about__info" aria-label="칼리 관련 정보">
            법인명 (상호) : 주식회사 컬리
            <span class="dividerAbout" aria-hidden="true">|</span>
            사업자등록번호 : 261-81-23567
            <span class="dividerAbout" aria-hidden="true">|</span>
            <a href="/" class="primary">사업자정보 확인</a><br />
            통신판매업 : 제 2018-서울강남-01646 호
            <span class="dividerAbout" aria-hidden="true">|</span>
            개인정보보호책임자 : 이원준<br />
            주소 : 서울특별시 강남구 테헤란로 133, 18층(역삼동)
            <span class="dividerAbout" aria-hidden="true">|</span>
            대표이사 : 김슬아<br />
            입점문의 : 입정문의하기
            <span class="dividerAbout" aria-hidden="true">|</span>
            제휴문의 :
            <span class="primary">business@karlycorp.com</span><br />
            채용문의 :
            <span class="primary">recruit@karlycorp.com</span><br />
            팩스 : 070 - 7500 - 6098


          </address>

          <ul class="snsContainer" aria-label="s n s 바로가기">
            <li><a href="/" class="blog"><span class="a11y">칼리 네이버 블로그 바로가기</span></a></li>
            <li><a href="/" class="facebook"><span class="a11y">칼리 페이스북 바로가기</span></a></li>
            <li><a href="/" class="instagram"><span class="a11y">칼리 인스타그램 바로가기</span></a></li>
            <li><a href="/" class="naverPost"><span class="a11y">칼리 네이버 포스트 바로가기</span></a></li>
            <li><a href="/" class="youtube"><span class="a11y">칼리 유튜브 바로가기</span></a></li>
          </ul>
        </div>
      </div>
      <div class="footerCompany">
        <ul class="companyWrap" aria-label="마켓컬리 인증서">
          <li class="company__list">
            <a href="/" class="isms">
              <span class="a11y">i s m s 인증서</span>
              [인증범위] 마켓칼리 쇼핑몰 서비스 개발 운영
              (심사받지 않은 물리적 인프라 제외) <br />
              [유효기간] 2022.01.19 - 2025.01.18
            </a>
          </li>
          <li class="company__list">
            <a href="/" class="privacy">
              <span class="a11y">이 프라이버시 플러스 인증서</span>
              개인정보보호 우수 웹사이트 <br />
              개인정보처리시스템 인증(ePRIVACY PLUS)
            </a>
          </li>
          <li class="company__list">
            <a href="/" class="toss">
              <span class="a11y">토스페이먼츠 인증서</span>
              토스페이먼츠 구매 안전(에스크로) 서비스를 이용하실 수 있습니다.
            </a>
          </li>
          <li class="company__list">
            <a href="/" class="woori">
              <span class="a11y">우리은행 인증서</span>
              고객님이 현금으로 결제한 금액에 대해 우리은행과 채무지급보증 계약을 체결하여 안전거래를 보장하고 있습니다.
            </a>
          </li>
        </ul>
      </div>
    </div>

    <div class="footerBottom">
      <span>마켓컬리에서 판매되는 상품 중에는 마켓컬리에 입점한 개별 판매자가 판매하는 마켓플레이스(오픈마켓) 상품이 포함되어 있습니다.</span>
      <span>마켓플레이스(오픈마켓) 상품의 경우 컬리는 통신판매중개자로서 통신판매의 당사자가 아닙니다. 컬리는 해당 상품의 주문, 품질, 교환/환불 등 의무와 책임을 부담하지 않습니다.</span>
      <small>&copy; KURLY CORP. ALL RIGHTS RESERVED</small>
    </div>
  </footer>
```
</div>
</details>

<br>

<details>
<summary>ProductLIst 페이지 메인</summary>
<div markdown="1">

```
 <main class="mainContainer">

    <h2 class="a11y">main</h2>

    <h3 class="productList__title">베스트</h3>

    <div class="productContainer">

      <!-- 사이드바 -->

      <div class="sideBar" role="group" aria-label="사이드바 메뉴">

        <div class="sideBar__button" aria-label="사이드바 필터">
          <span>필터</span>
          <a href="" class="reset__button">초기화</a>
        </div>

        <button class="sideBar__button" type="button">
          <span>카테고리<span class="grayNum__small" aria-hidden="true">1</span></span>
          <span class="arrowBottom"></span>
        </button>

        <button class="sideBar__button__clicked" type="button">
          <span>브랜드</span>
          <span class="arrowTop"></span>
        </button>
        <ul class="brand" aria-label="브랜드별 상품 보기">
          <li class="brand__list"><a href="" class="brand__link">감자밭<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">강남면옥<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">경남제약<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">경복궁<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">고래사<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">고메공방<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">고온어다이어트<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">교토마블<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">그래놀라 하우스<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="brand__list"><a href="" class="brand__link">그리츠 시그니처 램<span class="grayNum" aria-hidden="true">1</span></a></li>
          <li class="btn__list"><button type="button" class="more__button">브랜드 더보기</button></li>
        </ul>

        <button class="sideBar__button" type="button">
          <span>가격</span>
          <span class="arrowBottom"></span>
        </button>

        <button class="sideBar__button" type="button">
          <span>혜택</span>
          <span class="arrowBottom"></span>
        </button>

        <button class="sideBar__button" type="button">
          <span>유형</span>
          <span class="arrowBottom"></span>
        </button>

        <button class="sideBar__button" type="button">
          <span>특정상품 제외</span>
          <span class="arrowBottom"></span>
        </button>

      </div>



      <!-- 프로덕트 영역 -->
      <div class="product">
        <div class="menuContainer" role="menu" aria-label="베스트 상품 메뉴바">
          <span class="bold__main">총 284건</span>
          <ul class="menu__wrap">
            <li><a href="" class="recommend"><span class="bold__main">추천순</span></a></li>
            <li><span class="divider" aria-hidden="true">ㅣ</span>
              <a href="/" class="/">신상품순</a>
            </li>
            <li><span class="divider" aria-hidden="true">ㅣ</span>
              <a href="/" class="/">판매량순</a>
            </li>
            <li><span class="divider" aria-hidden="true">ㅣ</span>
              <a href="/" class="/">혜택순</a>
            </li>
            <li><span class="divider" aria-hidden="true">ㅣ</span>
              <a href="/" class="/">낮은 가격순</a>
            </li>
            <li><span class="divider" aria-hidden="true">ㅣ</span>
              <a href="/" class="/">높은 가격순</a>
            </li>
          </ul>
        </div>

        <div class="product__line" aria-label="상품정보" role="group">
          <ul class="product__wrap">
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품이름 풀무원 탱탱쫄면 사 개입">[풀무원] 탱탱쫄면 (4개입)</span>
                  <span class="product__price" aria-label="상품 가격 4980 원">4,980 원</span>
                  <span class="product__summary" aria-label="상품 설명 튀기지 않아 부담없는 매콤함">튀기지 않아 부담없는 매콤함</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">풀무원 탱탱쫄면</figcaption>
                  <img src="../images/product01.png" class="product__img" alt="풀무원 탱탱쫄면 이미지">

                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 온더바디 죠르디 시카 자석 선쿠션">[온더바디] 죠르디 시카 자석 선쿠션</span>
                  <span class="product__price" aria-label="상품 가격 32500원">32,500 원</span>
                  <span class="product__summary" aria-label="상품 설명 끈적임 없이 보송한 무기자차 선쿠션">끈적임 없이 보송한 무기자차 선쿠션</span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">죠르디 시카 자석 선쿠션</figcaption>
                  <img src="../images/product02.png" class="product__img" alt="죠르디 시카 자석 선쿠션 이미지">

                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 프로쉬 베이비 세탁세">[프로쉬] 베이비 세탁세</span>
                  <span class="discount">
                    <span class="discountRate" aria-label="할인율 24%">24%</span>
                    <span class="discountPrice" aria-label="할인된 가격 18900원">18,900 원</span>
                  </span>
                  <span class="nonDiscount" aria-label="할인전 가격 24900원">24,900 원</span>
                  <span class="product__summary" aria-label="상품 설명 성분을 꼼꼼히 따져 골라 더욱 편안한">성분을 꼼꼼히 따져 골라 더욱 편안한</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">베이비 세탁세</figcaption>
                  <img src="../images/product04.png" class="product__img" alt="베이비 세탁세 이미지">

                </figure>
                <span class="cartIcon"></span>
              </a></li>
          </ul>
          <ul class="product__wrap">
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품이름 풀무원 탱탱쫄면 사 개입">[풀무원] 탱탱쫄면 (4개입)</span>
                  <span class="product__price" aria-label="상품 가격 4980 원">4,980 원</span>
                  <span class="product__summary" aria-label="상품 설명 튀기지 않아 부담없는 매콤함">튀기지 않아 부담없는 매콤함</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">풀무원 탱탱쫄면</figcaption>
                  <img src="../images/product01.png" class="product__img" alt="풀무원 탱탱쫄면 이미지">

                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 온더바디 죠르디 시카 자석 선쿠션">[온더바디] 죠르디 시카 자석 선쿠션</span>
                  <span class="product__price" aria-label="상품 가격 32500 원">32,500 원</span>
                  <span class="product__summary" aria-label="상품 설명 끈적임 없이 보송한 무기자차 선쿠션">끈적임 없이 보송한 무기자차 선쿠션</span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">죠르디 시카 자석 선쿠션</figcaption>
                  <img src="../images/product02.png" class="product__img" alt="죠르디 시카 자석 선쿠션 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="태그">샛별배송</span>
                  <span aria-label="상품 이름 프로쉬 베이비 세탁세">[프로쉬] 베이비 세탁세</span>
                  <span class="discount">
                    <span class="discountRate" aria-label="할인율 24%">24%</span>
                    <span class="discountPrice" aria-label="할인된 가격 18900원">18,900 원</span>
                  </span>
                  <span class="nonDiscount" aria-label="할인전 가격 24900원">24,900 원</span>
                  <span class="product__summary" aria-label="상품 설명 성분을 꼼꼼히 따져 골라 더욱 편안한">성분을 꼼꼼히 따져 골라 더욱 편안한</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">베이비 세탁세</figcaption>
                  <img src="../images/product04.png" class="product__img" alt="베이비 세탁세 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
          </ul>
          <ul class="product__wrap">
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품이름 풀무원 탱탱쫄면 사 개입">[풀무원] 탱탱쫄면 (4개입)</span>
                  <span class="product__price" aria-label="상품 가격 4980 원">4,980 원</span>
                  <span class="product__summary" aria-label="상품 설명 튀기지 않아 부담없는 매콤함">튀기지 않아 부담없는 매콤함</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">풀무원 탱탱쫄면</figcaption>
                  <img src="../images/product01.png" class="product__img" alt="풀무원 탱탱쫄면 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>

            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 온더바디 죠르디 시카 자석 선쿠션">[온더바디] 죠르디 시카 자석 선쿠션</span>
                  <span class="product__price" aria-label="상품 가격 32500 원">32,500 원</span>
                  <span class="product__summary" aria-label="상품 설명 끈적임 없이 보송한 무기자차 선쿠션">끈적임 없이 보송한 무기자차 선쿠션</span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">죠르디 시카 자석 선쿠션</figcaption>
                  <img src="../images/product02.png" class="product__img" alt="죠르디 시카 자석 선쿠션 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 프로쉬 베이비 세탁세">[프로쉬] 베이비 세탁세</span>
                  <span class="discount">
                    <span class="discountRate" aria-label="할인율 24%">24%</span>
                    <span class="discountPrice" aria-label="할인된 가격 18900원">18,900 원</span>
                  </span>
                  <span class="nonDiscount" aria-label="할인전 가격 24900원">24,900 원</span>
                  <span class="product__summary" aria-label="상품 설명 성분을 꼼꼼히 따져 골라 더욱 편안한">성분을 꼼꼼히 따져 골라 더욱 편안한</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">베이비 세탁세</figcaption>
                  <img src="../images/product04.png" class="product__img" alt="베이비 세탁세 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
          </ul>
          <ul class="product__wrap">
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품이름 풀무원 탱탱쫄면 사 개입">[풀무원] 탱탱쫄면 (4개입)</span>
                  <span class="product__price" aria-label="상품 가격 4980 원">4,980 원</span>
                  <span class="product__summary" aria-label="상품 설명 튀기지 않아 부담없는 매콤함">튀기지 않아 부담없는 매콤함</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">풀무원 탱탱쫄면</figcaption>
                  <img src="../images/product01.png" class="product__img" alt="풀무원 탱탱쫄면 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 온더바디 죠르디 시카 자석 선쿠션">[온더바디] 죠르디 시카 자석 선쿠션</span>
                  <span class="product__price" aria-label="상품 가격 32500 원">32,500 원</span>
                  <span class="product__summary" aria-label="상품 설명 끈적임 없이 보송한 무기자차 선쿠션">끈적임 없이 보송한 무기자차 선쿠션</span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">죠르디 시카 자석 선쿠션</figcaption>
                  <img src="../images/product02.png" class="product__img" alt="죠르디 시카 자석 선쿠션 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 프로쉬 베이비 세탁세">[프로쉬] 베이비 세탁세</span>
                  <span class="discount">
                    <span class="discountRate" aria-label="할인율 24%">24%</span>
                    <span class="discountPrice" aria-label="할인된 가격 18900원">18,900 원</span>
                  </span>
                  <span class="nonDiscount" aria-label="할인전 가격 24900원">24,900 원</span>
                  <span class="product__summary" aria-label="상품 설명 성분을 꼼꼼히 따져 골라 더욱 편안한">성분을 꼼꼼히 따져 골라 더욱 편안한</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">베이비 세탁세</figcaption>
                  <img src="../images/product04.png" class="product__img" alt="베이비 세탁세 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
          </ul>
          <ul class="product__wrap">
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품이름 풀무원 탱탱쫄면 사 개입">[풀무원] 탱탱쫄면 (4개입)</span>
                  <span class="product__price" aria-label="상품 가격 4980 원">4,980 원</span>
                  <span class="product__summary" aria-label="상품 설명 튀기지 않아 부담없는 매콤함">튀기지 않아 부담없는 매콤함</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">풀무원 탱탱쫄면</figcaption>
                  <img src="../images/product01.png" class="product__img" alt="풀무원 탱탱쫄면 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 온더바디 죠르디 시카 자석 선쿠션">[온더바디] 죠르디 시카 자석 선쿠션</span>
                  <span class="product__price" aria-label="상품 가격 32500 원">32,500 원</span>
                  <span class="product__summary" aria-label="상품 설명 끈적임 없이 보송한 무기자차 선쿠션">끈적임 없이 보송한 무기자차 선쿠션</span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">죠르디 시카 자석 선쿠션</figcaption>
                  <img src="../images/product02.png" class="product__img" alt="죠르디 시카 자석 선쿠션 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
            <li class="product__list"><a href="/" class="product__link">
                <span class="product__info">
                  <span class="tag" aria-label="상품태그 샛별배송">샛별배송</span>
                  <span aria-label="상품 이름 프로쉬 베이비 세탁세">[프로쉬] 베이비 세탁세</span>
                  <span class="discount">
                    <span class="discountRate" aria-label="할인율 24%">24%</span>
                    <span class="discountPrice" aria-label="할인된 가격 18900원">18,900 원</span>
                  </span>
                  <span class="nonDiscount" aria-label="할인전 가격 24900원">24,900 원</span>
                  <span class="product__summary" aria-label="상품 설명 성분을 꼼꼼히 따져 골라 더욱 편안한">성분을 꼼꼼히 따져 골라 더욱 편안한</span>
                  <span class="product__badge" aria-label="상품 뱃지">
                    <span class="karlyBadge" aria-label="칼리 온리 뱃지">karly Only</span>
                    <span class="textBadge" aria-label="한정수량 뱃지">한정수량</span>
                  </span>
                </span>

                <figure class="imgContainer">
                  <figcaption class="a11y" aria-hidden="true">베이비 세탁세</figcaption>
                  <img src="../images/product04.png" class="product__img" alt="베이비 세탁세 이미지">
                </figure>
                <span class="cartIcon"></span>
              </a></li>
          </ul>
          <div class="movePage">
            <ul class="movePage__wrap">
              <li class="movePage__list"><a href="/" class="movePage__link">
                  <span class="doubleLeft"></span>
                  <span class="a11y">처음 페이지로 가기 버튼</span>
                </a></li>
              <li class="movePage__list"><a href="/" class="movePage__link">
                  <span class="left"></span>
                  <span class="a11y">이전 페이지로 가기 버튼</span>
                </a></li>
              <li class="movePage__list"><a href="/" class="movePage__link">
                  <span class="pageNum">1</span>
                  <span class="a11y">페이지</span>
                </a></li>
              <li class="movePage__list"><a href="/" class="movePage__link">
                  <span class="pageNum">2</span>
                  <span class="a11y">페이지</span>
                </a></li>

              <li class="movePage__list"><a href="/" class="movePage__link">
                  <span class="pageNum">3</span>
                  <span class="a11y">페이지</span>
                </a></li>
              <li class="movePage__list"><a href="/" class="movePage__link">
                  <span class="right"></span>
                  <span class="a11y">다음 페이지로 가기 버튼</span>
                </a></li>
              <li class="movePage__list"><a href="/" class="movePage__link">
                  <span class="doubleRight"></span>
                  <span class="a11y">맨 뒤 페이지로 가기 버튼</span>
                </a></li>
            </ul>
          </div>
        </div>
      </div>

    </div>
  </main>
```

</div>
</details>

<br><br><br><br> 

### SCSS
---
<details>
<summary>ProductList.scss</summary>
<div markdown="1">

```
  @use "../utils" as *;
@use "../components" as *;

.mainContainer {


  @include flexbox($direction: column, $items: center);

  font-family: Pretendard;

  padding: rem(48px) 0 rem(80px) 0;
  gap: rem(48px);
}

.productList__title {
  font-size: rem(21px);
  font-weight: 600;
  line-height: 150%;
}

//제목 외 전체 컨테이너

.productContainer {
  width: 100%;
  @include paddingPct(20);
  @include flexbox($items: flex-start);
}

//사이드바 영역

.sideBar {
  @include flexbox($direction: column);
  flex: 1 0 0;
}

.product {
  @include flexbox($direction: column, $items: flex-start);
}



.brand {
  @include flexbox($direction: column);

  &__list {
    @include flexbox($direction: column, $items: flex-start);

    width: rem(220px);
    padding: rem(12px) 0;

    gap: rem(8px);

    &:hover {
      background: $gray-100;
    }
  }

  &__link {
    display: block;

    width: 100%;
    height: 100%;
    @include flexbox($items: center);

    &::before {
      content: "";
      background: url("../../images/Icon/Check.svg");
      width: rem(24px);
      height: rem(24px);
      margin-right: rem(8px);
    }

    // &::after {
    //   content: "";
    //   font-size: rem(12px);
    //   color: $gray-300;
    //   margin-left: rem(4px);
    // }
  }
}

.grayNum {
  font-size: rem(12px);
  color: $gray-300;
  margin-left: rem(4px);
}

.grayNum__small {
 
  font-size: rem(12px);
  margin-left: rem(8px);
  color: $gray-300;
  
}


.btn__list {
  @include flexbox($justify: center, $items: center);
  // padding: 12px 0px 12px 0px;

  gap: rem(8px);

  width: rem(220px);
  height: rem(42px);
  padding: rem(12px) 0px rem(14px) 0px;

  border-bottom: 1px solid $gray-100;
}



// .sideBar__num {
//   @include flexbox($items: center);
//   gap: rem(8px);

//   &::after {
//     content: "1";
//     font-size: rem(10px);
//     font-weight: 600;
//     line-height: 160%;
//     color: $gray-300;
//   }
// }

// 프로덕트 메뉴바
.menuContainer {
  width: 100%;
  padding: 0px 0px rem(20px) 0px;
  @include flexbox($justify: space-between, $items: center);
}

.bold__main {
  font-weight: bold;
  color: $content;
}

.recommend {
  @include flexbox($items: center);

  &::after {
    content: "";
    display: inline-block;
    background: url("../../images/Icon/question.svg");
    width: rem(14px);
    height: rem(20px);
    margin-left: rem(5px);
  }
}

.menu__wrap {
  @include flexbox($items: center);
  color: $gray-300;
  font-weight: 500;
  gap: rem(4px);
  // flex-grow: 1;
}

//상품
.product {
  &__line {
    @include flexbox($direction: column);
    gap: rem(24px);
  }

  &__list {
    position: relative;
  }

  &__wrap {
    @include flexbox;
    gap: rem(16px);
  }

  &__link {
    @include flexbox($direction: column);
    gap: rem(16px);
  }

  &__info {
    @include flexbox($direction: column);
    gap: rem(8px);
  }

  &__price {
    font-size: rem(21px);
    font-weight: 600;
    line-height: 150%;
  }

  &__badge {
    @include flexbox;
    gap: rem(6px);
  }

  &__summary {
    font-size: rem(12px);
    color: $gray-400;
  }

  &__img {

    width: rem(249px);
    height: rem(320px);

  }
}


//상품 리스트
.imgContainer {
  order: -1;
}

.tag {
  color: $gray-400;
  font-size: rem(12px);
  font-weight: 600;
  line-height: 150%;
}


//할인 상품 내용

.discount {
  @include flexbox;
  gap: rem(8px);
}

.discountRate {
  font-size: rem(21px);

  font-weight: 600;
  line-height: 150%;
  color: $orange;
}

.discountPrice {
  font-size: rem(21px);
  font-weight: 600;
  line-height: 150%;
}

.nonDiscount {
  font-size: rem(12px);
  color: $gray-400;
  text-decoration: line-through;
}


.karlyBadge {
  padding: rem(4px);
  background: $gray-100;
  color: $primary;
  font-size: rem(14px);
  font-weight: bold;
  border-radius: rem(4px);
}

.textBadge {
  padding: rem(4px);
  background: $gray-100;
  color: $content;
  font-size: rem(14px);
  font-weight: bold;
  border-radius: rem(4px);
}



.movePage {
  @include flexbox($direction: column, $items: center);

  &__wrap {
    @include flexbox($items: center);
    padding: rem(48px) 0 0 0;
  }

  &__list {
    position: relative;
    width: rem(34px);
    height: rem(34px);
    border: 1px solid $gray-100;

    &:hover {
      background: $gray-100;
    }
  }

  &__link {
    display: block;
    width: 100%;
    height: 100%;
  }
}
```
</div>
</details>