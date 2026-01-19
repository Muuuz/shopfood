<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Shop</title>
     
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        * {
            box-sizing: border-box;    
            font-family: Arial, sans-serif;
        }
         
        body {
            margin: 0;                
            background: rgb(238, 187, 110);
        }
        
        .header {
            background:  #181616;
            color: rgb(240, 184, 101);
            text-align: center;
            padding: 20px;
            font-size: 40px;
            font-weight: bold;
        }
        
        .nav {
            background: #e08a3a;
            padding: 10px;
            display: flex;
            flex-wrap: wrap;
            align-items: center;
            gap: 10px;
        }
        
        .nav button {
            background: rgb(255, 255, 255);
            border: none;
            color: rgb(0, 0, 0);
            padding: 10px 20px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 16px;
        }
         
        .nav input {
            margin-left: auto;           
            padding: 8px 15px;
            border-radius: 20px;
            border: none;
            font-size: 16px;
        }
         
        .content {
            padding: 20px;
        }

        h2 {
            margin-bottom: 20px;
        }
        
        .section-title {
            font-size: 36px;
            font-weight: bold;
            margin: 30px 0;
        }
        
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 30px;
        }
        
        .card {
    background: white;
    border-radius: 24px;
    padding: 15px;
    transition: transform 0.25s ease, box-shadow 0.25s ease;
}


.name-price {
    display: flex;                 
    justify-content: space-between;
    align-items: center;
    margin-top: 10px;
}

.name {
    font-size: 16px;
    font-weight: 600;
}

.price {
    font-size: 16px;
    font-weight: bold;
    color: #e08a3a;
}

.img-box {
    height: 140px;
    border-radius: 20px;
    overflow: hidden;      
}
          
        .img-box {
            background: #00a8e8;
            height: 140px;
            border-radius: 30px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
        }
        
        .img-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;     
            border-radius: 30px;
        }
        
        .card:hover {
    transform: translateY(-6px);
    box-shadow: 0 18px 35px rgba(0,0,0,0.18);
}

        .footer {
    width: auto;
    background: #636262; 
    color: #ffffff;
    text-align: center;

    padding: 20px 10px;

    font-size: clamp(14px, 1.2vw, 18px);

    box-sizing: border-box;
    
        }
    </style>
</head>

<body>
    
    <div class="header">Shop</div>
    
    <div class="nav">
        <button onclick="filterCategory('all')">Home</button>
<button onclick="filterCategory('ramen')">Ramen</button>
<button onclick="filterCategory('soup')">Soup</button>
<button onclick="filterCategory('snack')">Snack</button>
<button onclick="filterCategory('drink')">Drink</button>
        <input type="text" placeholder="search ">
    </div>
    
    <div class="content">
        <h2>Most popular Food</h2>
                      
                       <div class="grid">
        <div class="card" data-category="ramen">                 
    <div class="img-box">          
        <img src="ramen-sausage.jpg" alt="Ramen">
    </div>

    <div class="name-price">       
        <span class="name">Spicy Ramen with sausage</span>
        <span class="price">$5.50</span>
    </div>
</div>
            <div class="card" data-category="ramen">                 
    <div class="img-box">          
        <img src="fried-rice.jpg" alt="Ramen">
    </div>

    <div class="name-price">       
        <span class="name">Fried rice</span>
        <span class="price">$2.50</span>
    </div>
</div>
                <div class="card" data-category="snack">                 
    <div class="img-box">          
        <img src="pancake.jpg" alt="snack">
    </div>

    <div class="name-price">       
        <span class="name">pan cake</span>
        <span class="price">$2.50</span>
    </div>
</div>
              
<div class="card" data-category="snack">                 
    <div class="img-box">          
        <img src="Patti-Samosa.jpg" alt="snack">
    </div>

    <div class="name-price">       
        <span class="name">Patti Samosa</span>
        <span class="price">$2.50</span>
    </div>
</div>
</div>

        <div class="section-title">Eazy take away</div>
       

        <div class="grid">
            <div class="card" data-category="ramen">
                <div class="img-box">
    <img src="ramen-eng.jpg"  alt="ramen">
</div>
                <div class="name-price">       
        <span class="name">Spicy Ramen with egg</span>
        <span class="price">$3.50</span>
    </div>
            </div>

            <div class="card" data-category="ramen">
                <div class="img-box">
    <img src="ramencutlet.jpg" alt="ramen">
