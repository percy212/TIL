# __API Server__

## API Server?
Client가 어떤 정보를 원한다고 하자. <br/>
Client는 그 정보가 DB에 있는지 어디에 있는지는 알 바 아니다. <br/>
그냥 그 정보만 받으면 된다. <br/>
그래서 API Server는 Client가 어떤 정보를 요청하면, <br/>
그 정보를 가져와서 Client에게 알려준다. <br/>

### 그래서 왜 씀?
Client에게 '너가 원하는 정보는 이거야'하고 알려주기만 해야지 <br/>
'우리는 모든 정보를 여기에 저장해. 여기서 찾아봐.' <br/>
해선 안되기 때문이다. <br/>
Client가 착한 사람이라면 금고를 열어줘도 상관없겠지만 <br/>
나쁜 사람이라면? <br/>
그렇기 때문에 중간 다리인 API Server가 필요하다. <br/>

## Flask?
API Server를 간단하게 만들 수 있는 파이썬 프레임워크. <br/>
Django를 써보려고 하다가 너무 복잡해서 Flask를 사용했다. <br/>

## HTTP request
GET, POST 등 서버에 요청을 보내는 방식이 여러가지 있다. <br/>
GET은 (/~/userid)처럼 URL을 통해 값을 넘겨준다. <br/>
POST는 HTML Body에 값을 적어서 넘겨준다. <br/>
그래서 GET과 달리 어떤 값을 넘겨주는지 바로 보이지 않는다.

