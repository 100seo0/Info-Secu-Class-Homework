#### 퀵 정렬(quick sort)

시간 복잡도: O(n log n)

worst case: 0(n^2)

space complexity: O(n)

피봇을 하나 정하고 피봇보다 작은 아이템은 왼쪽, 큰 아이템은 오른쪽에 놓는 방식

왼쪽, 오른쪽에 정렬된 아이템들을 퀵정렬함



#### 큐(Queue)

FIFO(first in first out)

euqueue 데이터를 입력하는 함수

dequeue 데이터를 출력하는 함수

printer job queue, BFS(Breadth First Search)



#### 스택(stack)

push: 스택에 답는 과정

스택이 가득 찼을때 오류를 야기 할 수 있음: stack over flow

pop: 스택에 있는 아이템을 빼내는 과정 LIFO

스택에 아무런 아이템이 없는데 아이템을 뺄려 하는 과정: stack under flow

Browser back button, DFS(Depth First Search)



#### 링크드리스트(Linked list)

node들이 link된 data structure

node의 next는 다음 node를 가리킴

출력할 때는 처음부터 데이터를 순회(current가 null이 될 때까지)

삭제하는 과정은 head를 지우는 방법과 중간에 있는 아이템을 지울 때 과정이 다르다.

head를 지울때는 head를 다음으로 넘겨주고 중간에 있는 아이템을 그 전 node가 가리키는 node를 다음 node로 연결시켜주고 삭제(free)해준다

reverse를 하고 싶을 때는 prev(이전 노드를 가리키는 변수)



#### 힙 정렬 알고리즘(Heap Sort) part 1/2

시간 복잡도

- Runtime: worst-case o(n log n)
- for get root value(max, min value): O(1) [1개의 값을 구할 때]

힙은 max heap과 min heap이 있음

parrent가 child보다 크면 heap(max heap 기준)

heapify: 일반적인 tree를 heap tree로 바꾸는 과정

siftdown: parrent가 child보다 작으면 스와핑해주는 과정을 반복하는 과정

온라인 쇼핑몰에서 최저가 물품 제품을 알려줄 때[O(1)]



#### 힙 정렬 알고리즘(Heap Sort) part 2/2

heap tree를 sort하는 과정

- root node를 마지막 node와 스와핑
- 마지막 node를 siftdown하는 과정을 반복



#### 이진트리 알고리즘 Binary Search Tree[BST] part 1/2

Search, Delete, Insert: O(log n)

현재있는 node보다 작은 값은 왼쪽에, 큰 값은 오른쪽에

tree는 node들의 구성체

node는 3개의 member를 가지고 있음(value, left, right)

삭제과정은 세가지로 나뉨

- 삭제하려는 node에 child node가 없는 경우
- 삭제하려는 node가 child node가 하나 있는 경우
- 삭제하려는 node의 child node가 양쪽에 있는 경우
  - 오른쪽에 있는 서브트리에서 가장 왼쪽에 있는 node를 root node로



#### 이진트리 알고리즘 Binary Search Tree[BST] part 1/2

- pre order traverse(한 서버에서 트리의 구조를 그대로 다른 곳에 보내고 싶을 때 사용)
  1. visit the root
  2. traverse the left subtree
  3. traverse the right subtree

- in ordr traveerse(정렬이 됨)
  1. visit  left
  2. visit parent
  3. visit right
- post order traverse
  1. visit left
  2. visit right
  3. visit root



#### 그래프 기본 개념 정리

vertex와 edge가 있을 때 그래프라고 부름

edge가 방향성이 있을 때는 direct graph

edge가 방향성이 없을 때는 undirect graph

edge가 value가 있을 떄 weighted graph

adjacency list는 공간복잡도가 낮음

adjacency matrix는 edge가 있는지 없는지 단 한 번의 검색으로 알 수 있으나, 공간 복잡도가 큼



#### 깊이우선탐색(DFS, Depth First Search)

각각의 인접 node에 접근하여 스택을 이용함

접근할 인접 node가 없을 경우 스택을 팝하여 그 전 접근한 node의 인접 node를 스택에 저장하는 일을 반복함



#### 그래프의 사이클 찾기(DFS, find cycle in undirect graph)

스택에 push, pop하는 과정을 통하여 visited를 보면 중복된 값이 있다는 것을 확인할 수 있음.

사이클이 있다는 것을 증명 가능