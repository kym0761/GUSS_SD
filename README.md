# GUSS_SD
 
설계 -> 견적 -> 발주 3단계를 거쳐 PO(Purchase Order)가 나온다.

PO가 나오면 납품 일정을 우리가 맞춰준다.

# 납품 일정의 중요한 3가지

1. 자재 내역
2. 납품일
3. 설치 위치

발주 이후에, 제작과 납품 일정, 반입을 위한 측정 등의 절차를 동시에 한다.

순서대로 하는 것 아니다. 순서대로 하면 시간이 부족하다.

# 납품 일정 절차 Phase

## Phase 1 : PO

PO는 삼성 전자와 영업이 가격 조율이나 자재 개수 등의 정보가 오가는 것이다.

우리가 해주어야 할 것은

1. 수량, 자재 종류가 맞는지 확인하기

```
스마트 드라이버 -> RACK, Base & Controller & io8포트 & io48포트

RACK은 Full(42u), Half(22u)

사업장 지역별로 Base의 사이즈가 정해져있다. 이 정보는 시트 어딘가에 있으니 확인하고 정리할 것

사이즈 종류 -> 250mm, 300mm, 600mm
```
| Base Height | Size(mm) |
| --- | --- |
| Infra | 250 |
| Memory | 300 |
| 인프라복합동 | 250(None A/F) or 600 |

2. 일정 맞추기
```
PO가 나오면 납품 요청일을 확인한다. 참고로 납품 요청일은 PO가 나오고 3개월 이후다. (!이내가 아니다. 이후다!)

모든 일정은 납품 요청일을 기준으로 RACK 제작, 검수(FAT) 날짜, 정위치 마킹 날짜, 정위치 인증(5D안착인증) 날짜가 잡힌다.

정위치 마킹과 인증을 하면서 반입구와 동선도 체크해야한다. -> 동선이나 반입구 사용이 불가능하다면 대안책이 될 동선도 만들어야한다.

반입구 사용날이 확정되면, 그 날이 납품 날짜다.(반입구 쓴다 == 제품 넣어준다.)

납품 날짜가 잡히면, 도비업체(ㅇㅈㅎㅇㅌㅋ)와 제작업체(ㅅㅅㅇ)에게 다 날짜 정보가 전달되어야한다.

FAT(우리 회사 FAT, 고객사 FAT)도 해야한다. FAT는 납품 날짜 2일전에는 끝내놔야한다. FAT 일정은 변경되면 안된다.

고객사 FAT는 날짜는 확정하지만, 참석 여부는 물어본다.(다른날 하시죠 ㄴㄴ; 못오면 그냥 우리가 알아서 진행한다는 의미.)

고객의 요구나 협력사, 도비업체의 사정으로 인해 납품 날짜가 변경되어야 한다면, 다른 업체 모두에게 해당 정보를 다 전달해주어야한다.
```

3. 2D 도면(위치) & 5D

```
이거 없으면, 우리가 애초에 설치하지 못한다.

위에서도 설명했지만, 도면 정보를 토대로 정위치를 잡으러 현장 답사를 갔을 때, 반입구와 동선 체크 해야한다.

2d 도면 정보는 최대한 빨리 받고, 원래는 담당자가 동행하면서 정위치 인증은 도면 가져와서 해주는 것이 맞다.

동행을 안하거나 불가능하면, 최소한 (ㅎㄹ) 등의 인증 업체에게 고객사에게 인증받았다 전달해달라 해야함.
```

## Phase 2 : 일정 (디테일하게)

납품 요청일이 확정되면, 우리는 총 3차에 걸쳐 일정을 조율한다? -> 보통은 최대 3차까지 진행했었다. 꼭 3차까지 가진 않음. 더 늘을 수도 있지만, 덜할 수도 있음.

