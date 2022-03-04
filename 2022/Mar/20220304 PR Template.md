<h1 align="center">
  <br/>
  <img width="300" alt="trevari logo" src="https://user-images.githubusercontent.com/42798132/156313235-d68b21f0-39e3-4f8e-ae86-6c25cb7bea02.png">
  <br/>
  <br/>
Github - PR Template
  <br/>
  <br/>
</h1>

<br/>

### PULL REQUEST TEMPLATE

<hr>

<br/>

#### 1. PR Template 을 적용한 이유
<br/>

PR 은 내가 작성한 코드에 대해 리뷰를 받기 위해 생성한다.  
리뷰어들을 통해 고려하지 못한 부분, 우려되는 부분, 기술적 / 비즈니스적인 부분 들을 다시 검토할 수 있다.


PR 없이 활성화된 branch 에 merge 를 해버리면  
죄를 짓게 된다.. .. 아주 높은 .. 아주아주 높은 확률로.


그러니 PR 은 필수적이다.

<br/>

**하지만**  
PR 을 생성하고 리뷰를 요청했으나  
리뷰 받지 못하는 슬픈 일을 다들 겪어봤을 것이다.  

왜 그럴까 ?   

<br/>

> ' 요청온 PR 이 무슨 기능을 수행하는지 그래서 무엇을 해결하는 건지 잘 모르겠다. '  
>
> ' 어떤 리뷰를 바라는 건지 모르겠다. '  
>
> ' 너무 길어서 읽고 싶지 않다. '  
>
> ' 바쁘다. '  

<br/>

외면 받고 있는 우리의 PR !!!!!  
위와 같은 이유를 들어보니 PR 의 단위가 너무 크거나 그 내용이 부실한 게 문제라는 것을 알게 되었다.  

<br/>

PR 의 단위 (= 작은 단위) 에 대한 URL 을 남겨놓겠다.  
[optimal pull request size](https://smallbusinessprogramming.com/optimal-pull-request-size )  

한 번 읽어보는 것을 추천한다.

</br>

PR 의 단위는 다 같이 얘기하고 실천하는 부분이고.  

</br>

PR 의 내용은 내가. 지금. 한 스텝을. 밟을 수 있겠다. 라고 판단했고,  
Github 에 있는 Repositories 에 PR Template 을 적용했다.  


<br/>
<br/>

<hr>

<br/>


#### 2. PR Template 의 구성은 어떻게 할까?
<br/>

나는 몇 가지를 고려해서 PR Template 을 구성해봤다.    

<br/>
<br/>

> 성격 : Type of change  

우선 PR 의 성격을 통한 분류를
1) 이슈 해결
2) 기능 추가
3) 리팩토링
4) 배포를 위한
5) 긴급

위와 같은 5개의 성격에 체크하는 방식으로
한 눈에 해당 PR 이 가진 성격을 나타낼 수 있게 했다.

<br/>
<br/>

> 문제 : Why ?

가장 중요한 해당 PR 의 존재 이유 !  

이걸 왜 변경했는지.  
뭐 때문에 변경해야만 하는지.  
  
PR 의 목적을 드러낼 수 있도록 해당 항목을 추가했다.  

<br/>
<br/>

> 해결 : Solved

그래서?  
문제를 정의했으니 해결 방법에 대해 얘기해야 한다.  

<br/>

*" a 라는 문제가 있었는데 이 PR 은 그 문제를 b 라는 방법으로 해결했어. "*

<br/>

어떻게 무엇을 해결했는지 적어 놓으면 리뷰어들이 찾아갈 곳을 알게 된다.  

<br/>
<br/>

> 집중 : To Reviewers

뭘 볼지 모르겠다면 봐야되는 부분을 알려주면 된다.  
리뷰어에게 신경 쓰이는 부분이나 부탁하고 싶은 것들에 대해 적을 수 있는 항목을 추가했다.  


<br/>
<br/>
<br/>

<hr>

<br/>
<br/>

작성된 PR Template 은 아래와 같은 구성이다.

<br/>
<br/>

## Type of change
```<!-- PR 의 타입 -->```
- [ ] Fix
- [ ] Feature
- [ ] Refactor
- [ ] Release
- [ ] Hotfix


## Why ?
```<!-- 변경이 필요한 이유 -->```

```<!-- 관련된 링크 -->```
- Fixes # (issue)
- Jira Ticket # (url)
- Other # (url)


## Solved
```<!-- 변경을 통해 해결 되는 것 -->```

- 


## Screenshots (optional)
```<!-- 관련 스크린샷 -->```


## Test Checklist



## To Reviewers
```<!-- 리뷰어에게 전달할 말 -->```

- 

 


