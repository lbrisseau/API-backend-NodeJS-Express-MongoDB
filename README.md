# CoursOC-NodeJS-Express-MongoDB

API fonctionelle pour mise en place du CRUD d'un Product avec 5 routes :

# GET: /api/products
Retournera tous les produits sous la forme { products: Product[] }

# GET: /api/products/:id
Retournera le produit avec le_id fourni sous la forme { product: Product }

# POST: /api/products
Créera un nouveau Product dans la base de données.
Le corps de la requête a pour forme :

{
    "name": string,
    "description": string,
    "price": number,
    "inStock": boolean
}

Il retournera le Product ainsi créé (y compris son champ _id ), sous la forme{ product: Product }.

# PUT: /api/products/:id
Modifiera le produit avec le _id fourni selon les données envoyées dans le corps de la requête.
Le corps de la requête a pour forme :

{
    "name": string,
    "description": string,
    "price": number,
    "inStock": boolean
}

Retournera un objet de la forme{ message: 'Modified!' }

# DELETE: /api/products/:id
Supprimera le produit avec le _id fourni.
Retournera un objet de la forme { message: 'Deleted!' }
