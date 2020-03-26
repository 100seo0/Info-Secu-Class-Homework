

#### 빅오 표기법(Big-O notation, Time Complexity), 시간복잡도, 공간복잡도 (Big O Notation)

$$
O(1) < O(logn) < O(n) < O(n log n) < O(n^2)
$$

1. O(1)

   Push, Pop on stack

   Access hash table (하나의 키에만 접근)

2. O(log n)

   Binary Search Tree Access, Search, Insertion, Deletion

3. O(n)

   traverse tree, traverse linked list

   아이템의 개수만큼 접근

4. O(n log n)

   Quick Sort, Merge Sort Heap sort

5. O(n^2)

   Insertion Sort, Bubble Sort, Selection sort



#### 거품 정렬(bubble sort)

시간 복잡도: O(n^2)

space  complexity: O(1)

인접한 두 개의 자료를 비교해서 차순에 맞게 교환하는 작업을 정렬이 완료될 까지 반복하는 것

자료수 -1 만큼 루핑하여 스와핑



#### 선택 정렬(selection sort)

 minimum value라는 공간이 필요함

첫 번째 value를 mainmum value에 넣고 리스트를 처음부터 끝까지 순회하면서 더 작은  value가 있다면 스와핑



#### 삽입 정렬(insertion sort)

간단하게 구현 가능하나 효율성이 떨어짐

배열의 모든 요소를 앞에서부터 차례대로 이미 정렬된 배열 부분과 비교 하여, 자신의 위치를 찾아 삽입함



#### 병합 정렬(merge sort)

시간 복잡도: O(n log n)

space  complexity: O(n)

리스트에 하나의 아이템이 남을 때까지 쪼갠 후 비교를 해 정렬될 아이템으로 병합을 시키는 알고리즘

