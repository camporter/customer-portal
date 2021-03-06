---

copyright:

  years: 1994, 2019

lastupdated: "2019-02-25"

keywords: audit log, user's access, interactions of each user, infrastructure system events 

subcollection: customer-portal

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}



# {{site.data.keyword.Bluemix_notm}} 인프라 시스템 이벤트 모니터링
{: #customerportal_monevent}

시스템이 계속해서 원활하게 실행되도록 시스템 이벤트를 모니터링할 수 있습니다. {{site.data.keyword.BluSoftlayer_full}}인프라에서 가상 서버 설정 및 관리에 대한 정보는 [가상 서버 시작하기](/docs/vsi/vsi_index.html#getting-started-with-virtual-servers)를 참조하십시오.
{:shortdesc}

## 계정에 대한 감사 로그 보기
{: #cp_viewacctauditlog}

각 고객 포털 계정에는 고객 포털 내 각 사용자의 상호작용을 추적하는 감사 로그가 제공됩니다. 추적된 상호작용에는 로그인 시도(성공 및 실패), 포트 속도 업데이트, 전원 켜기 또는 끄기 및 다시 시작, {{site.data.keyword.BluSoftlayer_notm}} 인프라 지원 직원이 수행하는 상호작용이 포함됩니다. 사용자 계정에 대한 감사 로그를 보려면 다음 단계를 수행하십시오.

1. 고유 인증 정보를 사용하여 [고객 포털 ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}에 액세스하십시오.
2. 탐색줄에서 **계정** > **관리** > **감사 로그**를 선택하여 감사 로그에 액세스하십시오.

감사 로그에는 처음에 사용자가 계정에서 수행한 최근 25개의 상호작용이 표시됩니다. 언제든지 최대 200개의 상호작용을 볼 수 있습니다. **표시** 드롭 다운 목록에서 표시된 결과의 수를 업데이트하십시오. 설정이 변경된 경우 상호작용에 대한 **조치** 열에 링크가 포함됩니다. 조치에 영향을 받은 설정과 변경사항에 대한 세부사항을 보려면 링크를 클릭하십시오. 상호작용에 대한 디바이스 이름 또는 사용자 이름을 클릭하면 디바이스 세부사항 화면 또는 사용자 프로파일 화면으로 각각 사용자를 경로 재지정합니다.

## 사용자의 액세스 로그 보기
{: #cp_viewuserlogs}

액세스 로그는 특정 고객 포털 사용자가 수행한 각 액세스 시도에 대한 데이터를 표시합니다. 로그는 각 액세스 시도에 대한 시간소인 및 IP 주소를 표시합니다. 사용자의 액세스 로그를 보려면 다음 단계를 수행하십시오.

1. 고유 인증 정보를 사용하여 [고객 포털 ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window}에 액세스하십시오.
2. 메뉴 표시줄에서 **계정** > **사용자**를 선택하여 사용자 창에 액세스하십시오.
3. **조치** 드롭 다운 목록에서 **감사 로그 보기**를 선택하여 사용자의 액세스 로그를 보십시오.

각 사용자에 대한 액세스 로그는 액세스 시도가 수행된 IP 주소와 함께 날짜별로 해당 사용자가 수행한 액세스 시도를 표시합니다. 액세스 로그 내 정보는 읽기 전용이므로 컨텐츠 편집을 아무 때나 수행할 수 없습니다. 이전 단계를 반복하여 언제든지 액세스 로그를 다시 볼 수 있습니다. 로그를 종료하고 사용자 화면으로 돌아가려면 **사용자 모두 보기** 링크를 클릭하십시오.
