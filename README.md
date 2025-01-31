# 25.01.22-01.31

## 2025.01.22 TIL
%와 /로 행렬화하여 배치
arr = arr.OrderBy(x => Random.Range(0f, 7f)).ToArray(); 를 통해 배열을 랜덤하게 섞어 그림의 위치를 랜덤으로 만듦  
project setting의 메뉴를 통해 splash image로 회사 로고 보여주기  
Audio Source를 통해 효과음 및 BGM 추가하기  

## 2025.01.27
메서드 = 클래스 함수  
재귀 호출의 경우 복잡한 식을 단순하게 만들어 줄 수 있지만 종료시점을 명확히 잡지 못하면 무한 루프에 빠질 우려가 있으니 유의하여 사용해야 함  
###틱택토
보드의 각 칸에 플레이어가 보고 선택할 수 있도록 숫자를 적어 넣을 때 선택한 곳은 각 플레이어의 마크로 숫자를 대체할 수 있도록  
숫자를 직접 적는 것이 아닌 배열의 구성요소를 끌어다 놓고 마크할 때 해당 배열 구성요소를 플레이어의 마크로 변경  
변경하기 전에 해당 칸이 두 플레이어의 문양 중 하나라도 같은 것이 있는지 판독  
플레이어가 한 번 마크할 때마다 승패가 결정났는지 여부 판독 위해 각 가로줄, 세로줄, 대각선줄에 대하여 두 개씩 묶어 같은 모양인지 비교함( ex. 가로 맨 윗줄의 경우 if (arr[1] == arr[2] && arr[2] == arr[3]) )  
만약 모든 칸에 처음에 적혀 있던 숫자가 아닌 다른 것이 적혀 있고 승패가 결정나지 않았을 경우 무승부로 판정시키도록 함

##2025.01.31
자료형은 값 타입과 참조 타입으로 나뉘어지고 타입에 따라서 스택/힙 메모리를 사용한다
