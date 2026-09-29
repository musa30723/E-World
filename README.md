<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>E World | Phones, Cars & Real Estate</title>

<meta name="description"
content="E World marketplace for phones, accessories, cars and real estate in UAE and Kenya.">

<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Arial,Helvetica,sans-serif;
    background:#f5f7fb;
    color:#111827;
}

a{
    text-decoration:none;
    color:inherit;
}

button,
input,
select{
    font:inherit;
}

/* TOP BAR */

.topbar{
    background:#0b1220;
    color:white;
    padding:9px 5%;
    display:flex;
    justify-content:space-between;
    gap:15px;
    font-size:13px;
}

/* NAVIGATION */

.navbar{
    background:white;
    border-bottom:1px solid #e5e7eb;
    padding:15px 5%;
    display:flex;
    align-items:center;
    gap:25px;
    position:sticky;
    top:0;
    z-index:100;
}

.logo{
    font-size:28px;
    font-weight:900;
    white-space:nowrap;
}

.logo span{
    color:#2563eb;
}

.search{
    flex:1;
    position:relative;
}

.search input{
    width:100%;
    padding:13px 18px;
    border:1px solid #d1d5db;
    border-radius:12px;
    outline:none;
    font-size:15px;
}

.search input:focus{
    border-color:#2563eb;
}

.nav-actions{
    display:flex;
    gap:8px;
}

.btn{
    border:0;
    padding:11px 15px;
    border-radius:10px;
    cursor:pointer;
    font-weight:700;
}

.currency{
    background:#eef2ff;
    color:#1d4ed8;
}

.cart{
    background:#111827;
    color:white;
}

/* HERO */