```
예시로 우리가 10월 28일에 고객이 납품 요청일을 잡았다하자. (그럼 당연히 PO가 7월 28일일 것이다. PO 발행 후 3개월)

1. ㅅㅅㅇ과 메일을 주고 받는다. -> 굿어스 7월 29일 RACK 발주 확인... S_ _ 의 담당자 (PJW 대리)에게 RACK 납품 가능 일자를 확인한다.
보통은 1달이라고 하지만, 안지켜진다. 그러니 우리는 1개월 반이라고 늘 생각한다.
주기적으로 확인을 계속 해야한다. 전화 계속



2. RACK 정보 확인 시, ㅅㅅㅇ에게 재고가 있는지, 언제 완성이 되는지, 언제부터 제작할 수 있는지를 확인한다.
보통은, 20개까지는 한번에 제작을 해줄 수 있다. 그렇게 ㅅㅅㅇ에서 제작을 끝내면 출하검사까지 진행하고나서 우리 회사 FAT, 고객 FAT 일정이 정해진다.
-> ㅅㅅㅇ에게 물어보고 납품 일정 조율을 요청 받으면, 고객사에게도 해당 내용을 전달하고, 납품일이 변경되면 위에서 말한대로 납품 조율을 통으로 다시한다.
1차..2차...3차...

```
위 절차가 끝났다면?

```
삼성에게 2d 도면을 받았다고 가정하자. 도면 정보는 테라타워가서 확인할 수 있음.

1. 현장 마킹 일정을 잡는다. -> 그리고 당연히 마킹을 한다!

2. 5D 안착 인증(정위치 인증)을 받는다.
정위치 인증 담당은, 마스터 시트의 유지보수업체 서브 시트를 보면 연락처와 업무에 "정위치" 라고 된 사람들이다.
사업체명 확인? 양식을 전달? ->이거 담당자마다 다르다 ㅇㅅㅇ;
정위치 인증을 실패하면, 그 자리에서 다시 하든지, 아니면 다른 곳 업무를 보고 다시 와달라고 해야한다.
생각해보면, 다음날하겠다든지 다른 날에 다시 하겠다하면, 이 정위치 인증 하나 때문에 거리가 먼 사업장까지 와야한다.
예시) 평택 정위치 인증 실패해서 다음날 다시 하겠다하면 다음날 넌 평택 사업장에 다시 와야한다!

도비업체에도 납품 예정 일자에 납품이 가능한지를 확인할 것! -> 가능한 날, 인원 수 등등 정보를 확인하면서 일정 조율해야한다.

어느 하나라도 정보가 바뀌면 모두에게 내용 통보해야한다.

도비업체(양중업체)에게 반입담당인원을 받는다. ->ㅇㅈㅎㅇㅌㅋ에서 LGS과장 -> 정보를 받으면 내방신청하기
우리가 하기도 하고, 도비업체에서 직접하기도 한다. 그래도, 이 인원 정보를 우리가 검토해야할 필요가 있다.

```

### FAT 및 Setup

납품할 기기 셋업하기

전자의 FAT까지 하고 난 뒤, 끝나면 초기화 작업까지 하는 것이 우리의 업무다.

초기화할 때 필요한 정보들이 있다.
일단 이 작업을 하기 전에 도면이 나올 때 RACK 번호가 부여되어야하는 점을 명심해야한다.

필요한 정보는
1. 판넬명, node 번호, ip -> 예시) 2FSMCS-Y123, NODE 22123-1, ip XXX.XXX.XXX.XXX

참고로 ip는 가스트론에게 전달받는다. 

```
->?? 전자에서 발주가 들어오면, 2d 도면에 정보가 있는데(rack 등) 이 정보를 기반으로, 가스트론에게 메일이나 전화해서 해당 랙 들어가는데, 노드번호와 ip를 주십쇼.
해당 담당자 마스터 시트 안에 있음. 라인별 담당자도 있고.

화성향은 세한이라는 업체, IP는 장기처 프로?
여기서 못받으면, 삼성 구매 담당자에게 이 정보를 받을 수 있게 요청해야함.

```

