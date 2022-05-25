import os      # os 의 기능을 갖다 사용하겠음
import time    # time 의 기능을 갖다 사용하겠음

# os.system("cls")   화면지워주는 표현
# time.sleep(x)      x 초간 화면을 멈춤

st = "안녕하세요~ 자판기 프로그램입니다. 삐리리리" 

for i in st:
    print(i, end="")
    time.sleep(0.1)

input("\n\n\n[ENTER] 시작하기")
os.system("cls")





money = 0

errcnt = 0
while True:
    # 메뉴출력
    print("="*30)
    print("1. 콜라 / 300")
    print("2. 사이다 / 300")
    print("3. 커피 / 200")
    print("4. 돈 넣기")
    print("5. 잔돈반환")
    print("6. 종 료")
    print("="*30)
    print(f"현재금액 {money}")

    # 선택받기
    menu = input("MENU CHOICE > ")
    
    # 처리
    if menu == "1":
        errcnt = 0
        if money >= 300:
            print("콜맛!!")
            money -= 300
        else:
            print("금액이 부족합니다.")
    
    elif menu == "2":
        errcnt = 0
        if money >= 300:
            print("사맛!!")
            money -= 300
        else:
            print("금액이 부족합니다.")
    
    elif menu == "3":
        errcnt = 0
        if money >= 200:
            print("사맛!!")
            money -= 200
        else:
            print("금액이 부족합니다.")

    elif menu == "4":
        errcnt = 0
        m = input("돈을 넣어주세요 : ")
        if m.isnumeric():
            m = int(m)
            money += m
        else:
            print("입력이 옳지 않습니다!!")

    elif menu == "5":
        errcnt = 0
        if money:
            print(f"{money} 원이 반환됩니다!")
            money = 0
        else:
            print("줄 돈이 없어요")
        
    elif menu == "6":
        if money:
            print(f"{money} 원 내가먹는다?!")
            money = 0
        print("서운해 :(")
        break

    else:
        errcnt += 1
        if errcnt == 3:
            print("혼나!!")
            break
        print("입력 오류!!")

    time.sleep(0.7)
    os.system("cls")
