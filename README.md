# MAS
  * ## 🗣 프로젝트 소개
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/4fb6b562-893c-42c4-95d3-9f144880c14e/1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T064725Z&X-Amz-Expires=86400&X-Amz-Signature=778db0f6bcdcdeaf2c91f3fddbd4d87b86e917923fceaa0bd8f18ca8b2d018f6&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%221.PNG.png%22&x-id=GetObject)   
MAS는 Movie & SNS의 줄임말로 영화를 좋아하는 사용자들이 영화를 주제로 자유롭게 이야기를 나누는 SNS사이트입니다.   
평소 영화를 좋아하고 관련 커뮤니티는 많지만 SNS형태의 영화서비스를 제공하는 사이트는 없었기 때문에 프로젝트를 기획하게 되었습니다.   
영화 API를 활용해 영화의 상세한 정보들을 쉽게 얻을 수 있습니다.      
게시글을 올리고 댓글을 작성하는 등의 활동을 통해 정보를 공유하며 리트윗,팔로우등 SNS의 기능들을 구현하였습니다.   


* ## 🛠 기술스택 & 개발환경
Frontend : Javascript / HTML5 / CSS3 / sass,scss / Vue.js / Vuetify / Nuxt.js        
Backend : Node.js / Express    
Database : MySQL      
Tools : vscode   
useAPI : OMDBAPI

* ## 🤚 Team & Part  
1인 프로젝트(개인)      
웹 프론트엔드 전체 디자인 및 개발   

 