.hero{
    margin:28px 5%;
    padding:55px 7%;
    border-radius:25px;
    color:white;
    background:
    linear-gradient(120deg,#0f172a,#1d4ed8 60%,#7c3aed);
    display:flex;
    justify-content:space-between;
    align-items:center;
    gap:30px;
}

.hero-small{
    color:#bfdbfe;
    font-weight:800;
    margin-bottom:12px;
}

.hero h1{
    font-size:clamp(38px,6vw,68px);
    line-height:1;
    margin-bottom:20px;
}

.hero p{
    max-width:650px;
    font-size:18px;
    line-height:1.6;
    color:#dbeafe;
}

.hero-buttons{
    display:flex;
    gap:10px;
    margin-top:25px;
    flex-wrap:wrap;
}

.hero-button{
    background:white;
    color:#111827;
    padding:13px 18px;
    border-radius:10px;
    font-weight:800;
}

.hero-button.secondary{
    background:#ffffff22;
    color:white;
    border:1px solid #ffffff55;
}

.hero-icon{
    font-size:110px;
}

/* MAIN */

.container{
    width:90%;
    max-width:1300px;
    margin:auto;
}

.section{
    margin:45px 0;
}

.section-title{
    display:flex;
    justify-content:space-between;
    align-items:end;
    margin-bottom:20px;
}

.section-title h2{
    font-size:28px;
}

.muted{
    color:#6b7280;
    margin-top:5px;
}

/* CATEGORIES */

.categories{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.category{
    background:white;
    padding:25px;
    border-radius:18px;
    border:1px solid #e5e7eb;
    display:flex;
    align-items:center;
    gap:18px;
    transition:.2s;
}

.category:hover{
    transform:translateY(-3px);
    box-shadow:0 12px 30px #00000012;
}

.category-icon{
    font-size:45px;
}

.category h3{
    margin-bottom:6px;
}

/* PRODUCTS */

.products{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:18px;
}

.product{
    background:white;
    border-radius:18px;
    overflow:hidden;
    border:1px solid #e5e7eb;
    transition:.2s;
}

.product:hover{
    transform:translateY(-3px);
    box-shadow:0 12px 30px #00000012;
}

.product-image{
    height:190px;
    background:linear-gradient(135deg,#e0e7ff,#f8fafc);
    display:flex;
    justify-content:center;
    align-items:center;
    font-size:75px;
    position:relative;
}

.badge{
    position:absolute;
    top:10px;
    left:10px;
    background:#111827;
    color:white;
    padding:6px 9px;
    border-radius:7px;
    font-size:11px;
    font-weight:800;
}

.product-info{
    padding:16px;
}

.product-info h3{
    font-size:17px;
    margin-bottom:7px;
}

.details{
    color:#6b7280;
    font-size:13px;
}

.price{
    font-size:21px;
    font-weight:900;
    margin:12px 0;
}

.product-buttons{
    display:flex;
    gap:8px;
}

.whatsapp{
    background:#16a34a;
    color:white;
    flex:1;
}

.buy{
    background:#2563eb;
    color:white;
    flex:1;
}

/* SELL SECTION */

.sell-box{
    background:white;
    border-radius:20px;
    border:1px solid #e5e7eb;
    padding:30px;
    display:grid;
    grid-template-columns:1.5fr 1fr;
    gap:30px;
}

.sell-box h2{
    margin-bottom:10px;
}

.contact-buttons{
    display:flex;
    gap:10px;
    flex-wrap:wrap;
    margin-top:20px;
}

.payment-list{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
    margin-top:15px;
}

.payment{
    background:#f3f4f6;
    padding:10px 12px;
    border-radius:9px;
    font-weight:700;
    font-size:13px;
}

/* FOOTER */

footer{
    background:#0b1220;
    color:#cbd5e1;
    padding:40px 5%;
    margin-top:60px;
}

.footer-grid{
    max-width:1300px;
    margin:auto;
    display:grid;
    grid-template-columns:2fr 1fr 1fr;
    gap:30px;
}

footer h3{
    color:white;
    margin-bottom:12px;
}

footer p{
    line-height:1.8;
}

.footer-logo{
    color:white;
    font-size:27px;
    font-weight:900;
}

.footer-logo span{
    color:#60a5fa;
}

.copyright{
    max-width:1300px;
    margin:30px auto 0;
    border-top:1px solid #263244;
    padding-top:20px;
    font-size:13px;
}

/* EMPTY SEARCH */

.empty{
    display:none;
    text-align:center;
    padding:40px;
    background:white;
    border-radius:15px;
    color:#6b7280;
}

/* MOBILE */

@media(max-width:950px){

    .products{
        grid-template-columns:repeat(2,1fr);
    }

    .navbar{
        flex-wrap:wrap;
    }

    .search{
        order:3;
        flex-basis:100%;
    }

    .sell-box{
        grid-template-columns:1fr;
    }

}

@media(max-width:650px){

    .topbar{
        flex-direction:column;
        text-align:center;
    }

    .navbar{
        padding:13px 4%;
        gap:12px;
    }

    .logo{
        font-size:24px;
    }

    .hero{
        margin:18px 4%;
        padding:40px 25px;
    }

    .hero-icon{
        display:none;
    }

    .hero h1{
        font-size:40px;
    }

    .container{
        width:92%;
    }

    .categories{
        grid-template-columns:1fr;
    }

    .products{
        grid-template-columns:1fr 1fr;
        gap:10px;
    }

    .product-image{
        height:145px;
        font-size:55px;
    }

    .product-info{
        padding:11px;
    }

    .product-info h3{
        font-size:14px;
    }

    .price{
        font-size:17px;
    }

    .product-buttons{
        flex-direction:column;
    }

    .footer-grid{
        grid-template-columns:1fr;
    }
}
</style>
</head>

<body>

<!-- TOP BAR -->

<div class="topbar">
    <span>🚚 Delivery across UAE & Kenya</span>
    <span>💳 Card • 🏦 Bank Transfer • 💬 WhatsApp Orders</span>
</div>


<!-- NAVIGATION -->

<nav class="navbar">

    <a href="#" class="logo">
        E<span>World</span>
    </a>

    <div class="search">
        <input
            type="text"
            id="search"
            placeholder="Search phones, cars, properties..."
        >
    </div>

    <div class="nav-actions">

        <button
            class="btn currency"
            id="currencyButton"
            onclick="changeCurrency()">
            AED د.إ
        </button>

        <button
            class="btn cart"
            onclick="showCart()">
            🛒 Cart
        </button>

    </div>

</nav>


<!-- HERO -->

<section class="hero">

    <div>

        <div class="hero-small">
            WELCOME TO E WORLD
        </div>

        <h1>
            Everything you need.<br>
            All in one world.
        </h1>

        <p>
            Shop phones and accessories, discover cars,
            and find real estate listings — all in one marketplace.
        </p>

        <div class="hero-buttons">

            <a href="#phones" class="hero-button">
                📱 Shop Phones
            </a>

            <a href="#categories"
               class="hero-button secondary">
                Explore Categories
            </a>

        </div>

    </div>

    <div class="hero-icon">
        📱
    </div>

</section>


<main class="container">


<!-- CATEGORIES -->

<section class="section" id="categories">

    <div class="section-title">

        <div>
            <h2>Shop by Category</h2>
            <p class="muted">
                Find what you are looking for
            </p>
        </div>

    </div>

    <div class="categories">

        <a href="#phones" class="category">

            <div class="category-icon">📱</div>

            <div>
                <h3>Phones & Accessories</h3>
                <p class="muted">
                    New & used devices
                </p>
            </div>

        </a>


        <a href="#cars" class="category">

            <div class="category-icon">🚗</div>

            <div>
                <h3>Cars</h3>
                <p class="muted">
                    Cars for sale
                </p>
            </div>

        </a>


        <a href="#realestate" class="category">

            <div class="category-icon">🏠</div>

            <div>
                <h3>Real Estate</h3>
                <p class="muted">
                    Homes & properties
                </p>
            </div>

        </a>

    </div>

</section>


<!-- PHONES -->

<section class="section" id="phones">

    <div class="section-title">

        <div>
            <h2>📱 Phones & Accessories</h2>

            <p class="muted">
                Featured products
            </p>
        </div>

    </div>


    <div class="products" id="phoneProducts">

        <!-- PRODUCT 1 -->

        <article
            class="product"
            data-search="iphone 17 pro max apple phone">

            <div class="product-image">

                📱

                <span class="badge">
                    FEATURED
                </span>

            </div>

            <div class="product-info">

                <h3>
                    iPhone 17 Pro Max
                </h3>

                <div class="details">
                    256GB • Like New • Dubai
                </div>

                <div
                    class="price"
                    data-aed="5499"
                    data-kes="199000">
                </div>

                <div class="product-buttons">

                    <button
                        class="btn whatsapp"
                        onclick="orderWhatsApp('iPhone 17 Pro Max')">
                        WhatsApp
                    </button>

                    <button
                        class="btn buy"
                        onclick="buyProduct('iPhone 17 Pro Max')">
                        Buy
                    </button>

                </div>

            </div>

        </article>


        <!-- PRODUCT 2 -->

        <article
            class="product"
            data-search="samsung galaxy s26 ultra phone">

            <div class="product-image">

                📲

                <span class="badge">
                    NEW
                </span>

            </div>

            <div class="product-info">

                <h3>
                    Samsung Galaxy S26 Ultra
                </h3>

                <div class="details">
                    512GB • New • Dubai
                </div>

                <div
                    class="price"
                    data-aed="4999"
                    data-kes="181000">
                </div>

                <div class="product-buttons">

                    <button
                        class="btn whatsapp"
                        onclick="orderWhatsApp('Samsung Galaxy S26 Ultra')">
                        WhatsApp
                    </button>

                    <button
                        class="btn buy"
                        onclick="buyProduct('Samsung Galaxy S26 Ultra')">
                        Buy
                    </button>

                </div>

            </div>

        </article>


        <!-- PRODUCT 3 -->

        <article
            class="product"
            data-search="airpods pro apple headphones">

            <div class="product-image">

                🎧

                <span class="badge">
                    POPULAR
                </span>

            </div>

            <div class="product-info">

                <h3>
                    AirPods Pro
                </h3>

                <div class="details">
                    USB-C • New
                </div>

                <div
                    class="price"
                    data-aed="899"
                    data-kes="32500">
                </div>

                <div class="product-buttons">

                    <button
                        class="btn whatsapp"
                        onclick="orderWhatsApp('AirPods Pro')">
                        WhatsApp
                    </button>

                    <button
                        class="btn buy"
                        onclick="buyProduct('AirPods Pro')">
                        Buy
                    </button>

                </div>

            </div>

        </article>


        <!-- PRODUCT 4 -->

        <article
            class="product"
            data-search="phone case accessory">

            <div class="product-image">

                📱

                <span class="badge">
                    DEAL
                </span>

            </div>

            <div class="product-info">

                <h3>
                    Premium Phone Case
                </h3>

                <div class="details">
                    Shockproof • Universal
                </div>

                <div
                    class="price"
                    data-aed="79"
                    data-kes="2850">
                </div>

                <div class="product-buttons">

                    <button
                        class="btn whatsapp"
                        onclick="orderWhatsApp('Premium Phone Case')">
                        WhatsApp
                    </button>

                    <button
                        class="btn buy"
                        onclick="buyProduct('Premium Phone Case')">
                        Buy
                    </button>

                </div>

            </div>

        </article>

    </div>

    <div id="noResults" class="empty">
        No products found.
    </div>

</section>


<!-- CARS -->

<section class="section" id="cars">

    <div class="section-title">

        <div>

            <h2>🚗 Cars</h2>

            <p class="muted">
                Featured vehicle listings
            </p>

        </div>

    </div>


    <div class="products">


        <article class="product">

            <div class="product-image">

                🚙

                <span class="badge">
                    CAR
                </span>

            </div>

            <div class="product-info">

                <h3>
                    Toyota Land Cruiser
                </h3>

                <div class="details">
                    Dubai • Automatic • 2022
                </div>

                <div
                    class="price"
                    data-aed="235000"
                    data-kes="8500000">
                </div>

                <div class="product-buttons">

                    <button
                        class="btn whatsapp"
                        onclick="orderWhatsApp('Toyota Land Cruiser')">
                        WhatsApp
                    </button>

                </div>

            </div>

        </article>


        <article class="product">

            <div class="product-image">

                🚘

                <span class="badge">
                    CAR
                </span>

            </div>

            <div class="product-info">

                <h3>
                    Nissan Patrol
                </h3>

                <div class="details">
                    Dubai • Automatic • 2021
                </div>

                <div
                    class="price"
                    data-aed="175000"
                    data-kes="6350000">
                </div>

                <div class="product-buttons">

                    <button
                        class="btn whatsapp"
                        onclick="orderWhatsApp('Nissan Patrol')">
                        WhatsApp
                    </button>

                </div>

            </div>

        </article>


    </div>

</section>


<!-- REAL ESTATE -->

<section class="section" id="realestate">

    <div class="section-title">

        <div>

            <h2>🏠 Real Estate</h2>

            <p class="muted">
                Homes and property listings
            </p>

        </div>

    </div>


    <div class="products">


        <article class="product">

            <div class="product-image">

                🏢

                <span class="badge">
                    PROPERTY
                </span>

            </div>

            <div class="product-info">

                <h3>
                    Modern 1-Bedroom Apartment
                </h3>

                <div class="details">
                    Dubai Marina • 1 bed • 2 bath
                </div>

                <div
                    class="price"
                    data-aed="1250000"
                    data-kes="45250000">
                </div>

                <div class="product-buttons">

                    <button
                        class="btn whatsapp"
                        onclick="orderWhatsApp('Modern 1-Bedroom Apartment')">
                        Enquire
                    </button>

                </div>

            </div>

        </article>


        <article class="product">

            <div class="product-image">

                🏡

                <span class="badge">
                    PROPERTY
                </span>

            </div>

            <div class="product-info">

                <h3>
                    Family Villa
                </h3>

                <div class="details">
                    Nairobi • 4 bed • 4 bath
                </div>

                <div
                    class="price"
                    data-aed="2100000"
                    data-kes="76000000">
                </div>

                <div class="product-buttons">

                    <button
                        class="btn whatsapp"
                        onclick="orderWhatsApp('Family Villa')">
                        Enquire
                    </button>

                </div>

            </div>

        </article>


    </div>

</section>


<!-- SELL -->

<section class="section">

    <div class="sell-box">

        <div>

            <h2>
                Sell on E World
            </h2>

            <p class="muted">
                Have a phone, car, accessory or property to sell?
                Contact us and we can publish your listing.
            </p>

            <div class="contact-buttons">

                <button
                    class="btn whatsapp"
                    onclick="orderWhatsApp('I want to sell an item on E World')">

                    💬 WhatsApp to List

                </button>

                <button
                    class="btn buy"
                    onclick="callNumber('+971544702455')">

                    📞 Call Us

                </button>

            </div>

        </div>


        <div>

            <h3>
                Payment Options
            </h3>

            <div class="payment-list">

                <span class="payment">
                    💳 Card
                </span>

                <span class="payment">
                    🏦 Bank Transfer
                </span>

                <span class="payment">
                    💬 WhatsApp Order
                </span>

            </div>

            <p class="muted" style="font-size:12px;margin-top:15px">
                Card payments require a payment gateway or merchant account
                before live transactions can be processed.
            </p>

        </div>

    </div>

</section>

</main>


<!-- FOOTER -->

<footer>

    <div class="footer-grid">

        <div>

            <div class="footer-logo">
                E<span>World</span>
            </div>

            <p>
                Phones • Cars • Real Estate • Accessories
            </p>

            <p>
                Your marketplace connecting buyers and sellers.
            </p>

        </div>


        <div>

            <h3>
                Contact
            </h3>

            <p>
                +971 54 470 2455
            </p>

            <p>
                +971 54 387 8294
            </p>

            <p>
                +254 700 835 858
            </p>

        </div>


        <div>

            <h3>
                Payments
            </h3>

            <p>
                Card
            </p>

            <p>
                Bank Transfer
            </p>

            <p>
                WhatsApp Orders
            </p>

        </div>

    </div>


    <div class="copyright">

        © 2026 E World. All rights reserved.

    </div>

</footer>


<script>

/* =========================
   E WORLD JAVASCRIPT
========================= */

let currency = "AED";


/* CURRENCY */

function money(aed,kes){

    if(currency === "AED"){

        return "AED " +
        Number(aed).toLocaleString();

    }

    return "KSh " +
    Number(kes).toLocaleString();

}


function updatePrices(){

    document
    .querySelectorAll("[data-aed]")
    .forEach(function(element){

        const aed =
        element.getAttribute("data-aed");

        const kes =
        element.getAttribute("data-kes");

        element.textContent =
        money(aed,kes);

    });

}


function changeCurrency(){

    if(currency === "AED"){

        currency = "KES";

        document
        .getElementById("currencyButton")
        .textContent = "KSh";

    }else{

        currency = "AED";

        document
        .getElementById("currencyButton")
        .textContent = "AED د.إ";

    }

    updatePrices();

}


/* WHATSAPP */

function orderWhatsApp(item){

    const phone =
    "971544702455";

    const message =
    "Hello E World 👋%0A%0A" +
    "I am interested in: " +
    item +
    "%0A%0APlease send me more details.";

    window.open(
        "https://wa.me/" +
        phone +
        "?text=" +
        message,
        "_blank"
    );

}


/* CALL */

function callNumber(number){

    window.location.href =
    "tel:" + number;

}


/* BUY */

function buyProduct(product){

    alert(
        "Thank you for choosing E World!%0A%0A" +
        product +
        "%0A%0A" +
        "For now, please complete your order through WhatsApp. " +
        "Live card checkout can be connected later."
    );

    orderWhatsApp(product);

}


/* CART */

function showCart(){

    alert(
        "Your E World cart is ready!%0A%0A" +
        "For orders, please use WhatsApp."
    );

}


/* SEARCH */

document
.getElementById("search")
.addEventListener("input",function(){

    const search =
    this.value.toLowerCase().trim();

    const products =
    document.querySelectorAll(
        "#phoneProducts .product"
    );

    let found = false;

    products.forEach(function(product){

        const text =
        product
        .getAttribute("data-search")
        .toLowerCase();

        if(text.includes(search)){

            product.style.display =
            "block";

            found = true;

        }else{

            product.style.display =
            "none";

        }

    });


    document
    .getElementById("noResults")
    .style.display =
    found ? "none" : "block";

});


/* START */

updatePrices();

</script>

</body>
</html>