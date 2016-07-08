
Spring-mongodb-data-rest is my Proof of concept to Connect MongoDB with Java using SpringBoot

In this case I had the Driver mongo inside Maven dependencies and this able to Connect to my Mongo instance.

After this inside STS or Eclipse we can run insideo the IDE or out

Out only with the next statment

mvn Springboot:run

In STS only execute like Spring boot App

After in Postman

http://localhost:8080/products

And the response must be something like this.

{
  "_links": {
    "self": {
      "href": "http://localhost:8080/products{?page,size,sort}",
      "templated": true
    }
  },
  "_embedded": {
    "products": [
      {
        "name": "Glass",
        "title": "Beatiful Glass",
        "description": null,
        "imageUrl": "http://img.com",
        "price": 4.98,
        "_links": {
          "self": {
            "href": "http://localhost:8080/products/564438ed77c8eee4e57999e9"
          }
        }
      },
      {
        "name": "Book",
        "title": "The Martian",
        "description": null,
        "imageUrl": "http://theMartian.com",
        "price": 15.87,
        "_links": {
          "self": {
            "href": "http://localhost:8080/products/56443acf77c8eee4e57999eb"
          }
        }
      },
      {
        "name": "Vocho",
        "title": "Vocho 2016 new generation",
        "description": null,
        "imageUrl": "http://vocho.com",
        "price": 23333.87,
        "_links": {
          "self": {
            "href": "http://localhost:8080/products/572d4f31fbeaf968ca0a495e"
          }
        }
      }
    ]
  },
  "page": {
    "size": 20,
    "totalElements": 3,
    "totalPages": 1,
    "number": 0
  }
}
