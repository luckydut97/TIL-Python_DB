
# 💻파이썬 복습 2022/10/06

### os.getcwd 함수를 이용하여 현재 작업 경로 가져오기
<br>getcwd의 의미는 **Get + Current + Working Directory**, "현재 작업 경로를 얻다"입니다.
<br> 작업 경로(Working Directory)란 내가 실행 중인 파이썬 모듈의 위치를 의미합니다.

```python
import os
#os모듈의 getcwd 함수를 사용하여 현재 작업 경로를 얻고 반환합니다.
def get_current_path(): return os.getcwd() 
c_path = get)current_path()
print('현재 실행중인 모듈의 작업 경로는 %s 입니다.' %c_path)
```


---

* #### 리스트(list)
<br>요소를 삭제하거나 변경할 수 있다. 이러한 특성을 **mutable**(가변성) 이라고 표현한다.  리스트는 append, remove 메소드로 요소들을 추가 및 삭제가 가능하다.
<br>또한, 다른 type의 데이터들을 담을 수 있다. 
<br>*대괄호로 선언*
<br>ex) list_a = [‘a’,1,2]
<br>
* #### 튜플(tuple)
<br>요소를 삭제하거나 변경할 수 없다. 이러한 특성을 **immutable**(불변성)이라고 표현한다.
<br>리스트처럼 append, remove 메소드가 존재하지 않지만, 튜플+튜플로 append, remove기능을 억지로 구현할 수 있긴 하다.
<br>*소괄호로 선언*
<br>
* #### 집합(set)
<br>순서가 없는 중복 불가능한 collection 자료형이다. 인덱싱은 불가하다.
<br>선언 방법 : 중괄호 {}, set 생성자 사용
<br>**자주 쓰이는 상황** : 주로 코딩테스트에서 어떤 값이 선언한 set(집합)에 존재 하는지 하지 않는지 확인한다.
```python
a=set([“a”,”b”,”c”]
print(“d” in a)
> False
```
* #### 딕셔너리(dict)
<br>key를 통해 value를 얻는다. 
<br>선언 방법: 
```Python
a = { 1: ‘hi’ }, a = { ‘a’ : [1,2,3]} 
```
<br>

---

### 딕셔너리 key로 value값 얻기
'''Python
grade = {'pey':10, 'julliet' : 99}
grade['pey']
'''
<br>

### 딕셔너리 만들 때 주의할 사항! 
<br> Key는 고유한 값이므로 중복되는 Key 값을 설정해 놓으면 하나를 제외한 나머지 것들이 모두 무시된다.
<br> Value에 리스트를 쓸 수 있어도, Key에는 리스트를 쓸 순 없다. 

### keys() 함수
'''Python
a={'name':'sangbeom', 'birth':'0912', 'phone':'01071564863'}
print(a.keys())
list(a.keys())
'''
### 키가 딕셔너리 안에 있는지 조사하기(in 활용)
'''Python
'name' in a
'''

---
