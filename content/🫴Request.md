As implied by the name, a [request](https://developer.mozilla.org/en-US/docs/Web/API/Request) is a standardized message sent to an [[Endpoint]] _requesting_ to obtain some resources. An example could be a request to obtain all the movies' names from IMDB database.

🍏🍎🍊 There are multiple types of requests. Some of them are:
* POST
* GET
* DELETE
* UPDATE
* OPTIONS
* PUT

The names suggest what we can achieve when sending these requests.🙂

The most common ones are **GET** and **POST**.

|                                         **GET**                                          |                                          **POST**                                          |
| :--------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------: |
|                            request is visible -> less secure                             |                            request is invisible -> more secure                             |
|                           the data that can be sent is limited                           |                             larger amounts of data can be sent                             |
| same request -> same response *(is not supposed to change the state of the application)* | same request -> potentially different response *(can change the state of the application)* |
|                                  is used to _get_ data                                   |          is used to _send_ data and receive the result of the performed operation          |
|                          faster and more efficient, less secure                          |                slowlier, more secure, can send more data of different types                |

### 🛠 How to

#### 🐍 Python

```
import requests

# GET request
r = requests.get("www.example.com/")
r = requests.get("www.example.com/message=mymessage")  # when sending a message as # a key-value pair with "message" as a key and "mymessage" as a value

# POST request
r = requests.post("www.example.com", data={"message": "my message"})
```

⚙️ **Resources:**
* [brief explanation](https://sendbird.com/learn/what-is-an-api-request) ~1min
* [longer explanation](https://www.altexsoft.com/blog/rest-api-design/) ~10min
* [one more explanation](https://blog.uptrends.com/technology/the-anatomy-of-an-api-call/) ~7min
* [conceptual video explanation](https://youtu.be/RkGJ9tKI8s0](https://youtu.be/RkGJ9tKI8s0), ~2min