ip : XXX.XXX.XXX.XXX을 받게 되고, 설정에서 gateway IP를 지정할 때 받은 IP를 기준으로 XXX.XXX.XXX.1 이다.

최소한 우리는, FAT를 하기 전에 일주일 전에는 IP정보를 얻어서 FAT를 진행해야한다. -> FAT 전날에 받으려고 했다가는 FAT 끝나고 초기화 작업을 못함.

FAT가 끝나면, 제조사에게 전원을 내리고 패킹하라고 요청한다.
또한, ㅅㅅㅇ&삼성전자에 판넬안내문도 전달해야함(양식은 공유 드라이버 안에 존재함)
->SD RACK 관리번호, 관리부서&담당자, 시공부서&담당자, 시공업체&담당자... 내용 있는 판넬안내문

설치했는데, 판넬안내문에 오타를 발견했다? -> 틀렸다면 나중에 다시 사업장을 와서라도 내용을 고쳐야한다..

### FAT 기능 검사 내용

~~ 나중에


### 초기화 업무

리눅스 명령어로 초기화한다.

IO48포트든, IO8포트든 연결해서 nginx 웹페이지 들어갈 수 있음

리눅스 접근용 클라이언트로 콘솔 접근 가능함(putty 비추, MobaXterm 추천)

명령어는, 보안 이슈로 현재 쓰지 않겠음.

1. ip 및 노드 & Location 정보 세팅

2. 로그 파일 삭제 및 폴더 초기화, 서비스 중인 프로그램 stop 및 disable 등등

참고로 지금 위는 순서 지켜야함. 2번 먼저하면 1번을 세팅할 수 없다. 서비스 중인 프로그램을 stop 시켰기 때문에 nginx 웹페이지를 못들어감.

접근 권한 때문에 sudo 사용해야 한다는 점, 쉘스크립트 만들어서 사용했다면 그 쉘스크립트도 마지막에 삭제해야하는 게 유의사항.


## Phase 3 : 납품 및 마무리?

1. 영업에게 인보이스 전달 요청한다.
2. ㅇㅈㅎㅇㅌㅋ, ㅅㅅㅇ에게 인보이스가 간다.
3. 검품장가서 인보이스에 도장을 받는다.
4. 반입구 도착 및 하차
5. 정위치 전달 및 앙카볼트 작업
6. 설치 완료 및 사진 촬영 & 인보이스 사인 받기
7. 끝!

설치 촬영한 사진 내용으로 완료보고서를 쓴다.
자재 내역
기둥 번호가 보이는 설치 위치 확인 가능한 사진
1. 문 닫고 정면
2. 문 열고 정면
3. 문 닫고 후면
4. 문 열고 후면
5. 측면

# SOP와 TBM

SOP와 TBM 문서 참고해서 채울 예정

# 기타?

전원 공급 요청-> 애매하다. 다만, 우리가 확인은 해야한다. 그러나, 우리 작업은 IP 및 기기 초기화까지고, 납품하고 나서부터의 관리는 ㄱㅅㅌㄹ의 업무다.
확인하게 된다면 언제 전원 공급을 하는지 알아보고 스탠바이 하면 되지만, 굳이 할 필요는 없다.

SET UP 단계서 우리는 3가지만 한다.

1. NODE 부여
2. IP 부여
3. SET UP

통신 프로그램 가동은 우리가 하지 않는다.

# 팁?

크로스체크 잊지말자

ㅇㅇㅅ 대리와 함께 잘 협업하자

시간이 부족하다는 점 명심

PM님과 이슈 정보 공유가 필요하다.

프로세스 구성도?

테라 사무실 컴퓨터에 SDS에 받아놓은 프로세스 구성도?

못가져온다. 테라 가게되면, 프로세스 구성도라는 문서를 보자.

일정표 마스터시트에 10 25기준 내가 해야할 일들 써져있음 참고할 것