* ## 🕹 주요기능
 
 <details><summary>로그인</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/67230a78-c2a9-46a4-b71f-1ee94de1ad58/3.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T064754Z&X-Amz-Expires=86400&X-Amz-Signature=28d2e316bddf4297d563f6c14ae4795eed85b29e6937bd1ac7c5137b0360395a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%223.PNG.png%22&x-id=GetObject)   
  * 로그인페이지 -> 아이디,비밀번호입력 -> 로그인버튼 -> 로그인
  * 우측 상단의 로그인탭 클릭 후 로그인페이지로 이동   
  * 이메일형식으로 아이디작성 (ex: joheegun@gmail.com)   
  * 로그인 성공시 게시글작성 가능   
  * 회원가입버튼 클릭시 회원가입페이지로 이동   
 
 </details> 
 <details><summary>회원가입</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/3bbb4197-9f9d-4c17-a14c-66b5c6c978de/2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T064807Z&X-Amz-Expires=86400&X-Amz-Signature=665a243bf3bebe85a621b8ff527f685c1de66333ba474a99c3457a936160a12e&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%222.PNG.png%22&x-id=GetObject)   
  * 회원가입페이지 -> 아이디,비밀번호등 개인정보 입력 -> 회원가입버튼 -> 회원가입완료
  * 상단의 회원가입탭 클릭 후 회원가입페이지로 이동   
  * 이메일형식으로 아이디작성     
  </details>  
 <details><summary>영화 검색</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/46c41540-4aa3-4d82-aed2-ca9b38d28d32/13.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T064823Z&X-Amz-Expires=86400&X-Amz-Signature=029801e880fda3f46e3af8e279a7e76503e103af07e3425b05d1bbf6a64c07e1&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%2213.PNG.png%22&x-id=GetObject)   
   ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/e8b063b5-b5cd-47e0-8fec-c9f99adf6bcd/14.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T064833Z&X-Amz-Expires=86400&X-Amz-Signature=635ec9fe708acd62d551bc5117d0245a80907ad1d02f0f94cb32e7e0ade9fca3&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%2214.PNG.png%22&x-id=GetObject)   
  * 상단 영화 검색탭 클릭 후 검색페이지 이동
  * 로그인이 되어 있지 않는 비회원도 이용 가능한 서비스           
  * 원하는 검색조건을 설정하고 Enter Press 
  * 검색조건에 따라 검색결과가 카드 리스트형식으로 나열됨   
  * 개별 아이템 클릭 시 해당 책에대한 정보가 있는 페이지로 이동
  * Vutifiy를 이용한 카드형식
  </details>  
 <details><summary>SNS게시글</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/db92e8b0-cd01-4bbb-a550-dd7ef2dd107f/4.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T064935Z&X-Amz-Expires=86400&X-Amz-Signature=6329703139218802f951ab78e61272c01426b6c90abcd408dca56525d1728312&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%224.PNG.png%22&x-id=GetObject)    
   ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/f2fc2a1e-a643-44b6-a43a-7e6b55347c96/1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T065000Z&X-Amz-Expires=86400&X-Amz-Signature=d76112a5b00ee217cfd12d844b1630ac1c5c2896aa6493d5619b9dd45fb943ad&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%221.PNG.png%22&x-id=GetObject)    
  * 카드형식으로 사용자들의 게시글들이 나타남         
  * 로그인이 되어있는 회원만 게시글작성 가능        
  * 내용,이미지 등을 입력하고 업로드 버튼 클릭      
  * 리트윗,좋아요,댓글,삭제 등을 material icon을 사용하여 클릭시 해당 서비스 이용      
  </details>   
        <details><summary>해시태그 검색</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/e92f3107-fc04-4c6f-8655-19686f932cc9/11.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T065017Z&X-Amz-Expires=86400&X-Amz-Signature=191dfbf240c1b69fac36fd03c86670f7dbc705c76e8e53301207631577b7d50a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%2211.png%22&x-id=GetObject)    
   
  * 해시태그 검색창에서 원하는 검색어 입력   
  * 해당 해시태그가 달려있는 게시물 나열(ex #겨울왕국)   
 
  </details>  
  <details><summary>SNS댓글</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/d86f9698-553c-48f0-8878-d31b79993965/7.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T065047Z&X-Amz-Expires=86400&X-Amz-Signature=45cc3a3a454a668f9477abe96dcac54d87fe12e80a74e2341e944e832db6b399&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%227.png%22&x-id=GetObject)       
  * 로그인이 되어있는 상태에만 댓글작성가능   
  * 댓글아이콘 클릭 시 하단에 댓글작성창과 댓글들이 나타남   
 
  </details>   
    <details><summary>SNS리트윗</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/c826f6f3-e44f-40d5-8de4-1d159b67b23d/8.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T065112Z&X-Amz-Expires=86400&X-Amz-Signature=be7e7dd259ac72304b2045931f8c3e25ee764082ee802d89f4da8630aa1b2c92&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%228.PNG.png%22&x-id=GetObject)    
 * 로그인된 사용자만 이용 가능한 서비스   
 * 리트윗하기위해 게시글의 리트윗 아이콘 클릭   
 * 상단에 리트윗했다는 메세지와함께 해당 게시글 리트윗    
  </details>  
        <details><summary>팔로우 및 팔로잉</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/f47a41b1-8849-479f-824d-8a371420de50/1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T065324Z&X-Amz-Expires=86400&X-Amz-Signature=d12762864e918136b9f6ac89a14b97f8ef667029b1196e186abd7fe30b889844&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%221.PNG.png%22&x-id=GetObject)       
  * 로그인된 사용자만 가능한 서비스    
  * 게시글에있는 버튼으로 팔로우,언팔로우 가능   
  * 팔로우 및 팔로잉된 사용자는 프로필에서 확인가능   
  </details> 
      <details><summary>프로필</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/1755aeec-b4a3-438b-bf68-897f278591fd/12.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211203%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211203T065149Z&X-Amz-Expires=86400&X-Amz-Signature=fec3cdf110db77aa1d470d666651484336c9b142224da23823899c5736fa0ddf&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%2212.PNG.png%22&x-id=GetObject)       
  * 로그인시 상단에 프로필탭이 나타남   
  * 자신의 팔로잉 및 팔로워 수, 게시글수를 볼 수 있음   
  * 자신의 닉네임을 변경할 수 있음   
  * 팔로잉 및 팔로워 리스트에서 사용자클릭시 해당사용자의 게시글을 모아 볼 수 있음   
  </details>  
 
   
 
* ## 📕 성과 
Nuxt.js를 활용하여 SSR의 개념을 배우고 검색엔진최적화를 진행해 볼 수 있었음        
Nuxt.js로 프로젝트를 설정하여 초기프로젝트 설정 비용감소와 생산성향상을 느낄 수 있었음           
규격화된 폴더구조로 개발하여 프로젝트관리 및 클린코드작성에 유의하며 개발 할 수 있었음       
실제 백엔드 API를 사용하여 구현하여 생산성 높은 프로젝트 환경 구축과 백엔드와의 통신하는 방법에 대하여 익힘         
Promise,Async/Await과 같은 비동기 처리 개념을 익힐 수 있었음       
Vuetify를 활용해 봄으로써 구글의 공식디자인을 활용해 볼 수 있었음      



* ## 📎 Link   
* Notion (https://www.notion.so/MBP-My-Book-Post-969e18f073ef4fe39d39b2ed0f635c17)   
* 웹구동 영상 (https://www.youtube.com/watch?v=uQr1mThCS3c)

