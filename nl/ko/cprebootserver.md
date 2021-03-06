---

copyright:

  years: 1994, 2019

lastupdated: "2018-02-25"

keywords: rescue kernel, command line, restart command

subcollection: customer-portal 

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}

# 서버 다시 부팅
{: #customerportal_rebootserver}

때때로 서버를 다시 시작해야 하는 {{site.data.keyword.BluSoftlayer_notm}} 인프라에서 이벤트가 발생합니다.
{:shortdesc}

서버를 다시 시작하려면 다음 단계를 사용하십시오.
1. 고객 포털에서 **지원** 탭을 클릭하십시오.
2. **다시 부팅**을 클릭하십시오.
3. 다시 시작할 서버를 선택하고 **다시 부팅**을 클릭하십시오.
4. 서버를 다시 시작하려면 다음 방법 중 하나를 선택하십시오.
  * 기본값(IPMI와 전원 스트립을 차례로 사용하여 다시 시작 시도)
  * IPMI
  * 전원 스트립
5. **다시 부팅**을 클릭하십시오.

이 페이지에서는 복구 커널로 부팅할 수 있는 기능을 제공하며, 이 기능은 구성 문제로 인해 서버가 OS에 부팅할 수 없는 문제점이 발생하는 경우 매우 유용합니다. 복구 커널에 부팅한 후 서버의 드라이브를 마운트한 후 구성 문제를 해결할 수 있습니다. 문제를 수정한 후 명령행에서 서버를 다시 시작할 수 있고 서버는 사용자 서버의 기본 커널로 다시 시작됩니다. 다시 시작 명령을 실행하면 완료 예상 시간이 표시됩니다.
