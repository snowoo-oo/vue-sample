<template>
  <div>
    <div>
      <select name="" id="">
        <option value=""></option>
        <option :value="city.code" :key="city.code" v-for="city in cities">
          {{ city.title }}
        </option>
      </select>
    </div>

    <div>
      <table>
        <thead>
          <tr>
            <th>제품번호</th>
            <th>제품명</th>
            <th>가격</th>
            <th>주문수량</th>
            <th>합계</th>
          </tr>
        </thead>
        <tbody>
          <tr :key="drink.id" v-for="drink in dirnkList">
            <td>{{ drink.id }}</td>
            <td>{{ drink.name }}</td>
            <td>{{ drink.price }}</td>
            <td><input type="number" v-model="drink.qty" /></td>
            <td>{{ drink.price * drink.qty }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      cities: [
        { title: '서울', code: '02' },
        { title: '부산', code: '051' },
        { title: '경기', code: '031' }
      ],
      dirnkList: [
        { id: 1, name: '콜라1', qty: 1, price: 1000 },
        { id: 2, name: '콜라2', qty: 2, price: 2000 },
        { id: 3, name: '콜라3', qty: 3, price: 3000 },
        { id: 4, name: '콜라4', qty: 4, price: 4000 },
        { id: 5, name: '콜라5', qty: 5, price: 5000 },
        { id: 6, name: '콜라6', qty: 6, price: 6000 }
      ]
    }
  }
}
</script>

<style></style>
