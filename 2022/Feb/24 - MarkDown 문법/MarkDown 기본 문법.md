<br>

개발을 하면서 MarkDown 파일을 작성해야 하는 일이 종종 생기기 마련이다.


Repository 에 있는 README.md 가 대표적인데  
프로젝트 초기 세팅 방법이나 참고 사항들을 적기도 하고,  
Pull Request 를 작성할 때도 MarkDown 형식으로 작성된다.


MarkDown 의 문법을 익히면 다른 사람에게 내 작업 내용을 공유하는데 읽기 좋은 문서를 작성할 수 있다.  
그리고 앞으로 TIL 을 MarkDown 형식으로 작성할 예정이기 때문에  
오늘은 MarkDown 에 대한 기본적인 문법에 대해 알아봤다.

<br><br>

MarkDown 이란?
==============
일반적인 텍스트로 작성하는 경량 마크업 언어로 서식이 있는 문서를 작성하는 데 사용된다.  
다른 마크업 언어에 비해서 쉬운 문법과 간단함이 가장 큰 특징이다.  
확장자는 .md 이며, 인터넷 미디어 타입은 text/markdown 으로  
존 그루버와 에런 스워츠가 사람이 읽고 쓰기 쉬운 플레인 텍스트 포맷을 사용하여 쓸 수 있도록 개발했다.


MarkDown 은 쉽고 간단한 문법과 별도의 도구가 필요 없다는 장점이 존재하지만,  
표준이 존재하지 않고 변환 방식과 생성 결과가 도구에 따라 달라진다는 단점 역시 존재한다.

아래는 MarkDown 의 공식 사이트 url 이다.  
https://daringfireball.net/projects/markdown/

<br><br>

MarkDown 문법
============


## 1. 줄 바꿈 
* 문장 줄 바꿈
   ```
   Space key 두 번
   ```
첫 번째 문장.  
두 번째 문장.

<br>

* 문단 줄 바꿈
   ```
   Enter key 두 번
   ```
첫 번째 문단. 

두 번째 문단.

<br><br>

## 2. 제목
* 큰 제목
    ```
    ===============
    ```
* 중간 제목
    ```
    ---------------
    ```
    큰 제목
    =====
    중간 제목
    -------

<br><br>

## 3. H1 ~ H6
* H1
```
#
```
* H2
```
##
```
* H3
```
###
```
* H4
```
####
```
* H5
```
#####
```
* H6
```
######
```
* H7 부터는 지원하지 않는다.
    # H1
    ## H2
    ### H3
    #### H4
    ##### H5
    ###### H6

<br><br>

## 3. 문체
* 이탈릭체
   ```
  *이탈릭체*
  _이탈릭체_
   ```
    *이탈릭체*  
    _이탈릭체_
    
<br>

* 볼드체
   ```
  **볼드체**
  __볼드체__
   ```
    **볼드체**  
    __볼드체__

<br>

* 취소선
   ```
  ~~취소선~~
   ```
  ~~취소선~~

<br><br>

## 4. 하이퍼링크
```
[링크명](URL)
[링크명](URL "사이트 제목")
```
[구글 링크](http://www.google.com)  
[구글 링크 사이트 제목 있음](http://www.google.com "구글 url")

<br><br>

## 5. 블록 인용
```
> 인용 1
>   > 인용 2
>   >   > 인용 3
```
> 인용 1
>   > 인용 2
>   >   > 인용 3

<br><br>

## 6. 리스트
* 순서가 있는 숫자 리스트
    ```
    1. 리스트
    2. 리스트
    3. 리스트
    ```
    1. 리스트
    2. 리스트
    3. 리스트

<br>

* 숫자를 변경해도 순서가 제대로 부여된다.
    ```
    1. 리스트
    1. 리스트
    3. 리스트
    ```
    1. 리스트
    2. 리스트
    3. 리스트

<br>

* 순서가 없는 리스트
    ```
    - 리스트
    - 리스트
    - 리스트
        - 리스트
            - 리스트
  
    + 리스트
    + 리스트
    + 리스트
        + 리스트
            + 리스트
  
    * 리스트
    * 리스트
    * 리스트
        * 리스트
            * 리스트
    ```
  - 리스트
  - 리스트
  - 리스트
    - 리스트
      - 리스트

  + 리스트
  + 리스트
  + 리스트
    + 리스트
      + 리스트

  * 리스트
  * 리스트
  * 리스트
    * 리스트
      * 리스트
      

<br><br>

## 7. 코드 블록
* Space key 네 번
    ```
    코드 블록이 아닌 문장.
  
        코드 블록 문장.
  
    코드 블록이 아닌 문장.
    ```
코드 블록이 아닌 문장.

    코드 블록 문장.

코드 블록이 아닌 문장.

<br>

* Tap key
    ```
    코드 블록이 아닌 문장.
  
        코드 블록 문장.
  
    코드 블록이 아닌 문장.
    ```
코드 블록이 아닌 문장.

    코드 블록 문장.

코드 블록이 아닌 문장.

<br>

*   ```<pre> <code> {code} </code> </pre>  ```
    ```
    <pre>
    <code>
    public class ExampleCodeBlock {
       public static void main(String[] args) {
          System.out.println("hello world!");
       }
    } 
    </code>
    </pre>
    ```
    <pre>
    <code>
    public class ExampleCodeBlock {
       public static void main(String[] args) {
          System.out.println("hello world!");
       }
    } 
    </code>
    </pre>

<br>

* ( ``` )
    ```
      ```
      public class ExampleCodeBlock { 
         public static void main(String[] args) {
            System.out.println("hello world!");
         }
      }
      ```
    ```
    ```
      public class ExampleCodeBlock { 
         public static void main(String[] args) {
            System.out.println("hello world!");
         }
      }
    ```



<br><br>

## 8. 구분 줄
* ``` <hr> ```
    ```
    * * *
  
    ***
  
    *****
  
    - - -
  
    ---------------------------------------
    ```
  
* * *

***

*****

- - -

---------------------------------------

<br><br>

## 9. 이미지
* 사이즈 조절 기능은 따로 없다.
    ```
     ![Alt 문자열](이미지 URL 혹은 이미지 경로)
     ![Alt 문자열](이미지 URL 혹은 이미지 경로 "이미지 제목")
     ![Alt 이미지 파일임](https://images.megapixl.com/5273/52734504.jpg)
  
     <img src="https://images.megapixl.com/5273/52734504.jpg" width="300px" height="300px" title="px 크기 조절" alt="이미지 파일임"></img>
     <img src="https://images.megapixl.com/5273/52734504.jpg" width="20%" height="20%" title="% 크기 조절" alt="이미지 파일임"></img>
    ```
  ![Alt 이미지 파일임](https://images.megapixl.com/5273/52734504.jpg)
  <img src="https://images.megapixl.com/5273/52734504.jpg" width="300px" height="300px" title="px 크기 조절" alt="이미지 파일임"></img><br>
  <img src="https://images.megapixl.com/5273/52734504.jpg" width="20%" height="20%" title="% 크기 조절" alt="이미지 파일임"></img>

<br><br>
