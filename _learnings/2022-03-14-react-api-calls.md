---
title: "Making API calls using useEffect"
permalink: /react-api-calls-using-useEffect/
---

Hello

```react
import React, { useState } from "react";
import "./styles.css";
import AllTheThings from "./components/AllTheThings";
import MyShoppingCart from "./components/MyShoppingCart";
import Form from "./components/Form";
import productsArr from "./products";

export default function App() {
  const [products, setProducts] = useState(productsArr);
  const [cart, setCart] = useState([]);

  // create an addToCart function that takes in a product as a param
  const addToCart = (i) => {
    // using the ...spread operator add the product to the cart array
    setCart([...cart, products[i]]);
  };

  // using the ...spread operator add the product to the cart array
  const removeFromCart = (i) => {
    // using Array.filter remove create a new array where that item is removed
    setCart(cart.filter((product, index) => index !== i));
  };

  const handleSubmit = (newProduct) => {
    setProducts([newProduct, ...products]);
  };

  return (
    <div className="App">
      <h1>Big Time Shopping</h1>
      <Form handleSubmit={handleSubmit} />
      <div className="products">
        <AllTheThings products={products} addToCart={addToCart} />
        <MyShoppingCart cart={cart} removeFromCart={removeFromCart} />
      </div>
    </div>
  );
}

```