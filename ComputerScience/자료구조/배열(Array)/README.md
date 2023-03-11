## Array(배열)

배열은 여러 개의 변수를 하나의 이름으로 그룹화하여 사용할 수 있도록 하는 데이터 구조입니다.  
각 변수의 인덱스를 이용하여 접근할 수 있으며, 동일한 데이터 타입만을 저장할 수 있습니다.

### 코틀린에서 배열 사용하기  
코틀린에서 배열을 사용하기 위해서는 다음과 같은 문법을 사용합니다.  
#### [배열의 선언과 초기화]
<pre><code>// Int 형 배열 선언
val numbers: IntArray = intArrayOf(1, 2, 3, 4, 5)

// String 형 배열 선언
val fruits: Array<String> = arrayOf("apple", "banana", "orange")</code></pre>

#### [배열의 사용]
코틀린에서 배열은 인덱스를 이용하여 값을 읽거나 쓸 수 있습니다. 인덱스는 0부터 시작합니다.
<pre><code>// 배열의 값 읽기
val number: Int = numbers[0]
val fruit: String = fruits[1]

// 배열의 값 쓰기
numbers[0] = 10
fruits[1] = "kiwi"</code></pre>

#### [배열의 길이]
코틀린에서 배열의 길이는 다음과 같이 구할 수 있습니다.
<pre><code>val length: Int = numbers.size</code></pre>

#### [배열의 반복문 처리]
코틀린에서 배열의 모든 값을 출력하거나 처리하려면 반복문을 사용합니다.  
다음은 for문을 이용한 배열의 반복문 처리 예시입니다.
<pre><code>for (number in numbers) {
    // 배열의 각 요소에 대한 처리
}

for (index in numbers.indices) {
		// 배열의 인덱스에 대한 처리
}</code></pre>

#### [배열의 정렬]
코틀린에서 배열을 정렬하기 위해서는 다음과 같은 문법을 사용합니다.
<pre><code>numbers.sort() // 오름차순으로 정렬
fruits.sortDescending() // 내림차순으로 정렬</code></pre>

#### [배열의 복사]
코틀린에서 배열을 복사하기 위해서는 다음과 같은 문법을 사용합니다.
<pre><code>val newNumbers = numbers.copyOf()
val newFruits = fruits.copyOfRange(0, n) // 0부터 n까지 복사</code></pre>
