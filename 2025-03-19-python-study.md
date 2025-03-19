# 2025년 3월 19일 - 파이썬 공부

# 어제까지 배운 내용
# - 자료형
# - 변수
# - 변수 이름
# - 형 변환
# - 연산자
# - 불리언
# - 주석
# - 인덱스와 슬라이싱
# - 문자열 처리
# - 문자열 메시지

# 자료형
print("hello world")

# 변수
# 변수는 문자 또는 `_`로 시작해야 함
# 문자, 숫자, `_`로 구성됨
# 공백, 특수문자 사용 불가
# 대소문자 구분함
# 키워드(예약어) 사용 불가
# 소문자 단어 및 `_`로 구분된 단어 사용 권장

envelope1 = 10000
envelope2 = 20000
envelope3 = "파이팅"

print(envelope1)  # 10000
print(envelope2)  # 20000
print(envelope3)  # "파이팅"

# 연산자
# int(): 정수 변환
# float(): 실수 변환
# str(): 문자열 변환
# 산술 연산자: +, -, /, *, % (나머지), // (몫), ** (거듭제곱)
# 비교 연산자: >, >=, == (같다), != (같지 않다)
# 논리 연산자: and, or, not
# 포함 여부 연산자: in, not in

num = int("5")
print(num)

num_1 = float("3.5")
print(num_1)

num_3 = str(2)
print(num_3)

A = int("5")
B = int("4") 
C = float("3.5") 
D = int("7")
print(A >= B and C <= D)  # True

print(5 == 2)  # False
print(5 != 2)  # True

print(5 / 2)   # 2.5
print(5 % 2)   # 1
print(5 // 2)  # 2 (몫)
print(5 ** 2)  # 25 (거듭제곱)

# 불리언 (bool())
# bool(None): False
# 문자열: 빈 문자열 False, 값이 있는 문자열 True
# 숫자: 0은 False, 그 외 숫자는 True

print(3 > 5)         # False
print(bool(None))    # False
print(bool("False")) # True (빈 문자열이 아니므로 True)

# 주석
# 한 줄 주석: #
# 여러 줄 주석: ''' 또는 """

print("신랑 신부 입장")
'''
신랑이 움직이면
신부가 인사하면
'''
print("안녕하세요")

# 문자열 처리 (슬라이싱)
lang = "apple"
print(lang[0:5])  # apple
print(lang[:-1])  # appl (마지막 문자 제외)

# 문자열 결합 및 길이 확인
snack, two = "꿀꽈배기", "2개"
juseyo = snack + two
juseyo += " 주세요"
print(juseyo)  # 꿀꽈배기2개 주세요

print(len(juseyo))  # 문자열 길이 출력

# 문자열 포맷팅
bread = "빵"
salt = "소금"
print("히바레 {}은 {}이 들어있어서 맛있어".format(bread, salt))
print(f"히바레 {bread}은 {salt}이 들어있어서 맛있어")

# 문자열 이스케이프 문자
print("에일리는 속으로 생각했다\n'나는 노래를 잘 불러'\n 그러나 실제로는 이렇게 말했다\n\"나 노래 못 불러\"")

# 문자열 메소드
letter = "how are You?"
print(letter.capitalize())  # 첫 글자만 대문자
print(letter.title())       # 각 단어의 첫 글자만 대문자
print(letter.swapcase())    # 대소문자 서로 변경
print(letter.split())       # 공백 기준으로 문자열 나누기 (리스트 반환)
print(letter.count("how"))  # 'how' 등장 횟수 반환 (대소문자 구분)

s = "나도고등학교"
print(s.startswith("나도"))   # '나도'로 시작하는지 (True/False)
print(s.endswith("나도"))     # '나도'로 끝나는지 (True/False)
print(s.replace("고등학교", "고교"))  # 특정 단어 치환
print(s.find("학교"))  # '학교'가 처음 등장하는 위치 (없으면 -1 반환)
print(s.find("대학교"))  # 찾는 단어가 없으면 -1 반환

# 문자열 정렬 및 공백 제거
s = "...나도고등학교..."
print(s.strip("."))  # 문자열 앞뒤의 특정 문자 제거 (여기서는 '.')
print(s.strip())  # 공백 제거

