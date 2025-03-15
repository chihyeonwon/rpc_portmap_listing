# rpc_portmap_listing
rpc_portmap_listing

본 글은 RPC Portmap Listing UDP 111 포트로 들어오는 공격에 대한 글입니다.
정보 수집 Information Scan 스캔성 공격의 일종으로 대상 컴퓨터에 해킹하기 위해 대상 컴퓨터가 RPC의 어떤 포트를 Open 하여 서비스하는 지를 알아내는 방법입니다.패킷에서 tcp를 분석
분석한 TCP Header를 봤을 때 RPC 가 서비스 중이라면 CALL 프로토콜이 4 이고 2면 rpc service로 판단한다.
공격자가 보내는 패킷의 횟수를 카운트해 인정 시간 내에 임계치에 해당하는 횟수이면 rpc port map listing Attack 으로 간주.
불필요한 서비스 포트를 disabled 사용 하지 않음으로써 공격의 피해를 최소화 할 수 있다.
