<template>
  <div class="Home">
    <div class="wrapper">
      <!-- Header Menu -->
      <div class="header">
        <div class="icon-menu"><svg width="36" height="35" viewBox="0 0 36 35" fill="none"
            xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
            <rect x="0.3125" width="35.3528" height="35" fill="url(#pattern0)" />
            <defs>
              <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
                <use xlink:href="#image0" transform="translate(0 -0.00504031) scale(0.00195312)" />
              </pattern>
              <image id="image0" width="512" height="512"
                xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAgAAAAIACAQAAABecRxxAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAAmJLR0QAAKqNIzIAAAAJcEhZcwAADsQAAA7EAZUrDhsAAAAHdElNRQfjCQMRCAXm9rnTAAAJOUlEQVR42u3dW4xdVRkH8P/ZhRaQWggiFRAo0iLlfi3YcGkVMVYTg0YIEgExgiH6oIm+EUx4UExMkPBAYoKgJaBgkBgjoECRSymgCLbQMlwKSaEtKWVaKQVafBgOc+mUNjDnfGHO7/cye6+1z+S/H9aXfc7ee60EAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIDxr7XNI6ZlZqZn90yqjgpst415NcuyJM+//2FbLwBN5uScfDH7Vp8J8IG9mDszP/dk8+jdoxeAiTk/P8lnqrMDY+KZ/CLX5c0tO0YrAKfn6kyvTgyMqaW5JP8Y2diM2J+UK3O74Q/jzsH5e64Z+Vve8CuAPfKXnFidE+iYB/OVrBncHVoA9srdOaQ6H9BRSzI3K9s7gwVgSu7JUdXZgI77V07LuoHN9m8ArVxr+ENPOCbXtjcnvPv3kvy4OhXQJTOzMo8k7a8AU/NUplRnArqmP4dkRfsK4Cq//UNPmZTdctvAFcB+6cuO1XmArnor07O8SXKJ4Q89Z8dcnLQyIcuzT3UWoOtezAFNjjP8oSd9Okc3Oa06BVBkbpNjqzMARY5pcnB1BqDIwU32rs4AFNmnlTfM9gc9akOzxZQgQK/Yocn66gxAkf4mq6szAEVWN3m6OgNQZFmT/1RnAIo83mRBdQagyN2t7JKXM7k6B9B1r2Vqk9dzS3UOoMDNeaNJck11DqDANQOzAi/MXdVJgC67PQ+3JwU9Ng+9Nz8wMP5tyvH5d3tS0JfyicyqTgR0za/z22RwZaCd8qCFQaBHPJFZ2ZAMrgz0Rs7KK9WpgC5YnTMHhv/Q5cGXZV57vTBg3OrPvPS1d4a+DLwoc7KqOh3QQSszJw8P7g6fDeDRzMpD1QmBDlmYWfnX0IaRN//W5vpsyonZoTopMKY25PJcmDXDG7e8+78pC3Jjdsuh5gqCceKt/C5n59ZsHtnR2upH9s95OcecwfAR91RuyHV5YfTO1jY+vF9OzcxMz5TsXn0ewHZ7NWvTl8VZkBerowAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABRrbaN/58zKzMzIlHysOiqw3danP0uzJIuy4f0O23oBmJxv5NzMzqTqMwE+sI25L/Nzc9aN3j16AdgjP8olmVKdHRgTa3N1fpU1W3a0Rmm5MD/PHtWJgTH1Sn6aa/PO8MaRBWBKfpNvVCcFOuK2XDD8OmB4ATggd2R6dUagY57NGekb3B1aAGbknnyqOh/QUS/l1Dzd3hksAHvn/hxQnQ3ouOfyubw8sNm827RDbjL8oSdMy02ZMLD57p9cmm9XpwK6ZP+8nXuT9leA6XnCAz/QQzbmyCxtfwW4wvCHnjIplycDVwCH5fFtvhMAjC+bc3iWNEm+b/hDz2lycdLKxKzw4C/0oNXZp8lJhj/0pD1zQpPTqlMAReY2Oao6A1DkyCYzqjMARQ5uMrU6A1Bkr1Y2ZmJ1CqDExubD/w/go6rJ+uoIQJH+pv1eMNBzVjZZVp0BKLK0yb+rMwBFHmtyT3UGoMhdXgaCXrUq+zR5MzdW5wAK3Ji3W0kOzePxPAD0ls05LE82SRbn1uosQJfdnCfbk4IelCeyU3UeoGs25LA8254WfE0mZE51IqBrLsttyeDKQE3uzNzqTEBXLMjnsykZujTY1NyfA6tzAR33TGZn5cDm4K//L+eMrKhOBnTYinypPfwz7PZfX2Z7MwDGtaX53NDlwYff/38+x+cP1QmBDvlzTsryoQ0jHwDqz9m5IKurcwJjbFXOz9fy6vDGCaMc+Fh+kzdzpCcDYJx4NVfk3Dy0ZcfWFwXbNV/POTk5O1dnBz6wDbk3N+RPW5v5a1urAu6UEzIzMzIlk6vPBNhu6/JalmVxFmVjdRQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIBirW30T8spmZkZmZzdqqMC221t1mVZFufePP9+h229AEzLeflWDqo+D+BD6cv8/HZrZWD0AjAjl+as7FCdHBgTb+fG/Cx9W3ZM2KJlYi7L73N0murMwBhpckS+lx3zQDYN7xh5BXBgbspx1WmBjliUs/Pc0IbhBeC4/DV7VmcEOmZN5mXh4O7QAnBi7sjk6nxAR63LF7KovTNYAD6b+7JHdTag417J7Cwb2GwXgJ2yMEdW5wK64r+ZldeTwbsAV+ar1ZmALvlkJudvSfsK4LgsHOWGIDBebc5JWZR37/b/0vCHntLk8mTgCuCkPFCdBui6WVnUJLmoOgdQ4KKklV2yMrtWJwG6rj97NTnZ8Iee9PHMbnJqdQqgyJwmR1RnAIoc3mR6dQagyIzG23/Qs/Zs5c3sWJ0CKPFWk83VGYAibzdZV50BKNLfZEV1BqDIiiZLqzMARZY2ebQ6A1Dk0SZ3V2cAitzVSpPl2bc6B9B1L2Rak82ZX50DKDA/m1tJPp2+TKzOAnTVW5me5U2SF/P76ixAl12b5e1JQafmSct/Qw/pz2fzUnta8PXpz7zqREDX/DALkqErA92SM6szAV3xx3xzYGOwAEzO3Tm2OhfQcY9kTtYPbDbvNa7Ll7OkOhnQYYszrz38hxaAZFVOtkIAjGv35eSsGtwdviLQhlyfSZk9bNFwYHx4J1fl3PxvaNNoQ/3UXJ1Dq7MCY2pZfpA7RjY2oxy4IMfku+mrzguMkafznRy25fDP+1zsNzkl5+T0HFCdHfjAns8duSH/3NrUf9v+tr9/ZmZGdsvO1WcCbLcNWZulWZIXqoMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAFDv/5J6UQW0Y1HaAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDE5LTA5LTAzVDE3OjA4OjA1KzAwOjAwggq8XQAAACV0RVh0ZGF0ZTptb2RpZnkAMjAxOS0wOS0wM1QxNzowODowNSswMDowMPNXBOEAAAAZdEVYdFNvZnR3YXJlAHd3dy5pbmtzY2FwZS5vcmeb7jwaAAAAAElFTkSuQmCC" />
            </defs>
          </svg></div>
        <div class="title-header">
          <h2>Foods Items</h2>
        </div>
        <div class="icon-search">
          <form>
            <div>
              <input v-model="search" type="text" name="search" placeholder="Search.." @input="searching()">
            </div>
            <div>
              <b-dropdown size='sm' offset="-100" style="margin-left:5px; height:50px;" variant='outline-primary'>
                <select name="category_id" @click="sortby()" class="form-control">
                  <option selected disabled>sort by:</option>
                  <option value="ID">Id</option>
                  <option value="NAME_PRODUCT">Name</option>
                  <option value="PRICE">Price</option>
                </select>
              </b-dropdown>
            </div>
          </form>
        </div>
      </div>
    </div>
    <div class="wrapper" id="header-cart">
      <div class="header-cart">
        <div class="title-cart">
          <h2>Cart <span> {{ listcart.cartdata.length }} </span></h2>
        </div>
      </div>
    </div>
    <!-- header cart -->
    <div class="wrapper-allcart">
      <div class=" overflow-auto" id="cart">
        <div class="cart-customer">
          <div v-if="listcart.cartdata.length == 0">
            <div class="cart"><img src="@/assets/food-and-restaurant.png"></div>
            <div class="desc-cart" v-if="listcart.cartdata.length == 0">
              <h2>You cart is empty</h2>
              <p>Please add some items from the menu</p>
            </div>
          </div>
          <div v-if="listcart.cartdata.length >= 1" hidden>
            <div class="cart"><img src="@/assets/food-and-restaurant.png"></div>
            <div class="desc-cart" v-if="listcart.cartdata.length >= 1" hidden>
              <h2>You cart is empty</h2>
              <p>Please add some items from the menu</p>
            </div>
          </div>
          <!-- cart -->
          <div class="wrapper-cart" v-for="cart in listcart.cartdata" :key="cart">
            <div class="cart1">
              <img :src="cart.IMG" id="cart-img">
            </div>
            <div class="cart2">
              <cart2-1>
                <h5 style="font-size:20px; text-align:left;"> {{ cart.NAME_PRODUCT}} </h5>
              </cart2-1>
              <div class="cart2-2">
                <b-button-group>
                  <b-button variant="success" style="font-weight: 900;" @click="removeQTY">-</b-button>
                  <div class="form-control total" value="1" v-if="cart.ID"> {{ value }} </div>
                  <b-button variant="success" style="font-weight: 900;" @click="addQTY">+</b-button>
                </b-button-group>
                <h4 style="font-size:18px;margin-left: 50px;">
                  Rp.{{new Intl.NumberFormat('id-ID', { maximumSignificantDigits: 3 }).format(cart.PRICE)}}</h4>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- CHECKOUT BUTTON -->
      <div class="total-price" v-if="listcart.cartdata.length == 0">
      </div>
      <div class="total-price" v-else>
        <h5>Total</h5>
        <h4 style="margin-left:5em;">Rp.{{ listcart.total }}</h4>
      </div>
      <div class="checkout" v-if="listcart.cartdata.length == 0" hidden>
      </div>
      <div class="checkout" v-else>
        <b-button variant="outline-primary" @click="$bvModal.show('bv-modal-CheckOut')"
          style="margin-bottom:15px;font-size:20px;font-weight:700;">CheckOut
        </b-button>
        <b-button variant="danger" @click="clean" style="font-size:20px;font-weight:700;">Cancel</b-button>
      </div>
    </div>
    <!-- SIDEBAR ACTION -->
    <div class="wrapper" id="sidebar">
      <div class="sidebar">
        <div class="sidebar-action">
          <!-- Home -->
          <div class="icon-menus">
            <router-link v-bind:to="'/home'">
              <img src="@/assets/fork.png"><span>Menus</span>
            </router-link>
          </div>
          <!-- HISTORY -->
          <div class="icon-history">
            <router-link v-bind:to="'/history'">
              <img src="@/assets/clipboard.png">
              <span>History</span>
            </router-link>
          </div>
          <!-- MODAL C. R. U. D -->
          <div><img src="@/assets/add.png" @click="$bvModal.show('auth')">
            <b-modal id="CRUD" hide-footer header-border-variant="primary"><template v-slot:modal-title>
                <h3>CoffeeShop <code>CRUD</code></h3>
              </template>
              <div class="d-block text-center">
                <h2>Hello welcome back ! </h2><br>
                <p style="float:left;">Chouse you needed :</p>
              </div>
              <b-button variant="primary" class="mt-3" block @click="$bvModal.show('bv-modal-AddData')">
                <h5>ADD PRODUCT</h5>
              </b-button>
              <b-button variant="outline-primary" class="mt-3" block @click="$bvModal.show('bv-modal-UpdateData')">
                <h5>UPDATE PRODUCT</h5>
              </b-button>
              <b-button variant="outline-primary" class="mt-3" block @click="$bvModal.show('bv-modal-DeleteData')">
                <h5>DELETE PRODUCT</h5>
              </b-button>
            </b-modal>
          </div>
          <!-- USER INFORMATION -->
          <div class="icon-userinfo">
            <img src="@/assets/meetme.png" @click="$bvToast.show('my-toast')" style="margin-top:5.5em">
            <b-toast id="my-toast" variant="primary" solid>
              <template v-slot:toast-title>
                <div class="d-flex flex-grow-1 align-items-baseline">
                  <b-img blank blank-color="#fff" class="mr-2" width="14" height="14"></b-img>
                  <strong class="mr-auto">Notice!</strong>
                  <small class="text-muted mr-2">TOKEN USER</small>
                </div>
              </template>
              <div class="body-info">
                <h5>hello welcome to coffee shop.</h5>
                <p>your information token access:</p>
                <div class="hideToken">
                  <h5> {{ tokenInfo }} </h5>
                </div>
                <img src="@/assets/exit.png"
                  style="width:8em; height:8em; display:block; margin:-1.5em auto 1em; cursor:pointer;"
                  @click="logout()">
              </div>
            </b-toast>
          </div>
        </div>
      </div>
    </div>
    <!-- GET PRODUCT -->
    <b-row id="row">
      <div id="product" v-for="data in product" :key="data.ID" v-on:click="addCart(data)">
        <Product :images="data.IMG" :names="data.NAME_PRODUCT" :price="data.PRICE" />
      </div>
    </b-row>
    <!-- AUTHENTICATION -->
    <b-modal id="auth" hide-footer title="Authentication coffee shop">
      <div class="d-block text-center">
        <h3>C.R.U.D <code><i>Not access!</i></code></h3>
      </div>
      <b-form-input v-model="token" class="mt-3" type="text" placeholder="type your token access"></b-form-input>
      <b-button class="mt-5" variant="primary" block @click="checkToken()">
        <h5>Check token</h5>
      </b-button>
      <b-button class="mt-2" variant="outline-danger" block @click="$bvModal.hide('auth')">
        <h5>Cancel</h5>
      </b-button>
    </b-modal>
    <!-- MODAL ADD PRODUCT -->
    <b-modal id="bv-modal-AddData" size="lg" header-bg-variant="primary" header-text-variant="white"
      header-border-variant="dark" footer-border-variant="dark"><template v-slot:modal-title>
        <h2>Add Product </h2>
      </template><template v-slot:modal-footer>
        <b-button variant="outline-danger" @click="clean">
          <h5>Cancel</h5>
        </b-button>
        <b-button variant="primary" style="width:16em; margin:0 25px 0 15px;" @click="save()">
          <h5 style="font-weight:700;">Add</h5>
        </b-button>
      </template>
      <div class="modal-body">
        <h5 style="margin-top:-10px;">Name</h5>
        <b-form-input v-model="form.NAME_PRODUCT" id="input1" placeholder="name product"></b-form-input>
        <h5 style="margin-top:18px;">Price</h5>
        <div class="input-group mb-3" id="input3">
          <div class="input-group-prepend"><span class="input-group-text">Rp.</span></div>
          <b-form-input v-model="form.PRICE" placeholder="entry price product"></b-form-input>
        </div>
        <h5 style="margin-top:18px;">Image</h5>
        <div class="input-group" id="input2">
          <div class="custom-file"><input v-model="form.IMG" type="text" class="form-control" id="inputGroupFile04"
              aria-describedby="inputGroupFileAddon04" placeholder="link url-image"></div>
          <div class="input-group-append"><button class="btn btn-outline-primary" type="button"
              id="inputGroupFileAddon04">OK ! </button></div>
        </div>
        <h5 style="margin-top:18px;">Category</h5>
        <div id="input4">
          <b-form-select v-model="form.CATEGORY" :options="options">

          </b-form-select>
        </div>
      </div>
    </b-modal>
    <!-- MODAL UPDATE PRODUCT -->
    <b-modal id="bv-modal-UpdateData" size="lg" header-bg-variant="primary" header-text-variant="white"
      header-border-variant="dark" footer-border-variant="dark"><template v-slot:modal-title>
        <h2>Update Product </h2>
      </template><template v-slot:modal-footer>
        <b-button variant="outline-danger" @click="clean">
          <h5>Cancel</h5>
        </b-button>
        <b-button variant="primary" style="width:16em; margin:0 25px 0 15px;" @click="Update()">
          <h5 style="font-weight:700;">Update</h5>
        </b-button>
      </template>
      <div class="modal-body">
        <div class="input-group" id="input2" style="width: 40%; float:right; border:1px solid black; border-radius:5%;">
          <div class="custom-file">
            <b-form-input v-model="update.ID" placeholder="type id product"></b-form-input>
          </div>
          <div class="input-group-append"><button class="btn btn-outline-primary" type="button">Search</button></div>
        </div>
        <h5 style="margin-top: 40px;">Name</h5>
        <b-form-input v-model="update.NAME_PRODUCT" id="input2" placeholder="name product"></b-form-input>
        <h5 style="margin-top:18px;">Price</h5>
        <div class="input-group mb-3" id="input3">
          <div class="input-group-prepend"><span class="input-group-text">Rp.</span></div>
          <b-form-input v-model="update.PRICE" placeholder="entry price product"></b-form-input>
        </div>
        <h5 style="margin-top:18px;">Image</h5>
        <div class="input-group" id="input2">
          <div class="custom-file"><input v-model="update.IMG" type="text" class="form-control"
              placeholder="link url-image"></div>
          <div class="input-group-append"><button class="btn btn-outline-primary" type="button">OK ! </button>
          </div>
        </div>
        <h5 style="margin-top:18px;">Category</h5>
        <div id="input4">
          <b-form-select v-model="update.CATEGORY" :options="options" v-if="selected == null">
            <h2> </h2>
          </b-form-select>
        </div>
      </div>
    </b-modal>
    <!-- MODAL DELETE PRODUCT -->
    <b-modal id="bv-modal-DeleteData" hide-footer header-bg-variant="primary" header-text-variant="white"
      header-border-variant="dark"><template v-slot:modal-title>
        <h4>Delete Product</h4>
      </template>
      <div class="d-block text-center">
        <b-input-group prepend="ID" class="mt-3">
          <b-form-input v-model="deleteID"></b-form-input>
        </b-input-group>
      </div>
      <b-button variant="outline-danger" class="mt-3" block @click="Delete()"
        style="width:15em;display:block; margin:20px auto;">
        <h4>Delete </h4>
      </b-button>
    </b-modal>
    <!-- MODAL CHECKOUT USER -->
    <div>
      <b-modal id="bv-modal-CheckOut" hide-footer header-bg-variant="primary">
        <template v-slot:modal-title>
          <h2 style="color:white;">Checkout</h2>

          <div class="cashier" style="display:flex; flex-direction:row; color:white;">
            <p style="margin-right:10px; margin-bottom:-10px;"> Cashier : <span>adityaUdi</span></p>
          </div>
        </template>
        <div class="checkout-list overflow-auto" block style="height:15em; margin-bottom:30px;">
          <div class="list" v-for="items in listcart.cartdata" :key="items">
            <div class="menu1" style="margin-top:15px;">
              <h5>{{items.NAME_PRODUCT}}</h5>
            </div>
            <div class="menu2" style="margin-top:15px;">
              <h5>Rp. {{items.PRICE}}</h5>
            </div>
          </div>
        </div>
        <div class="total-list" style="display:flex; flex-direction:row; justify-content:flex-end;">
          <h5>total:</h5>
          <h5 style="padding-right: 20px; padding-left: 50px;">{{ listcart.total }}</h5>
        </div>
        <div class="total-list" style="display:flex; flex-direction:row; justify-content:flex-start;">
          <h5>payment: <code>Cash</code></h5>
        </div>
        <div style="margin-top:-2em;">
          <b-button variant=outline-danger class="mt-5" block @click="print">
            <h5> Print</h5>
          </b-button>
          <b-button variant=primary class="mt-2" block @click="$bvModal.hide('bv-modal-example')">
            <h5>Send Email </h5>
          </b-button>
        </div>
      </b-modal>
    </div>
    <!-- MODAL AUTH TOKEN -->
    <div>
      <b-modal id="modal-auth" hide-footer hide-header-close no-close-on-esc no-close-on-backdrop
        title="Coffee Shop AUTHENTICATION">
        <h5><code>PLEASE CHECK YOUR TOKEN ON LOGIN.</code> </h5>
        <div class="body" style="display:flex; flex-direction:row;">
          <b-input v-model="tokenUser" placeholder="Token..." style="width:90%; margin-top:5px;"></b-input>
          <h5 style="padding:10px 15px;cursor:pointer;" @click="next()"><i> NEXT</i></h5>
        </div>
      </b-modal>
    </div>
  </div>
