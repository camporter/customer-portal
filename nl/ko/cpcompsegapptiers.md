---

copyright:

  years: 1994, 2019

lastupdated: "2019-02-25"

keywords: available hardware firewalls, application tiers, web servers, securing environment, activating firewall 

subcollection: customer-portal

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# 환경 보안 및 스케일링
{: #cp_compsegapptierssecscal}

애플리케이션을 호스팅할 때 모든 시스템 관리자가 고려해야 할 가장 중요한 측면 중 두 가지는 애플리케이션의 보안 및 확장성입니다.
{:shortdesc}

## 방화벽으로 시스템 보안
{: #cp_bpsecuresystem}

사용 가능한 하드웨어 방화벽을 사용하여 디바이스의 보안이 항상 유지되도록 하십시오. 규칙이 올바르게 설정된 경우에는 원하지 않는 활동으로부터 서버를 보호할 수 있도록 작동 중지 시간 없이 요청 시에 하드웨어 방화벽을 프로비저닝할 수 있습니다.

방화벽은 적용하기 위해 수동으로 구성하고 사용으로 설정해야 하는 디바이스에 대한 추가 기능 서비스입니다. 필요하지 않은 포트를 잠그고 사설 네트워크 기반 시스템이 시스템에 대한 외부 접근성을 추가로 관리할 수 있도록 공용 포트를 사용 안함으로 설정할 수 있습니다. 고객 포털의 주기적 취약성 스캔은 위험을 빠르게 완화할 수 있도록 미해결 또는 알 수 없는 보안 위험을 식별합니다.

방화벽을 주문한 후에는 이를 사용해야 하며 규칙을 설정해야 합니다.

### 방화벽 활성화
{: #cp_bpnofirewalbypass}

방화벽 구매는 시스템 보호의 시작이지만, 사용자를 보호하는 것은 아닙니다. 프로비저닝 후 방화벽은 **무시 모드**에 있으며 규칙 세트를 포함하지 않습니다. 방화벽을 시작하고 실행하려면 원하지 않는 활동 차단을 시작할 수 있도록 규칙을 작성하고 방화벽을 활성화해야 합니다.


## 애플리케이션 계층을 세분화하여 환경 보안
{: #cp_copmsecenv}

논리적 애플리케이션 계층을 실제 인프라 계층으로 세분화하면 ACL(Access Control List)을 사용하여 더 강화된 보안을 제공할 수 있습니다. 애플리케이션 계층을 세분화할 때 고려할 가장 중요한 컴포넌트 중 하나는 각 계층에 허용하는 트래픽과 발생 위치입니다. 이 정보를 판별하려면 애플리케이션의 근본적인 작동 방식과 사용자에게 요청한 컨텐츠를 제공하기 위해 서로 의존하는 서비스가 무엇인지에 대해 고려하십시오.

예를 들어, 웹 프론트엔드 및 데이터베이스 백엔드에 의존하는 2계층 애플리케이션이 있다고 가정하십시오. 이 애플리케이션의 경우 포트 80 및 443(SSL을 사용 중인 경우)이 웹 서버의 인터넷에 대해 열려 있는지 확인하십시오. 또한 인터넷에 대한 모든 포트를 잠그고 {{site.data.keyword.BluSoftlayer_full}} 인프라 사설 네트워크를 사용하여 VPN을 통해 서버를 관리하려고 할 수 있습니다. 데이터베이스 서버에서 공인 IP 주소의 바인드를 해제하고 웹 서버의 포트 1433(MSSQL용) 또는 3306({{site.data.keyword.mysql}}용) 전반에서 모든 트래픽을 데이터베이스 서버로 전달하려고 할 수 있습니다. 웹 서버와 같이 사설 네트워크를 통해 데이터베이스 서버를 관리할 수 있습니다. 또한 데이터베이스 서버에 소프트웨어 방화벽을 설정하여 웹 서버에서 특정 데이터베이스 포트로의 모든 트래픽을 잠글 수 있습니다.

이 방식으로 환경을 설정하여 인터넷에서 SSH 또는 RDP에 액세스하지 못하게 하고 데이터베이스에 대한 모든 인터넷 트래픽을 사용 안함으로 설정하여 보안을 향상시킵니다. 웹 계층 및 데이터베이스 계층 간에 ACL을 작성하면 웹 서버가 손상된 경우에 데이터베이스가 쉽게 손상되지 않습니다.

## 애플리케이션 계층을 세분화하여 환경 스케일링
{: #cp_copmscaleenv}

다중 계층 환경은 수직 또는 단일 호스트 아키텍처와 비교할 때 좀 더 쉬운 스케일링 가능성을 제공합니다. 추가 리소스가 필요한 서비스의 스케일링을 허용하여 애플리케이션을 더 쉽게 확장할 수 있도록 다중 계층 환경을 설정할 수 있습니다. 예를 들어, 이전 시나리오에서 웹 서버가 과부화된 경우 다른 웹 서버를 배치할 수 있습니다. 그런 다음 사이트 또는 애플리케이션 데이터를 복제하고 로드 밸런싱하거나 라운드 로빈 DNS를 설정하여 두 개의 웹 서버가 웹 로드를 분할하도록 할 수 있습니다. 라운드 로빈 DNS 또는 로드 밸런싱은 다중 웹 서버에서 수신 요청에 응답할 수 있도록 하여 환경에 고가용성을 제공합니다. 단일 서버가 작동 중지되면 다른 노드를 사용하여 사용자 요청을 처리할 수 있습니다.

데이터베이스를 스케일 확장할 수도 있습니다. 예를 들어, {{site.data.keyword.mysql}} 데이터베이스를 사용할 때 하나의 옵션은 다른 실제 서버를 설정하여 {{site.data.keyword.mysql}} 복제 설정에서 하위로 사용하는 것입니다. 모든 데이터베이스 쓰기를 마스터로 세분화하고 모든 읽기를 하나 이상의 하위로 세분화하여 더 많은 로드를 지원하도록 데이터베이스를 스케일링할 수 있습니다. 또한 하위의 상태를 마스터로 변경할 수 있으므로 이 유형의 설정은 고가용성 레벨을 추가합니다. 그런 다음 {{site.data.keyword.mysql}} 마스터 노드가 작동 중지되는 경우 읽기 및 쓰기 트래픽을 모두 하위로 라우팅할 수 있습니다.

이러한 사례는 환경을 보호하고 스케일링할 수 있는 많은 방법 중 일부에 불과합니다. 보안 또는 확장성 관점에서 환경을 설계하기 위한 최상의 방법과 관련된 질문이나 문의사항이 있는 경우 {{site.data.keyword.BluSoftlayer_notm}} 인프라의 영업 기술 팀이 도움을 드릴 수 있습니다.
