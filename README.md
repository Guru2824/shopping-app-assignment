# Shopping App Portal

#### Authentication Module

- [x] Login

// User Login
userapi.userLogin(email, password, role).then(res => {
    // console.log(res)
    return res;
});

#### Users Module

- [x] Register

// User Register
userDetailsapi.userRegister(userDetails).then(res => {
    // console.log(res)
    return res;
});

- [x] Get User Details

// To Get User Details
userDetailsapi.getUserDetails(getUserDetails_id).then(res => {
    // console.log(res);
    return res;
});

#### Products Module

- [x] List active products

// List Active Products
productsapi.getAllActiveProducts().then(res => {
    // console.log(res.data);
    return res;
});

- [x] Add Product

// To Add New Products
productsapi.addProduct(product).then(res => {
    console.log(res.data);
    return "Product Added";
});

- [X] Activate/Inactive Product

// To Active InActive Products
var status = true;
productsapi.checkValidProduct(orderId, status).then(res => {
    // console.log(res)
    return res;
});

- [x] Get Product Details

// To Get Product Details
productsapi.getProductDetails(getProductDetails_id).then(res => {
    // console.log(res);
    return res;
});

#### Orders Module
- [x] Add Order

// To Place An New Order
orderapi.productOrders(orderDetails).then(res => {
    // console.log(res.data);
    return res.data;
});

- [x] List All Orders

// List All Orders
orderapi.getAllOrders().then(res => {
    // console.log(res.data);
    return res.data;
});

- [x] List my Orders

// To Get My Order List
orderapi.myOrders(userId).then(res => {
    return res;
});

- [x] Cancel a Order

// To Cancel Order
orderapi.orderCancel(cancelOrderId).then(res => {
    return "Order Cancelled Successfully";
});

- [x] Update order status

// Order Status To Delivered
orderapi.deliveryOrder(deliveryOrderId).then(res => {
    // console.log(res);
    return "Order Delivered Successfully";
});

