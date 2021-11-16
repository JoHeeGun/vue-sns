# MAS
  * ## 🗣 프로젝트 소개
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/4fb6b562-893c-42c4-95d3-9f144880c14e/1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211115%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211115T160328Z&X-Amz-Expires=86400&X-Amz-Signature=5eb0c552a43cf7e68b14d199f7c87000a1d22d5461ec092f5881c65e17bddba2&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%221.PNG.png%22)   
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
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/67230a78-c2a9-46a4-b71f-1ee94de1ad58/3.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T075322Z&X-Amz-Expires=86400&X-Amz-Signature=85c695af9a94644c638b9d9234cc4280f809075987d50687a3a83b98662fbbbb&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%223.PNG.png%22)   
  * 로그인페이지 -> 아이디,비밀번호입력 -> 로그인버튼 -> 로그인
  * 우측 상단의 로그인탭 클릭 후 로그인페이지로 이동   
  * 이메일형식으로 아이디작성 (ex: joheegun@gmail.com)   
  * 로그인 성공시 게시글작성 가능   
  * 회원가입버튼 클릭시 회원가입페이지로 이동   
 
 </details> 
 <details><summary>회원가입</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/3bbb4197-9f9d-4c17-a14c-66b5c6c978de/2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T075330Z&X-Amz-Expires=86400&X-Amz-Signature=6e007d0b0e54641622c678a5b9c1ce8ef381915a3765a44c5705738b0b594771&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%222.PNG.png%22)   
  * 회원가입페이지 -> 아이디,비밀번호등 개인정보 입력 -> 회원가입버튼 -> 회원가입완료
  * 상단의 회원가입탭 클릭 후 회원가입페이지로 이동   
  * 이메일형식으로 아이디작성     
  </details>  
 <details><summary>영화 검색</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/46c41540-4aa3-4d82-aed2-ca9b38d28d32/13.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T075634Z&X-Amz-Expires=86400&X-Amz-Signature=ecb31b2075595b3c957ae8b507dc69716873f525cf54f42b17ce1fff7c68f601&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%2213.PNG.png%22)   
   ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/e8b063b5-b5cd-47e0-8fec-c9f99adf6bcd/14.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T075636Z&X-Amz-Expires=86400&X-Amz-Signature=bd9f9b80e6b4360b642a4b3dfd62798d4442ad5c43335f01bfd21ddb90b77d31&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%2214.PNG.png%22)   
  * 상단 영화 검색탭 클릭 후 검색페이지 이동
  * 로그인이 되어 있지 않는 비회원도 이용 가능한 서비스           
  * 원하는 검색조건을 설정하고 Enter Press 
  * 검색조건에 따라 검색결과가 카드 리스트형식으로 나열됨   
  * 개별 아이템 클릭 시 해당 책에대한 정보가 있는 페이지로 이동
  * Vutifiy를 이용한 카드형식
  </details>  
 <details><summary>SNS게시글</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/82306297-a6c5-4e67-a94b-1d345209d627/1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T080448Z&X-Amz-Expires=86400&X-Amz-Signature=e6e25f1e79db115a39be8691ea0bad696824f8121184f7e64931d6c0d1d0ef6a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%221.PNG.png%22)    
   ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/d8b54646-2975-420e-a0e0-d17640ce2911/2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T080504Z&X-Amz-Expires=86400&X-Amz-Signature=e5ae60ff42e6be969985ea9c341e3792dfdbed0f0a9c8a293b9036270da5c5e8&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%222.PNG.png%22)    
  * 카드형식으로 사용자들의 게시글들이 나타남         
  * 로그인이 되어있는 회원만 게시글작성 가능        
  * 내용,이미지 등을 입력하고 업로드 버튼 클릭      
  * 리트윗,좋아요,댓글,삭제 등을 material icon을 사용하여 클릭시 해당 서비스 이용      
  </details>   
        <details><summary>해시태그 검색</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/6de66987-3e5d-4137-bef9-581dff1037ec/3.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T080915Z&X-Amz-Expires=86400&X-Amz-Signature=27b965e3dbcfdde4ec6c096c674541f31e0bfd97827ade7522e092740ceeeaaa&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%223.PNG.png%22)    
   ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/7b5ce960-5893-42c1-a58e-925b7ee0c6b5/4.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T080919Z&X-Amz-Expires=86400&X-Amz-Signature=81e81b62fa70c82297d8223acb5af10680e09b8f2e9cb40c4a852c347d70cec6&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%224.PNG.png%22)    
  * 해시태그 검색창에서 원하는 검색어 입력   
  * 해당 해시태그가 달려있는 게시물 나열(ex #겨울왕국)   
 
  </details>  
  <details><summary>SNS댓글</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/d86f9698-553c-48f0-8878-d31b79993965/7.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T081104Z&X-Amz-Expires=86400&X-Amz-Signature=5ac0a1db0cd85e426ac6f9980cd96f7a137208b0892ba434e3e67ec13e6a76c7&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%227.png%22)       
  * 로그인이 되어있는 상태에만 댓글작성가능   
  * 댓글아이콘 클릭 시 하단에 댓글작성창과 댓글들이 나타남   
 
  </details>   
    <details><summary>SNS리트윗</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/b2ff15b5-eadc-4b0f-85e2-1a601404e12e/1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T083229Z&X-Amz-Expires=86400&X-Amz-Signature=42b37e0336fd45ad31a27395d5cca9c1cf02a4c979b5d06fb8a6cc1e023d2514&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%221.PNG.png%22)    
   ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/60e7a142-aee6-466a-a5af-63194f6f4b8f/2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T083232Z&X-Amz-Expires=86400&X-Amz-Signature=6a5d0d4a5bb8c08fb0662231986ea3e4262b7de18f0e850db5c79e6c517f0f64&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%222.PNG.png%22)    
 * 로그인된 사용자만 이용 가능한 서비스   
 * 리트윗하기위해 게시글의 리트윗 아이콘 클릭   
 * 상단에 리트윗했다는 메세지와함께 해당 게시글 리트윗    
  </details>  
        <details><summary>팔로우 및 팔로잉</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/3bbbf81b-4b0d-4e83-9c61-337ee382d0c7/1.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T084200Z&X-Amz-Expires=86400&X-Amz-Signature=c10c8aef10036b7405803a8c3adc18f08ab9bbf4b4d86ce1675473d78aef0ed7&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%221.PNG.png%22)       
  * 로그인된 사용자만 가능한 서비스    
  * 게시글에있는 버튼으로 팔로우,언팔로우 가능   
  * 팔로우 및 팔로잉된 사용자는 프로필에서 확인가능   
  </details> 
      <details><summary>프로필</summary>
 
  ![예시 이미지](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/e8d7fbd5-edb2-47ef-b708-c755a20e84b2/2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211116%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211116T084514Z&X-Amz-Expires=86400&X-Amz-Signature=3402a7811d4c30412065b645f92dc776fc4df90162ef19e4391acf8c4f6b4651&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%222.PNG.png%22)       
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