</div>
                <div class="name-price">       
        <span class="name">Spicy Ramen with pork cutlet</span>
        <span class="price">$5.50</span>
    </div>
               
            </div>

            <div class="card" data-category="soup">
                <div class="img-box">
    <img src="Tom-yum.jpg" alt="Soup">
</div>
                <div class="name-price">       
        <span class="name">Tom yum</span>
        <span class="price">$1.50</span>
    </div>
               
            </div>

            <div class="card" data-category="snack">
                <div class="img-box">
    <img src="Veg-Spring-Rolls.jpg" alt="Snack">
</div>
                <div class="name-price">      
        <span class="name">Veg Spring Rolls</span>
        <span class="price">$2.00</span>
    </div>
               
            </div>

            <div class="card" data-category="drink">
                <div class="img-box">
    <img src="Chocolate-Chip-Frappuccino.jpg" alt="Drink">
</div>
                <div class="name-price">       
        <span class="name">Chocolate Chip Frappuccino</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>
            
            <div class="card" data-category="drink">
                <div class="img-box">
    <img src="coffee.jpg" alt="Drink">
</div>
                <div class="name-price">       
        <span class="name">Coffee</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>
            
            <div class="card" data-category="drink">
                <div class="img-box">
    <img src="coca.jpg" alt="Drink">
</div>
                <div class="name-price">       
        <span class="name">Coca cola</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>

            <div class="card" data-category="drink">
                <div class="img-box">
    <img src="macha.jpg" alt="Drink">
</div>
                <div class="name-price">       
        <span class="name">Macha</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>

            <div class="card" data-category="soup">
                <div class="img-box">
    <img src="chicken-broth.jpg" alt="soup">
</div>
                <div class="name-price">       
        <span class="name">chicken broth</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>

            <div class="card" data-category="snack">
                <div class="img-box">
    <img src="Churro-Bugles" alt="snack">
</div>
                <div class="name-price">       
        <span class="name">Churro Bugles</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>

            <div class="card" data-category="soup">
                <div class="img-box">
    <img src="Miso-Soup.jpg" alt="soup">
</div>
                <div class="name-price">       
        <span class="name">Miso Soup</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>

            <div class="card" data-category="ramen">
                <div class="img-box">
    <img src="stir-fried-udon-noodles.jpg" alt="ramen">
</div>
                <div class="name-price">       
        <span class="name">stir fried udon</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>

            <div class="card" data-category="snack">
                <div class="img-box">
    <img src="snack-mix.jpg" alt="snack">
</div>
                <div class="name-price">       
        <span class="name">snack-mix</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>

            <div class="card" data-category="ramen">
                <div class="img-box">
    <img src="korain-nodle.jpg" alt="ramen">
</div>
                <div class="name-price">       
        <span class="name">korain nodle</span>
        <span class="price">$2.50</span>
    </div>
               
            </div>
            
            <div class="card" data-category="drink">
                <div class="img-box">
    <img src="icewater.jpg" alt="Drink">
</div>
                <div class="name-price">       
        <span class="name">Ice Water</span>
        <span class="price">$0.50</span>
    </div>
                
            </div>
            <div class="card" data-category="soup">
                <div class="img-box">
    <img src="Tom-Yum-Talay.jpg" alt="Soup">
</div>
                <div class="name-price">       
        <span class="name">Tom Yum Talay</span>
        <span class="price">$1.50</span>
    </div>       
            </div>
             <div class="card" data-category="snack">
                <div class="img-box">
    <img src="latia- spicy-gluten-stick.jpg" alt="Snack">
</div>
                <div class="name-price">       
        <span class="name">Latiao Spicy Gluten Stick</span>
        <span class="price">$1.50</span>
    </div>
    
                
        </div>
    </div>
    
    <div class="footer"> © 2026 Mu_testsite. All rights reserved.</div>

</body>
<script>
function filterCategory(category) {
    const cards = document.querySelectorAll('.card');

    cards.forEach(card => {
        const cardCategory = card.dataset.category;

        if (category === 'all' || cardCategory === category) {
            card.style.display = 'block'; 
        } else {
            card.style.display = 'none';  
        }
    });
}
</script>

</html>
