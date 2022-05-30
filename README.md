# chatting app

## 개요
2020.05.30 ~  
1대 1 채팅 앱
- client: Android  
- Server: Firebase


<br>


## 오류 수정 사항
1. <b>SPAN_EXCLUSIVE_EXCLUSIVE</b>  
[activity_sign_up.xml](https://github.com/HS0204/chat-app/blob/main/app/src/main/res/layout/activity_sign_up.xml#L36) EditText 뷰 객체 SPAN_EXCLUSIVE_EXCLUSIVE 오류   
[stackoverflow](https://stackoverflow.com/questions/13670374/android-span-exclusive-exclusive-spans-cannot-have-a-zero-length) 참고 xml에 textNoSuggestions 추가하여 해결

2. <b>Null Object Reference</b>  
[MessageAdapter.kt](https://github.com/HS0204/chat-app/blob/main/app/src/main/java/hs/project/chattingapp/MessageAdapter.kt#L39) 39번째 줄에서, receive 데이터가 없는, 즉 초기화되지 않은 경우 널 오류 발생  
? 연산자로 해결


<br>


## 개선사항
### 로그인
- [ ] 비밀번호 6자리 이상 알리기
- [ ] 올바르지 않은 이메일 형식
- [ ] 중복된 이메일 체크

### 채팅
- [ ] 아무것도 입력하지 않았을 때 보내기 않기
- [ ] 채팅 내용 삭제
- [ ] 대화 상대 삭제

### UI
- [ ] 액션바 컬러 수정