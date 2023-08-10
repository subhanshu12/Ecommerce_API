# Ecommerce Platform API
This is a RESTful API for managing product inventory in an ecommerce platform. It is built using Node.js and MongoDB.

## Getting Started
To get started with the API, follow these steps:

### Prerequisites
- Node.js (version 14 or above)
- MongoDB (Make sure MongoDB is installed and running on your system)

### Installation
1. Clone the repository:
   git clone https://github.com/subhanshu12/Ecommerce_API

2. Navigate to the project directory:
    cd ecommerce-platform-api

3. Install the dependencies:
    npm install

4. Start the API server:
    npm start

The server should now be running at http://localhost:8000

## API Endpoints
- To test the API using Postman:
1. Create a product
URL: POST /products/create
Content-Type: application/json

Example Request:
POST http://localhost:8000/products/create
{
  "name": "laptop",
  "quantity": 10
}
Example Response:
{
  "product": {
    "name": "laptop",
    "quantity": 10,
    "_id": "609f4fbcf6b753001faad7a4",
  }
}

2. List products
URL: GET /products

Example Request:
GET http://localhost:8000/products
{
  "products": [
    {
      "_id": "609f4fbcf6b753001faad7a4",
      "name": "laptop",
      "quantity": 10,
    },
    {
      "_id": "609f4fbcf6b753001faad7a5",
      "name": "camera",
      "quantity": 5,
    },
    {
      "_id": "609f4fbcf6b753001faad7a6",
      "name": "smartwatch",
      "quantity": 8,
    }
  ]
}

3. Delete a product
URL: DELETE /products/:id

Example Request:
DELETE http://localhost:8000/products/609f4fbcf6b753001faad7a4
Example Response:
{
  "message": "Product deleted"
}

4. Update quantity of a product
URL: POST /products/:id/update_quantity/?number=10

Example Request:
POST http://localhost:8000/products/609f4fbcf6b753001faad7a4/update_quantity/?number=10 
Example Response:
{
    "product": {
      "_id": "609f4fbcf6b753001faad7a4",
      "name": "laptop",
      "quantity": 20,
    },
    "message": "Updated successfully"
  }

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License.
<img width="1075" alt="Screenshot 2023-08-10 180918" src="https://github.com/subhanshu12/Ecommerce_API/assets/101986633/fa6fa88f-811b-47a5-b758-e8b43bdad045">
<img width="1072" alt="Screenshot 2023-08-10 180937" src="https://github.com/subhanshu12/Ecommerce_API/assets/101986633/7f8833a5-e889-464a-874f-d54b8ba9c5ee">
<img width="1080" alt="Screenshot 2023-08-10 181056" src="https://github.com/subhanshu12/Ecommerce_API/assets/101986633/3468fb65-5b01-4e50-8404-b344d08ac20f">
<img width="1075" alt="Screenshot 2023-08-10 181131" src="https://github.com/subhanshu12/Ecommerce_API/assets/101986633/44023ead-3d58-4a84-bc68-542c5c479efd">
<img width="1078" alt="Screenshot 2023-08-10 181221" src="https://github.com/subhanshu12/Ecommerce_API/assets/101986633/f13fc6ee-79e4-46d9-a4c3-664f1c267774">
<img width="1074" alt="Screenshot 2023-08-10 181353" src="https://github.com/subhanshu12/Ecommerce_API/assets/101986633/23e4082e-b255-497c-b76b-2f2dd3f547a2">
<img width="1077" alt="Screenshot 2023-08-10 181416" src="https://github.com/subhanshu12/Ecommerce_API/assets/101986633/820b8f65-f8c5-4954-9298-ee4c3922cab9">



By - Subhanshu Tripathi
