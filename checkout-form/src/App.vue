<template>
    <section class="p-info">
      <h1>Payment information</h1>
      <div class="">
        <img src="/img-card.png" alt="card img">

        <h5>Name on card</h5>
        <input v-model="cardName" maxlength="10" />

        <h5>Card number</h5>
        <input v-model="cardNum" maxlength="16" />

        <h5>expiration date</h5>
        <input v-model="expMonth" maxlength="2" />
        <input v-model="expYear" maxlength="2" />

        <h5>CVC</h5>
        <input v-model="cvc" maxlength="3"/>

        <br />
        <br />

        <button type="submit">Confirm payment</button>
      </div>
    </section>

    <section class="p-order">
      <h1>Order Summary</h1>
      <div>
        <img>
        <h6>Title</h6>
        <small>Ipsum</small>
        <span>550 USD</span>
      </div>
    </section>
  </template>

<script>

export default {
  name: 'App',
  data() {
    return{
      cardName:"",
      cardNum:"",
      expMonth:"",
      expYear:"",
      cvc:""
    }
  }
}
</script>

<style>
#app{
  /*display: flex;*/
  /*justify-content: center;*/
  /*align-items: center;*/
}
.p-info{
  float:left;
  background-color: blanchedalmond;
  margin-left: 700px;
  margin-top: 300px;
  padding: 50px;
  border-radius: 10%;
}
.p-order{
  float:right;
  background-color: blanchedalmond;
  margin-right: 1000px;
  margin-top: 300px;
  padding: 50px;
  border-radius: 10%;
}
</style>
