# Blockchain -Basic-

**블록**들이 **체인**으로 연결된 것이자 **데이터 분산 처리** 기술, 네트워크에 참여하는 
모든 사용자가 모든 거래 내역 등의 데이터를 **분산**, **저장**하는 **P2P** 방식의 기술

## How it works & Advantage ?

1. 네트워크에 참여하는 **모든 사용자**가 해시값으로 연결된 블록체인 장부를 가지고 있게 됨

    → **탈중앙화**(decentralization)

2. **모든 사용자가 장부를 가지고 있고** 확인 할 수 있음

    → **투명성**(Transparency), **추적가능성**(Traceability)

3. 블록체인(장부)에 기록 된 정보는 **변경이 불가능하고 계속 남아있음**

    → **불변성**(Immutability)

4. 블록체인의 거래 내역이 공개 장부에 기록되어 모두가 볼 수 있다고 하더라도

    **거래 당사자들의 신원은 드러나지 않음**

    → **익명성**(Anonymity)

---

## BlockChain Structure

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/84dd8350-843c-4722-a0ec-a4f4a3bb90de/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/84dd8350-843c-4722-a0ec-a4f4a3bb90de/Untitled.png)

[https://medium.com/@kimjunyong/블록체인의-정의와-기술-비전공자도-이해하는-기본적-이해-6706ebb43009](https://medium.com/@kimjunyong/%EB%B8%94%EB%A1%9D%EC%B2%B4%EC%9D%B8%EC%9D%98-%EC%A0%95%EC%9D%98%EC%99%80-%EA%B8%B0%EC%88%A0-%EB%B9%84%EC%A0%84%EA%B3%B5%EC%9E%90%EB%8F%84-%EC%9D%B4%ED%95%B4%ED%95%98%EB%8A%94-%EA%B8%B0%EB%B3%B8%EC%A0%81-%EC%9D%B4%ED%95%B4-6706ebb43009)

- **Header**
    - **Hash of the block**

        블록의 해시값이 담긴 곳

        [**what is Hash?**](https://www.notion.so/Hash-Function-69ec2a95ccf6410a80d34ca12328f8f0)

    - **version**

        해당 블록의 버전입니다. 현재 이 블록 헤더를 만든 비트코인 프로그램의 버전 정보

    - **Previous block Hash**

        묶여있는 블록에서 앞 블록의 주소값

    - **Merkle Rude**

        '머클 루트'는 블록의 바디 부분에 저장된 트랜잭션(거래 정보) 들의 해시 트리

    - **Nonce**

        블록을 만드는 과정에서 해시 값을 구할 때 필요한 재료 역할을 수행

    - **Time**

        대략적인 생성 시간을 의미

    - **bits**, **target**

        난이도 해시 목표 값을 의미하는 지표

- **Body**
    - **거래 카운트**

    - **Transaction**

        데이터베이스의 상태를 변환시키는 하나의 논리적 기능을 수행하기 위한 작업의 단위 또는 한꺼번에 모두 수행되어야 할 일련의 연산들을 의미

---

## Type of BlockChain

- Public blockchain

    ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fb5ce009-adf7-494f-b7da-caec20618cd8/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fb5ce009-adf7-494f-b7da-caec20618cd8/Untitled.png)

    TokenPost, [https://wooaoe.tistory.com/19](https://wooaoe.tistory.com/19)

    거래 내역뿐만 아니라 네트워크에서 이루어지는 여러 행동(Actions)이 다 공유되어 추적이 

    가능한 블록체인

- Private blockchain

    ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/78e1d395-c097-480d-85ff-a0672f0b2efc/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/78e1d395-c097-480d-85ff-a0672f0b2efc/Untitled.png)

    TokenPost, [https://wooaoe.tistory.com/19](https://wooaoe.tistory.com/19)

    허가된 참여자 외 거래 내역과 여러 행동(Actions)은 공유되지 않고 추적이 불가능하다. 프라이빗 블록체인 네트워크에 참여하기 위해 한 명의 주체로부터 허가된 참여자만 참여하여 블록을 생성할 수 있다.

- Consortium

    ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/93d7bf91-e209-4a30-914e-6cc81bb7c449/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/93d7bf91-e209-4a30-914e-6cc81bb7c449/Untitled.png)

    TokenPost, [https://wooaoe.tistory.com/19](https://wooaoe.tistory.com/19)

    컨소지엄 블록체인은 기업 연합형 블록체인으로 이해하면 쉽다. 네트워크에 허가된 여러 참여자가 구성하여 블록을 생성할 수 있다. ex) Hyperledger Fabric