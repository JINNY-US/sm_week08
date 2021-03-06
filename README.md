# sm_week08
스마트모바일프로그램설계 8주차

7주차 팀 프로젝트 활동 : https://github.com/Kim-KyungJin/sm_week07

### 팀 구성   
스마트정보통신공학과 201621216 이준석   
스마트정보통신공학과 201921036 김경진   
스마트정보통신공학과 201921054 박유리   
스마트정보통신공학과 201921083 이혜정   
스마트정보통신공학과 201921104 홍수빈    
스마트정보통신공학과 201990009 미르자크메더브 사르더르    

   ***   
### 모든 항목은 변경되거나 삭제될 여지가 있습니다   
   ***   
   
### 7주차 보완 (김경진, 홍수빈)   

#### *같이 팀플을 진행하는 홍수빈 학생은 친할아버지 부고로 인하여 이번 주차 활동을 많이 하지 못하였습니다. 이 점 양해해 주시길 바랍니다.*

>진행과정1   
>>랜더링 오류가 자꾸 떠서 앱 자체가 다운받아지지도 않고 실행도 되지 않는 상태입니다.     
>>코드 상으로는 빨간 줄 없는 코드인데 어디서 오류가 나는지 모르겠습니다.    
>>>![image](https://user-images.githubusercontent.com/57963888/115985037-f109a600-a5e4-11eb-904d-f073aff0775c.png)   
>>>![image](https://user-images.githubusercontent.com/57963888/115985053-febf2b80-a5e4-11eb-90d2-5ce34cffde28.png)   

>item_post.xml의 3번째 줄에서   
>com.google.android.material.card.MaterialCardView이   
>문제인 거 같은데 이번 주차에 오류를 고치지 못했습니다.   
>>![image](https://user-images.githubusercontent.com/57963888/115985830-9eca8400-a5e8-11eb-8a25-f7639da0f41a.png)   


>마찬가지로 fragment_post_detail.xml의 45번째 줄에   
>com.google.android.material.button.MaterialButton이 오류를 발생시키는 거 같습니다.      
>>![image](https://user-images.githubusercontent.com/57963888/115985971-287a5180-a5e9-11eb-9ab2-f4fd97e2edc6.png)   
>>Material이랑 관련되면 오류가 나는 거 같습니다.   
>>다음 주차에 왜 오류가 나는지 알아볼 예정입니다.

>진행과정2
>>지금까지 고객 사용자의 입장에서 화면을 구성하고 업주의 입장에서 화면을 구성하지 않아   
>>업주가 사용할 화면을 재구성하였습니다.   
>>>
>>>업주 페이지   
>>>![image](https://user-images.githubusercontent.com/57963888/116077028-f7288100-a6cf-11eb-8292-037cc92fee65.png)   
>>>
>>>광고 문의   
>>>![image](https://user-images.githubusercontent.com/57963888/116076927-d6f8c200-a6cf-11eb-97a3-37d9fcc48211.png)   
>>>
>>>가게 설정하기   
>>>![image](https://user-images.githubusercontent.com/57963888/116080425-03164200-a6d4-11eb-9e95-82313f7794b0.png)   
>>>
>>>데이터베이스와의 연동은 추후에 진행할 예정입니다.   



   ***   
   
### 로그아웃, 비밀번호 찾기 (박유리, 이혜정)   
>진행과정   
> 지난주에 회원 가입과 로그인 기능을 이어서 로그아웃 기능과 비밀번호 찾기 기능을 구현했습니다.
>
>> 1. 로그인 유지
>>
>> 로그인이 유지되지 않아서 앱을 나갔다가 들어오거나 메인화면에서 이전 버튼을 누르면 로그인 화면으로 돌아왔었습니다.
>> 앱 접속마다 로그인해야하는 번거로움을 줄이고자 로그인이 유지될 수 있게 코드를 추가하였습니다.
>> 추가한 코드는 다음과 같습니다.
>>
>>![유저확인](https://user-images.githubusercontent.com/79883808/115999908-d3f6c680-a628-11eb-8531-aadb2533c223.PNG)

>> 2. 로그아웃
>>
>> 로그인 유지로 로그아웃 기능이 필요해져서 추가하였습니다.
>> 다음은 실행영상입니다.
>>
>> [로그아웃](https://user-images.githubusercontent.com/79883808/115999930-f7ba0c80-a628-11eb-8b50-c7bc69275dca.mp4)
>>
>> 앱에 재접속하거나 이전버튼을 눌러도 로그인이 유지되는 것을 볼 수 있습니다. 로그아웃 버튼을 눌러야 로그인화면으로 돌아갈 수 있습니다.

>> 3. 비밀번호찾기
>>
>> 비밀번호를 잊었을 경우 비밀번호 찾기를 눌러 회원가입 했던 이메일을 적어서 이메일이 발송되게 하고 온 이메일을 들어가 비밀번호를 새롭게 다시 만들 수 있게 하는 방식으로 구현하였습니다.
>>
>> [비밀번호 찾기 기능](https://user-images.githubusercontent.com/79883558/115999039-27ffac00-a625-11eb-9337-bf3f47bf1bfd.mp4)
>>
>> 처음 비번이 1234567이었는데 비밀번호찾기를 통해 비번을 123456로 바꾸었습니다.
>> 그 결과 123456로 로그인이 되는 것을 확인할 수 있습니다. 

***   
   
### 구글 지도 띄우기, 장소 검색하기 보완 (이준석, 미르자크메더브 사르더르)   
>진행과정   
>>지도를 휴대폰에서도 띄우기를 성공했으나 검색창을 누르면 튕기는 현상이 발생했습니다.
>>>![KakaoTalk_20210426_212323630](https://user-images.githubusercontent.com/57963888/116082231-217d3d00-a6d6-11eb-92d7-99407fcce0fd.jpg)![KakaoTalk_20210426_212248075](https://user-images.githubusercontent.com/57963888/116082226-20e4a680-a6d6-11eb-9f43-c9c8cf42b0bf.jpg)   
>>>

