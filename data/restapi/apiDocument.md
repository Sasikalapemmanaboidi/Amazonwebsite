//live link
https://amazonnodeapi.herokuapp.com


//page1
//list of categories
https://amazonnodeapi.herokuapp.com/category
>>>http://localhost:7900/category



//page2
//products as per categories
https://amazonnodeapi.herokuapp.com/getProducts/?category_id=4
>>>http://localhost:7900/getProducts/?category_id=4

//API for cost filter:
https://amazonnodeapi.herokuapp.com/filter/1?lcost=200&hcost=500
>>>http://localhost:7900/filter/1?lcost=200&hcost=500

//pagination:
https://amazonnodeapi.herokuapp.com/filter/1?lcost=100&hcost=1000&skip=0&limit=2
>>>http://localhost:7900/filter/12?lcost=100&hcost=1000&skip=0&limit=2
//Sort Low to High:
https://amazonnodeapi.herokuapp.com/filter/2?lcost=100&hcost=1000&sort=1
>>>http://localhost:7900/filter/7?lcost=100&hcost=1500&sort=1

//page3
//details of products and menu wrt categories
https://amazonnodeapi.herokuapp.com/productDetails/8
>>>http://localhost:7900/productDetails/8


//menuproducts wrt categories
https://amazonnodeapi.herokuapp.com/menu/1
>>>http://localhost:7900/menu/1


//page4
//place order(post)
>>>localhost:7900/placeorder
{
    "name" : "sudha",
    "email" : "sudha@gmail.com",
    "address" : "dno:4-348, ramalayam street, Madhavapatnam",
    "phone" : 6309900021,
    "cost" : 1500,
    "menuItem" :[31,55,71],
    "status" : "pending"
}



//view order(get)
https://amazonnodeapi.herokuapp.com/vieworders?email=sashikala@gmail.com
>>>localhost:7900/vieworders?email=sashikala@gmail.com


//menu on basis of user selection (id)
>>>localhost:7900/menuItem

[51,42,31]

[
    {
        "_id": "62506c8abedb89d7859d009c",
        "id": 31,
        "name": "Makeup Brushes",
        "category_id": 6,
        "category": "Cosmetics",
        "img": "https://ibb.co/BZ03LxL",
        "description": "Different sizes of makeup brushes with box kit",
        "price": 1800,
        "rating": 4.2
    },
    {
        "_id": "62506c8abedb89d7859d00a7",
        "id": 42,
        "name": "Birthday lighting kit",
        "category_id": 9,
        "category": "lighting decoration",
        "img": "https://ibb.co/642W7pG",
        "description": "Happy birthday lighting decorative kit",
        "price": 1200,
        "rating": 4.5
    },
    {
        "_id": "62506c8abedb89d7859d00b2",
        "id": 51,
        "name": "Duck Toys",
        "category_id": 12,
        "category": "Baby kits & toys",
        "img": "https://ibb.co/4fJHcLh",
        "description": "yellow colour duck toys for lower prices ",
        "price": 250,
        "rating": 4.2
    }
]


//delete order
>>>localhost:7900/deleteorder


//update order
>>>localhost:7900/updateorder/625853241540acb7c299535b
{
    
            "status": "In Transit",
            "bank_name":"SBI",
            "bank_status": "transferred money"
}