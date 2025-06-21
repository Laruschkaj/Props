# Props
15.2.16 Props Exercise

# Props Exercise

## Spacecraft Inventory System 🌌

Hello, future software developer! In this exercise, we will practice props in React by creating a spacecraft inventory management system. 🥹

Your mission is to showcase various items aboard a spacecraft, detailing each one's name, type, quantity, and price. But there's a twist! You'll need to implement smart messages within your application: one to warn when any item's stock is running low 🚨 and another to highlight items of high value 💎 that could attract interstellar thieves. This is how it should look: 

![Demo.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/163f1722-85e9-4a3c-adba-457a91094f00/9a8726c0-98cc-4df3-8f77-20dc6b9d82f7/Demo.png)

## Tasks 📋

- `index.html`
    - Add CDN links for React, ReactDOM, and Babel to enable JSX processing in the browser.
    - Add the message, inventory item, and app component files. Be mindful of their import order.
- `Message.js`
    - Accept `children` as props and render them as is.
- `InventoryItem.js`
    - Accept `name`, `type`, `quantity`, and `price` as props.
    - Set defaults to `quantity` and `price`.
    - Render the item's details.
    - Render a `Message` if the quantity is below the 5 threshold, indicating low stock.
    - Render a `Message` if the total value (`quantity * price`) exceeds the $1000 threshold, suggesting extra protection due to high value.
- `App.js`
    - You are given a list of inventory items. Feel free to change the list.
    - Loop through the inventory items and render an `InventoryItem` for each item in the list.

Happy coding!

## Starter Code 🌱

- `index.html` serves as the entry point for the web application. You will load React libraries and link to the React component scripts for in-browser JSX processing.
- `App.js` is the main component that you will use to aggregate the inventory list, rendering `InventoryItem` components for each item in the inventory.
- `InventoryItem.js` represents individual inventory items. You will display their name, type, quantity, and price. You will also conditionally render messages based on stock levels and value.
- `Message.js` displays warnings or notifications. You will render the wrapped messages through its children props.