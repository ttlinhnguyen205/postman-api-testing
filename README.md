# Báo cáo thực hành Postman

# 1. Giới thiệu

Postman là công cụ dùng để kiểm thử API, hỗ trợ gửi request và nhận response từ server.  
Trong bài thực hành này, em đã sử dụng Postman để thực hiện các phương thức cơ bản của REST API gồm:

- GET
- POST
- PUT
- DELETE

API sử dụng trong bài thực hành:

https://jsonplaceholder.typicode.com/

---

# 2. GET Request

## Mục đích
Dùng để lấy dữ liệu từ server.

## URL

```text
https://jsonplaceholder.typicode.com/posts
```

## Phương thức

```text
GET
```

## Kết quả

Request trả về danh sách bài viết dưới dạng JSON và trạng thái:

```text
200 OK
```

## Hình minh họa



---

# 3. POST Request

## Mục đích

Dùng để tạo dữ liệu mới trên server.

## URL

```text
https://jsonplaceholder.typicode.com/posts
```

## Phương thức

```text
POST
```

## Body JSON

```json
{
  "title": "Hello",
  "body": "Testing Postman",
  "userId": 1
}
```

## Kết quả

Request tạo dữ liệu thành công và trả về:

```text
201 Created
```

## Response JSON

```json
{
  "title": "Hello",
  "body": "Testing Postman",
  "userId": 1,
  "id": 101
}
```

## Hình minh họa


---

# 4. PUT Request

## Mục đích

Dùng để cập nhật dữ liệu trên server.

## URL

```text
https://jsonplaceholder.typicode.com/posts/1
```

## Phương thức

```text
PUT
```

## Body JSON

```json
{
  "id": 1,
  "title": "Updated Title",
  "body": "Updated content",
  "userId": 1
}
```

## Kết quả

Request cập nhật dữ liệu thành công và trả về:

```text
200 OK
```

## Response JSON

```json
{
  "id": 1,
  "title": "Updated Title",
  "body": "Updated content",
  "userId": 1
}
```

## Hình minh họa


---

# 5. DELETE Request

## Mục đích

Dùng để xóa dữ liệu trên server.

## URL

```text
https://jsonplaceholder.typicode.com/posts/1
```

## Phương thức

```text
DELETE
```

## Kết quả

Request xóa dữ liệu thành công và trả về:

```text
200 OK
```

## Response JSON

```json
{}
```

## Hình minh họa


---

# 6. Kết luận

Qua bài thực hành, em đã:

- Hiểu được cách hoạt động của API
- Sử dụng Postman để kiểm thử API
- Thực hiện thành công các phương thức:
  - GET
  - POST
  - PUT
  - DELETE
- Hiểu cách gửi request và nhận response dạng JSON

Bài thực hành giúp em làm quen với quá trình kiểm thử API trong phát triển phần mềm.