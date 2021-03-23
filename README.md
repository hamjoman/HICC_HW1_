# Git이란 무엇인가?

# Git
  
  
  리눅스 기반의 개발 분산형 파일 버전 관리시스템

# 

  # 1) 깃의 목적, 장점

   버전 관리 : 같은 파일에 각기 다른 버전 보관 가능

              ex) 파일에 이브이가 있다
                -> 각각 부스터, 쥬피선더, 샤미드 ver 루트를 만들 것임
                -> 그러나 이브이 단계에서의 수정사항이 생기면 Git 통해 수정할 수 있고 
                -> 각 ver 스토리에 녹아들게 된다
                -> 즉, 동일 파일로 각자의 버전 작업이 가능함
      
#
   백업 : 기록해온 과정이 전부 남음, 내 파일의 변화 기록이 전부 담겨있음 = 히스토리가 담김
#
   협업 : 히스토리 = 열람가능 = 타인과의 공유 가능


              cf. 깃허브: 웹호스팅 관리 사이트
                    ㄴ 협업 시에 깃 히스토리를 push (발행)하여 GitHub 에 올리면 팀원이 그 기록을 확인할 수 있게 된다.
                    ㄴ 상대가 어떻게 했느냐의 깃 히스토리를 공유할 수 있는 것
               
               
   #


# 2) 깃의 개념 이해하고, 저장소 꾸리기


 - 내가 생각하기에 Git이란 "거대한 저장 쳇바퀴" 같다.

                [Directory(실제 파일)] →add(추가)→ [Index (임시 저장소)] →commit(확정)→ [HEAD (최종확정본)] →*push(발행) → [원격저장소 (Github)]
                 ↑ *pull(갱신 과정) └ [branch 생성 (중간 격리 시설 마련)], merge(가지 병합) 등의 작업 ┘
          
    
      * push: 발행, 실제로 작업한 내역물을 원격저장소(Github)에 공유함.
      * pull: 갱신, 원격저장소(Gitbub)에 올라왔던 모든 사항을 내 컴퓨터 저장 공간에 백업해서 진행함.
          
          
         #  
          
          
           - 깃은 한편으로 '기록의 저장소' 이기 때문에,  # ['저장소'를 '지정'] 해주어야 한다.
           - Github와의 연동을 진행할 것이기 때문에, 미리 # [ 온라인 저장소 (원격 저장소) ]를 Github에서 'Repository'로 새로 만들어준다.


                  깃을 설치 후, 어디에 내 모든 파일 제어 기록을 '저장'할 것인지 설정해주어야한다.
                  git init 를 통해 만들라고 하지만, 이는 새로운 로컬저장소를 자동으로 생성해주는 것 같고 (???) 내가 원하는 곳에 넣으려면,
                  C:/ 등에 파일을 하나 만들어서 그걸 'Git Bash here'의 방식으로 열어준다.
                  git clone ~ 생성한 Repository의 링크 입력 ~
                
             * 그럼 이제 내가 새로 생성한 원격저장소와 연동될 수 있는 내 [ 로컬저장소 ]가 생성이 된거다. (Directory 라고 나는 이해하기로 했다.)
          
          
          # 
          
          - # Git Repository # 깃으로 관리하는 저장소이다.
              * local Repository (내 컴), Remote Repository (외부 서버)
              * 둘을 연동시키고 싶으면 수시로 push 해주거나 Remote 설정을 해두면 되는듯?



