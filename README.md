당연히 알아야할 알고리즘 (C언어로 구현 )
----------
<1> Dynamic Programming


1. dynamic programming 이해
    쉽게 말해서 효율적인 완전탐색 기법.
    계산할때마다 적어놓고 같은 문제가 나오면 갖다쓰자! DP의 기본원리


    방법의 구체화 → 과거의 해를 memory 테이블( 1차원 배열 or 2차원 배열)로 만들어서 저장하며 탐색을 한다. 그러면 반복되는 같은 과정의 계산을 하지 않아도 되기 때문에 효율적이다.


2. 대표적 예제 세가지 fibonacci, LCS , 배낭 -> 풀고 위에 코드와 비교해보면 좋습니다.


1 ) fibonacci------------------------------------------------------------------------------------------
https://makefortune2.tistory.com/60

    코드 구현은 위에 코드파일로 있습니다.
    
        
2 ) LCS-----------------------------------------------------------------------------------------------


https://hsp1116.tistory.com/37

    코드 구현은 위에 코드파일로 있습니다.
3 ) 배낭-----------------------------------------------------------------------------------------------
    
    ex) 배낭문제의 핵심 아이디어.
1. i 번째 이하 번호의 물건을 넣을 수 있을때 i 번째 물건이 못 들어가면 그 전 물건들로 구성한 값들 중 최댓값 → m
2. i 번째 이하 번호의 물건을 넣을 수 있을때 i 번째 물건이 들어갈 수 있따면 이제 i 번째를 고려할 수 있는 거니까
    1. i 번째 물건을 먼저 넣어 놓고(w-wi) i-1 개이하로 넣을 수 있을때 최댓값
    2. i 번째 믈건을 넣지 않고 i-1 번째 까지의 물건들로 w 를 맞췄을때의 최댓값
    둘 중 큰 값 → m
        코드 ->위에 코드파일로 있습니다.
    
----------
<2> Greedy Algorithms

이건 여러분의 두뇌를 믿으셔야 합니다.

<3> Graph Algorithms
1. 간선과 점으로 이루어진 데이터 structure를 이용하여 문제를 해결하는 알고리즘.
그래프를 다루는 기법 ( Search ) 예제 BFS, DFS

1 ) BFS ( Breadth-First Search )

    https://gmlwjd9405.github.io/2018/08/15/algorithm-bfs.html
    방문했다는 print표시할때는 큐에 넣을때 하거나 뺄때하거나 둘중 하나 하면 된다.
    
2 ) DFS (Depth _ First Search)

    https://gmlwjd9405.github.io/2018/08/14/algorithm-dfs.html
    작은 인덱스 찾아갈때 마다 방문했다는 프린트를 하면 방문 표시 가능.
    
    BFS DFS 코드-> 위에 코드파일에 합쳐서있습니다.
    
 
----------
<4> Spanning Trees

https://gmlwjd9405.github.io/2018/08/28/algorithm-mst.html

1. Spanning Tree 의 이해
    - Spanning Tree는 그래프의 최소 연결 부분 그래프 이다. 즉 n개의 정점이 있다면 n-1개의 간선으로 연결한 그래프.
    - 따라서 싸이클이 없는 특징이 있다.
    - 그 중 MST 가 의미있다.  Minimum Spanning Tree = 최소 신장 트리
        - 가중치의 합이 최소가 되는 spanning tree 라서 최적화의 의미가 있는 트리.


    Spanning tree 만들기는 BFS, DFS 로 만들 수 있고
    MST는 Kruskal 알고리즘, Prim 알고리즘으로 만들 수 있다.


2. Kruskal 알고리즘, Prim 알고리즘
    1 ) Kruskal 알고리즘
    
    2 ) Prim 알고리즘


----------
<5> Shortest Path
1. 벨만포드 알고리즘
2. 다익스트라 알고리즘

----------
<6> Sorting Algorithm (basic)

![](https://paper-attachments.dropbox.com/s_045BE8BDF599E13279771AF585282B064EA037480C46167C43B1CC52F61C91A5_1565881167980_.PNG)

                        막 Sorting →아주 비효율적
                        goto → 속도저하 → 최대한 쓰지 않도록
![](https://paper-attachments.dropbox.com/s_045BE8BDF599E13279771AF585282B064EA037480C46167C43B1CC52F61C91A5_1565883299539_.PNG)

                Bubble Sorting → 좀 더 효율적


![](https://paper-attachments.dropbox.com/s_045BE8BDF599E13279771AF585282B064EA037480C46167C43B1CC52F61C91A5_1565945189459_dfdfdfdfdf.PNG)


Quick Sorting → 더 더 효율적
qsort(요소들에 접근할 이름 or 주소 , 요소개수 , 요소크기 , compare)






