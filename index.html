
<!DOCTYPE html>
<html lang="ko">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>성회 지연 결혼식에 초대합니다</title>
    <link href="https://hangeul.pstatic.net/hangeul_static/css/NanumBarunGothicYetHangul.css" rel="stylesheet">
    <style>
        @import url('https://hangeul.pstatic.net/hangeul_static/css/nanum-square.css');
            #welcome {
            font-family: 'NanumBarunGothicYetHangul';
            }
            #every-guests {
            font-family: 'NanumBarunGothicYetHangul';
            }
            #selecttitle {
            font-family: 'NanumBarunGothicYetHangul';
            }
            #selectbnb {
            font-family: 'NanumBarunGothicYetHangul';
                height: 30px;
                border-top: none;
                border-left: none;
                border-right: none;
                border-bottom: 3px solid black;
            }
            #radiobnb {
            font-family: 'NanumBarunGothicYetHangul';
                height: 30px;
                border-top: none;
                border-left: none;
                border-right: none;
            }
            html {
            /* 수평 중앙 정렬하기 */
            text-align: center;
            }

            #guest-name {
                font-family: 'NanumSquareBold';
                width: 120px;
                height: 30px;
                border-top: none;
                border-left: none;
                border-right: none;
                border-bottom: 3px solid black;
            }
            #guest-number {
                font-family: 'NanumSquareBold';
                width: 30px;
                height: 30px;
                border-top: none;
                border-left: none;
                border-right: none;
                border-bottom: 3px solid black;
            }
            #guest-submit {
                font-family: 'NanumSquareAceb';
                width: 40px;
                height: 35px;
                border-top: none;
                border-left: none;
                border-right: none;
                border-bottom: 3px solid black;
            }
    </style>
  </head>
  <body>
    <h4 id="welcome">참석하시는 모든 분들👫께서는<br>성함을 작성해 주시기 바랍니다🎈</h4>
    <!--<h5 id="every-guests">*오시는 모든 분들 한 분 씩 작성 부탁드립니다*</h5>-->

    <form>
      <!-- 방명록 작성자명 입력란 -->
      <span id="selecttitle" style="font-size:14px">신랑🤵 또는 신부👰 측 선택</span>
      <!-- <select name="신랑 측" id="selectbnb">
        <option name="checkbnb" value="broom">신랑 측</option>
        <option name="checkbnb" value="bride">신부 측</option>
      </select> -->
    <span id="radiobnb" style="font-size:14px">
      <input type='radio' name='bnbs' value='broom' />신랑
      <input type='radio' name='bnbs' value='bride' />신부
    </span>
      <br>
      <br>
      <span id="selecttitle" style="font-size:14px">성함</span>
      <input type="text" id="guest-name" placeholder="성함을 입력해주세요" /> <br>
      <!-- 방명록 전송 버튼 -->
      <span id="selecttitle" style="font-size:14px">본인 포함 참석 수</span>
      <input type="number" id="guest-number" value="1" /> <br><br>
      <button type="button" id="guest-submit">작성</button>
    </form>

    <script type="module">
      import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-app.js";
      import { getAnalytics } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-analytics.js";
      import {
        query,
        orderBy,
        getFirestore,
        collection,
        getDocs,
        addDoc,
      } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore.js";
      const firebaseConfig = {
        apiKey: "AIzaSyARqvdnWaApt4SPvEdanjePpz018bB9rBQ",
        authDomain: "shjy-wedding.firebaseapp.com",
        projectId: "shjy-wedding",
        storageBucket: "shjy-wedding.firebasestorage.app",
        messagingSenderId: "392737311336",
        appId: "1:392737311336:web:159db86cb0436f6aaf89dd",
        measurementId: "G-KYDM9YX46C"
        };

      const app = initializeApp(firebaseConfig);
      const analytics = getAnalytics(app);

      const db = getFirestore(app); // Firestore 실행
      const testRef = collection(db, "test"); // 'guests' 컬렉션 불러오기
      const q = query(testRef, orderBy("created_at", "desc")); // 불러온 방명록 전체 목록을 최신순(작성일시 내림차순)으로 정렬

      // 방명록 작성 기능
      async function sendGuest() {
        // 사용자가 입력한 데이터 받아오기
       // const bnb = await document.querySelector("#select").value;
       //const bnb = document.getElementById("selectbnb");
       //const value = (bnb.option[bnb.selectedIndex].value);
        const name = await document.querySelector("#guest-name").value;
        const number = await document.querySelector("#guest-number").value;
        // const content = await document.querySelector("#guest-content").value;

      var bnb = document.getElementsByName('bnbs');
      var bnbChoice = 'broom'; // 여기에 선택된 radio 버튼의 값이 담기게 된다.
        for(var i=0; i<bnb.length; i++) {
            if(bnb[i].checked) {
                bnbChoice = bnb[i].value;
            }
        }
        alert(name + " 님 작성 되었습니다. 감사합니다. 💕");
        // Firestore에 데이터 전송
        await addDoc(testRef, {
          name: name,
          bnb: bnbChoice,
          number: number,
          created_at: new Date(),
        });

        // 입력란 초기화
        document.querySelector("#guest-name").value = "";
        document.querySelector("#select").value = "";
        document.querySelector("#number").value = "";
        //document.querySelector("#guest-content").value = "";

      }

      // 방명록 전체 목록 표시 기능
      async function getGuestList() {
        // 방명록 전체 목록의 HTML 코드
        let html = `<ul>`;

        // Firestore에서 최신순으로 정렬된 목록 받아오기
        const guestList = await getDocs(q);

        // 화면에 출력
        guestList.forEach((data) => {
          // 날짜 형식 변환
          const date = new Date(data.data().created_at.toDate());
          const myDate = `${date.getFullYear()}년 ${
            date.getMonth() + 1
          }월 ${date.getDate()}일 ${date.getHours()}:${date.getMinutes()}`;

          // 개별 방명록의 HTML 코드를 전체 목록 HTML 코드에 추가
          html += `
            <li>
              <p class="guest-list-name">참석자 이름: ${data.data().name}</p>
              <p class="guest-list-created-at">작성일: ${myDate}</p>
            </li>
          `;
        });

        html += `</ul>`;

        // 방명록 전체 목록을 실제로 화면에 표시
        document.querySelector("#guest-list").innerHTML = html;
      }

      // '작성' 버튼에 위 함수 연결
      document.querySelector("#guest-submit").addEventListener("click", () => {
        sendGuest();
        getGuestList();
      });

      // 방명록 화면 첫 진입 시 전체 목록 화면에 표시
      getGuestList();
    </script>
  </body>
</html>