</template>
<script>
  import Product from '../../components/product'
  import axios from 'axios'

  export default {
    name: 'product',
    components: {
      Product,
    },
    data() {
      return {
        product: [],
        listcart: {
          cartdata: [],
          total: 0,
        },
        search: '',
        selected: null,
        options: [{
            value: null,
            text: 'Please select an category',
            disabled: true
          },
          {
            value: 'Foods',
            text: 'Foods'
          },
          {
            value: 'Drinks',
            text: 'Drinks'
          },
          {
            value: 'Fried',
            text: 'Fried'
          },
          {
            value: 'Coffee',
            text: 'Coffee'
          },
        ],
        form: {
          NAME_PRODUCT: '',
          PRICE: 0,
          IMG: '',
          CATEGORY: ''
        },
        value: 1,
        update: {
          ID: '',
          NAME_PRODUCT: '',
          PRICE: '',
          IMG: '',
          CATEGORY: ''
        },
        deleteID: '',
        addHistory: {
          CASHIER: 'adityaudi',
          DATE: 'Kamis 22 Sep 2020',
          ORDERS: [],
          AMOUNT: 0
        },
        token: '',
        tokenInfo: '',
        tokenUser: ''
      }
    },
    mounted() {
      this.load()
    },
    methods: {
      load() {
        this.$bvModal.show('modal-auth')
      },
      next() {
        if (this.tokenUser != "") {
          axios.get(process.env.VUE_APP_URL, {
              token: this.tokenUser
            })
            .then((result) => {
              this.$bvModal.hide('modal-auth')
              this.tokenInfo = this.tokenUser
              this.product = result.data
              this.tokenUser = ''
              console.log(result)
            })
            .catch((error) => {
              alert('Token: Invalid token!', error)
            });
        } else {
          alert('token column is not filled!')
        }
      },
      sortby() {
        axios.get(`${process.env.VUE_APP_URL}/filterby?sort=${event.target.value}`)
          .then((result) => {
            this.product = result.data
          }).catch((err) => {
            alert('erorr', err)
          });
      },
      save() {
        axios.post(process.env.VUE_APP_URL + '/add', this.form)
          .then((res) => {
            this.form = []
            this.clean()
            alert('Product Sucessfully Saved!', res)
          }).catch(err => {
            alert('Data Error!' + err)
          })
      },
      print() {
        axios.post(process.env.VUE_APP_URL_HISTORY, this.addHistory)
        alert('Terimakasih telah berbelanja!')
      },

      Update() {
        axios.put(process.env.VUE_APP_URL, {
            ID: this.update.ID,
            NAME_PRODUCT: this.update.NAME_PRODUCT,
            PRICE: this.update.PRICE,
            IMG: this.update.IMG,
            CATEGORY: this.update.CATEGORY
          })
          .then((res) => {
            alert('Product was Updated!', res)
            this.form = []
            this.clean()
          })
          .catch(err => {
            alert('update error!', err)
          })
      },
      Delete() {
        axios.delete(`${process.env.VUE_APP_URL}/delete/${this.deleteID}`)
          .then(res => {
            alert("Success delete product", res)
            this.form = []
            this.clean()
          })
          .catch(err => {
            alert('delete product errorr!', err)
          })
      },
      clean() {
        this.$bvModal.hide('bv-modal-AddData')
        this.$bvModal.hide('bv-modal-UpdateData')
        this.$bvModal.hide('bv-modal-DeleteData')
        this.listcart.cartdata = []
        this.form = []
      },
      addCart(data) {
        this.listcart.cartdata.push(data)
        this.listcart.total += Number(data.PRICE)
        this.addHistory.ORDERS.push(data.NAME_PRODUCT)
        this.addHistory.AMOUNT += Number(data.PRICE)
      },
      searching() {
        axios.get(`${process.env.VUE_APP_URL}/search?name=${this.search}`)
          .then(res => {
            this.product = res.data
          }).catch(err => {
            this.product = [], err
          })
      },
      addQTY() {
        this.value += 1
        this.listcart.total = this.listcart.cartdata[0].PRICE * this.value
      },
      removeQTY() {
        if (this.value > 1) {
          this.value -= 1
          this.listcart.total = this.listcart.cartdata[0].PRICE * this.value
        } else {
          this.listcart.cartdata = []
        }
      },
      checkToken() {
        if (this.token != "") {
          axios.post(process.env.VUE_APP_URL, {
              token: this.token
            })
            .then((result) => {
              this.$bvModal.hide('auth')
              this.$bvModal.show('CRUD')
              this.token = ''
              console.log(result)
            })
            .catch((err) => {
              alert('Token invalid, pls call admin to access myCRUD!', err)
            });
        } else {
          alert('token column is not filled!')
        }
      },
      logout() {
        this.$bvToast.toast(
          alert('Logout berhasil, Sampai Jumpa!'),
          this.$router.replace({
            name: "login"
          }),
          this.$bvToast.hide('my-toast'),
          this.tokenInfo = ''
        )
      },
    }
  }
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .icon-menus span,
  .icon-menus a {
    color: white;
    background-color: #007BFe;
  }

  .icon-history span,
  .icon-history a {
    color: black;
    background-color: unset;
  }

  .sidebar a {
    text-decoration: none;
    color: black;
  }

  .header {
    background-color: white;
    width: 73%;
    height: 4.5em;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.25);
    position: fixed;
    z-index: 1;
    border-radius: 8px;
    border-bottom: #007BFF solid;
    box-shadow: 10px 10px rgba(144, 144, 144, 0.212);
  }

  .icon-menu {
    padding-left: 40px;
    cursor: pointer;
  }

  .icon-search {
    padding-right: 30px;
    cursor: pointer;
    border: 1px white solid;
  }

  .header-cart {
    width: 27.6%;
    height: 4.5em;
    margin-left: 58.6em;
    background-color: white;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.25);
    z-index: 1;
    text-align: center;
    border-radius: 8px;
    border-bottom: #007BFF solid;
    box-shadow: 10px 10px rgba(144, 144, 144, 0.212);
    position: fixed;
  }

  .title-cart h2 {
    padding-top: 12px;
  }

  .header-cart span {
    background-color: #57CAD5;
    color: white;
    border-radius: 20%;
  }

  .sidebar {
    width: 4em;
    height: 39em;
    background-color: white;
    padding-top: 7em;
    margin-left: 1.5em;
    padding-bottom: 12em;
    border-radius: 8px;
    border-bottom: #007BFF solid;
    box-shadow: 10px 10px rgba(144, 144, 144, 0.212);
    position: fixed;
    cursor: pointer;
  }

  .sidebar-action {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    font-weight: 500;
    font-size: 16px;
  }

  .sidebar-action img:hover {
    transform: scale(1.1);
  }

  .sidebar-action img {
    padding: 1.4em;
  }

  .wrapper-allcart {
    width: 100%;
    height: 100%;
    margin: 4.8em auto auto 58.8em;
    position: fixed;
    background-color: white;
    border-radius: 8px;
    box-shadow: -10px 10px rgba(144, 144, 144, 0.212);
  }

  .sidebar .icon-userinfo img {
    width: 100px;
    height: 100px;
  }

  #cart {
    width: 21.7em;
    height: 58%;
    margin-bottom: 30px;
  }

  .cart-customer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  /* MODEL STYLING */
  #bv-modal-AddData h5 {
    font-family: sans-serif;
  }

  #bv-modal-AddData .modal-body #input1,
  #input2,
  #input3,
  #input4 {
    box-sizing: border-box;
    box-shadow: 0px 4px 6px rgba(228, 214, 214, 10);
  }

  /* cart style */
  #row {
    width: 80%;
    margin-left: 5em;
    padding-top: 4.5em;
  }

  /* atur cart */
  .wrapper-cart .cart2 {
    padding-top: 20px;
  }

  .wrapper-cart .cart2-2 {
    display: flex;
    flex-direction: row;
    justify-items: center;
    align-items: center;
  }

  .wrapper-cart {
    display: flex;
    flex-direction: row;
    width: 20%;
    justify-content: center;
    align-items: flex-start;
  }

  .wrapper-cart img {
    width: 5em;
    height: 5em;
    margin-top: 20px;
    margin-right: 12px;
  }

  .total-price {
    display: flex;
    flex-direction: row;
    margin-left: 30px;
    justify-items: center;
    align-items: center;
  }

  .checkout {
    display: flex;
    flex-direction: column;
    width: 18em;
    margin-top: 1em;
    margin-left: 30px;
  }

  form {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: flex-end;
  }

  form input[type=text] {
    width: 130px;
    box-sizing: border-box;
    border: 2px solid #ccc;
    border-radius: 4px;
    font-size: 16px;
    background-color: white;
    background-image: url('https://cms-assets.tutsplus.com/uploads/users/523/posts/27345/preview_image/search-icon-large.png');
    background-repeat: no-repeat;
    background-size: 4em;
    background-position: right;
    padding: 12px 20px 12px 10px;
    -webkit-transition: width 0.2s ease-in-out;
    transition: width 0.6s ease-in-out;
    float: right;
  }

  form input[type=text]:focus {
    width: 100%;
  }

  .checkout-list {
    display: flex;
    flex-direction: column;

  }

  .list {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }

  .hideToken {
    overflow-x: auto;
    overflow-y: hidden;
    background-color: white;
    margin: 1.5em auto 3em;
  }

  #modal-auth .body h5:hover {
    background-color: #007BFF;
    color: white;
    margin-left: 10px;
  }
</style>