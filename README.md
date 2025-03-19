# kk000254.github.io

**파이썬 개념 정리**

1. 자료형 (Data Types)

정수형 (int)
실수형 (float)
문자열 (str)
불리언 (bool)

예제

print(type(10))      # <class 'int'>
print(type(3.14))    # <class 'float'>
print(type("hello")) # <class 'str'>
print(type(True))    # <class 'bool'>

2. 변수 (Variables)

변수는 데이터를 저장하는 공간으로, 다음과 같은 규칙을 따름
문자 또는 _로 시작해야 함
문자, 숫자, _로 구성됨 (공백, 특수문자 사용 불가)
대소문자 구분함
키워드(예약어) 사용 불가

예제

envelope1 = 10000
envelope2 = 20000
envelope3 = "파이팅"

print(envelope1)  # 10000
print(envelope2)  # 20000
print(envelope3)  # "파이팅"

3. 형 변환 (Type Conversion)

다른 자료형으로 변환할 때 사용
int(): 정수 변환
float(): 실수 변환
str(): 문자열 변환

예제

num = int("5")
print(num)  # 5

num_1 = float("3.5")
print(num_1)  # 3.5

num_3 = str(2)
print(num_3)  # '2'

4. 연산자 (Operators)

산술 연산자: +, -, /, *, % (나머지), // (몫), ** (거듭제곱)
비교 연산자: >, >=, == (같다), != (같지 않다)
논리 연산자: and, or, not
포함 여부 연산자: in, not in

예제

print(5 / 2)   # 2.5
print(5 % 2)   # 1
print(5 // 2)  # 2 (몫)
print(5 ** 2)  # 25 (거듭제곱)

print(5 == 2)  # False
print(5 != 2)  # True

5. 불리언 (Boolean)

참(True) 또는 거짓(False)을 표현하는 값

bool(None): False

문자열: 빈 문자열 False, 값이 있는 문자열 True

숫자: 0은 False, 그 외 숫자는 True

예제

print(3 > 5)         # False
print(bool(None))    # False
print(bool("False")) # True (빈 문자열이 아니므로 True)

6. 주석 (Comments)

코드에 대한 설명을 작성할 때 사용
한 줄 주석: #
여러 줄 주석: ''' 또는 """

예제

# 한 줄 주석
print("신랑 신부 입장")

'''
여러 줄 주석
신랑이 움직이면
신부가 인사하면
'''
print("안녕하세요")

7. 문자열 처리

1) 인덱스와 슬라이싱

lang = "apple"
print(lang[0:5])  # apple
print(lang[:-1])  # appl (마지막 문자 제외)

2) 문자열 결합 및 길이 확인

snack, two = "꿀꽈배기", "2개"
juseyo = snack + two
juseyo += " 주세요"
print(juseyo)  # 꿀꽈배기2개 주세요
print(len(juseyo))  # 문자열 길이 출력

3) 문자열 포맷팅

bread = "빵"
salt = "소금"
print("히바레 {}은 {}이 들어있어서 맛있어".format(bread, salt))
print(f"히바레 {bread}은 {salt}이 들어있어서 맛있어")

4) 문자열 메소드

letter = "how are You?"
print(letter.capitalize())  # 첫 글자만 대문자
print(letter.title())       # 각 단어의 첫 글자만 대문자
print(letter.swapcase())    # 대소문자 서로 변경
print(letter.split())       # 공백 기준으로 문자열 나누기 (리스트 반환)
print(letter.count("how"))  # 'how' 등장 횟수 반환 (대소문자 구분)

8. 문자열 정렬 및 공백 제거

s = "...나도고등학교..."
print(s.strip("."))  # 문자열 앞뒤의 특정 문자 제거 (여기서는 '.')
print(s.strip())  # 공백 제거

이 문서는 계속 업데이트될 예정입니다!
