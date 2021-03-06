참고자료: [HTTP request methods | MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)

# What are HTTP request methods?

HTTP는 다양한 종류의 **요청 메서드**를 통해 특정 resource에 대해 어떤 action이 취해져야 하는지를 알린다

대표적으로 GET, POST, PUT, DELETE가 있음

### GET

서버에 **특정 resource의 representation**을 요청한다. GET 요청은 데이터를 요청하는 용도로만 사용되어야 한다

데이터를 담고 있으면 안 됨

GET 요청의 body에 데이터(payload)를 담아 보내는 방식이 specification 수준에서 금지된 것은 아니나, semantic하지 않음.

몇몇 서비스에서는 body가 포함된 GET 요청을 거부하기도 함

_Request has body: false_
_Successful response has body: true_

### POST

서버에 데이터를 **보낸다**.

POST 요청 body의 유형은 **Content-Type** 헤더에 의해 indicate됨

POST와 PUT의 차이: PUT 요청은 연달아 하더라도 동일한 결과가 발생 (side-effect 없음), POST 요청은 연달아 할 경우 특정 명령을 수차례 적용한 것과 같이 추가적인 결과가 발생

일반적으로 **HTML form**에서 활용됨

_Request has body: true_
_Successful response has body: true_

### PUT

새로운 resource를 생성하거나, 대상 resource가 있을 경우 representation을 요청의 payload로 대체

_Request has body: true_
_Successful reponse has body: false_

### DELETE

특정 resource를 삭제

_Request has body: maybe_
_Successful reponse has body: maybe_

### OPTIONS

특정 URL 혹은 서버에 permitted communication options를 요청

client는 OPTIONS 메서드를 활용해 URL을 특정할 수 있으며, 별표(\*)를 이용하면 전체 서버를 대상으로도 할 수 있음

> **_CORS 설정과 연관된 메서드_**

_Request has body: false_
_Successful response has body: true_
