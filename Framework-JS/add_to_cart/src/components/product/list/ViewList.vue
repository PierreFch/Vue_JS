<template>
    <div class="item" v-for="item in items" :key="item.text">
        <div class="picture">
            <img src="https://fakeimg.pl/300x150/" alt="Image produit" title="magasin de quelque chose quelque part">
        </div>
        <div class="description">
            <h2>{{item.text}}</h2>
            <p>{{item.description}}</p>
            <div class="bottom">
                <div class="quantity">
                    <input type="number" id="quantity" name="quantity" min="1" v-model="item.qty"/>
                </div>
                <div class="flex">
                    <div class="add">
                        <button v-on:click="addToCart(item)">Ajouter au panier</button>
                    </div>
                    <div class="price">
                        <p>{{item.price}}</p>
                    </div>
                </div>
            </div>
        </div> 
    </div>
</template>

<script>
export default {
  name: 'ViewList',
  props: {
    name: String,
    text: String
  },
  data(){
      return{
          items: [
                {text: "Produit 1", description: "Mon premier produit à vendre", price: "10€"},
                {text: "Produit 2", description: "Mon deuxième produit à vendre", price: "20€"},
                {text: "Produit 3", description: "Mon troisème produit à vendre", price: "30€"},
                {text: "Produit 4", description: "Mon quatrième produit à vendre", price: "5€"},
                {text: "Produit 5", description: "Mon cinquième produit à vendre", price: "2€"},
                {text: "Produit 6", description: "Mon sixième produit à vendre", price: "40€"},
          ]
      }
  },
  methods: {
		// Add Items to cart
    addToCart(itemToAdd) {
      // Add the item or increase qty
			let itemInCart = this.cartItems.filter(item => item.id===itemToAdd.id);
			let isItemInCart = itemInCart.length > 0;

      if (isItemInCart === false) {
      
				itemInCart[0].qty += itemToAdd.qty;
			}
			itemToAdd.qty = 1;
    }
  }
}
</script>

<style scoped>
.item{
    margin: 20px;
    width: calc(30% - 20px);
    box-shadow: 0 10px 15px 5px #EBEBEB;
}
img{width: 100%;}
.description{
    padding: 20px;
}
h2{
    margin: 0;
}
.flex{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.price p{
    font-weight: 600;
    font-size: 1.1em;
}
button{
    border: 1.5px solid transparent;
    background: #1A1A1C;
    color: #FFF;
    padding: 10px 20px;
    font-size: 0.9em;
    cursor: pointer;
    transition-duration: 150ms;
    margin: 10px 0;
}
button:hover{
    border: 1.5px solid #1A1A1C;
    background: #FFF;
    color: #1A1A1C;
}
</style>