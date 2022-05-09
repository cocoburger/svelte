<script>
  let count = 0; // state
  let people = {
    name: "철수",
    age: 20,
    sex: "남성",
  };

  let list = [
    {
      id: 0,
      content: "첫 번째 할 일",
      done: false,
    },
    {
      id: 1,
      content: "두 번째 할 일",
      done: false,
    },
    {
      id: 2,
      content: "세 번째 할 일",
      done: true,
    },
    {
      id: 3,
      content: "네 번째 할 일",
      done: false,
    },
  ];

  const handleClick = () => (count = count + 1); //count를 count +1로 재할당.
</script>

<h2>이름 : {people.name}</h2>
<h2>나이 : {people.age}</h2>
<h2>성별 : {people.sex}</h2>

<ul>
  {#each list as item}
    <li>
      <p>{item.id}</p>
      <p>{item.content}</p>
      <p>{item.done}</p>
    </li>
  {/each}
</ul>
