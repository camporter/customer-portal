---

copyright:

  years: 1994, 2019

lastupdated: "2019-02-25"

keywords: master user, unique account permission set, SoftLayer account, account permissions 

subcollection: customer-portal

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:tip: .tip}
{:screen: .screen}
{:new_window: target="_blank"}
{:note: .note}


# 向 SoftLayer 帐户添加用户
{: #customerportal_addusertocpacct}

一个或多个用户可以与帐户的关联产品和服务进行交互。如果您是主用户，或者具有管理访问权，那么可以添加用户。
{:shortdesc}

如果您要管理 {{site.data.keyword.BluSoftlayer_full}} 基础架构用户，那么您可以管理的 SoftLayer 帐户取决于分配给您的用户帐户的访问权。您可以管理的帐户还取决于帐户的设置方式。如果您是主用户，或者以帐户所有者身份拥有管理访问权，那么可以管理其他客户门户网站用户。如果您的帐户未设置为主用户，那么您可以管理自己的用户概要文件。

根据您的访问权，您可以通过“用户”窗口来管理您的 SoftLayer 帐户或其他用户的帐户。[客户门户网站 ![外部链接图标](../icons/launch-glyph.svg)](https://control.softlayer.com/){:new_window} 中的“用户”窗口会显示与帐户关联的用户。“用户”窗口上可用的交互根据您的唯一帐户许可权集而有所不同。
  * 如果您是帐户的主用户，那么可以查看与该帐户关联的所有用户。

  如果您必须共享帐户的主登录凭证，共享凭证时务必谨慎。主登录将控制您帐户的各个方面，必须谨慎地保护好。要使其他用户能够使用客户门户网站，您可以设置单个用户或基于许可权的用户。创建基于许可权的用户可确保您最大限度地控制谁能够与您帐户的某些方面进行交互。
{:tip}

  * 如果您具有管理访问权，那么可以查看您添加的所有用户。如果向这些用户授予了管理其他用户的许可权，那么还可以查看他们添加的任何用户。您还可以管理与帐户关联的任何用户。这包括编辑对客户门户网站的访问权，更改用户状态以及除去用户。

要通过 {{site.data.keyword.Bluemix_notm}} 控制台来管理用户，请参阅[帐户设置](/docs/account?topic=account-signup#signup)部分以及[管理身份和访问权](/docs/iam?topic=iam-getstarted#getstarted)。有关 {{site.data.keyword.Bluemix_notm}} 控制台的更多信息，请参阅[导航 {{site.data.keyword.Bluemix_notm}} 控制台](/docs/overview?topic=overview-ui#ui)。

组织内的不同人员具有不同的角色和责任，因而用户许可权集并不通用。您可以使用角色将用户添加到客户门户网站，以提供与其特定角色相应的访问权来准确访问其所需内容。如果错误地做出更改或更改未经授权，您可以根据这些更改追溯到相关用户或组。因此，您可以提供相应培训或更新用户许可权以最小化风险。然后，您的用户可以重点关注在客户门户网站中为其指定的角色上。

使用以下步骤向帐户添加用户。

1. 使用您的唯一凭证来访问客户门户网站。
2. 从导航栏中选择**帐户 > 用户**。
3. 单击**添加用户**。
4. 填写**个人信息**部分中的必填字段。提供状态、用户名和用于客户门户网站通信和通知（包括用于为帐户设置密码的初始通知）的电子邮件地址。

  （可选）您可以不输入用户的地址，而改为单击**使用缺省公司信息**复选框来填充公司地址。
  {: tip}

5. 填写**登录设置**部分中的必填字段。指定用户是否可以编辑设置，IP 地址是否受到限制，以及是否需要用户来设置和使用安全问题。另外，对于任何不使用 IBM 标识的用户，您可以设置密码在多长时间后到期。
**注：**
    * 如果使用 IBM 标识进行认证，请按照**登录**下的指示信息，在 [IBM 标识概要文件 ![外部链接图标](../icons/launch-glyph.svg)](https://www.ibm.com/account/profile){:new_window} 中更新密码。
    * 单击**将门户网站密码用于 VPN** 复选框，以同步客户门户网站和 VPN 的密码。
6. 单击**添加用户**。

为用户创建帐户后，用户将收到一封电子邮件通知，用于完成其帐户设置。用户必须设置密码并（可选）创建安全问题（如果您指示需要使用安全问题）。

没有主用户管理访问权的用户如何登录到客户门户网站，这取决于在其 SoftLayer 帐户中提供了用户访问权的主用户：
  * 如果主用户具有用于认证的 IBM 标识，那么主用户创建的每个用户都会具有 IBM 标识。
  * 如果主用户具有用于认证的 {{site.data.keyword.BluSoftlayer_notm}} 基础架构标识，那么主用户创建的每个用户都会具有 {{site.data.keyword.BluSoftlayer_notm}} 基础架构用户名。主用户和主用户创建的每个用户都必须运行迁移工具来切换到 IBM 标识。
  * 如果这两种情况均不适用（例如，对于 IBM 业务合作伙伴），请联系支持人员以确定要使用的用户标识。

## 设置帐户的用户许可权
{: #cp_setuserpermsacct}

使用以下步骤为刚才添加的用户设置许可权。

1. 单击**许可权**图标（由带锁的用户人像指示）。
2. 为新用户更新所有选项卡上的**用户许可权**。

    从**快速许可权**列表中选择一个选项，可查看三种类型用户的许可权集。单击**设置许可权**以选择许可权集，或者通过在每个可用选项卡上选择各个选项来定制用户的访问权。
    {: note}
    
3. 单击**添加门户网站许可权**以添加许可权，或单击**重置许可权**以重置用户的许可权。
4. 单击**设备访问权**图标（由含三台服务器的图形指示）。
5. 单击希望用户访问的每台设备对应的设备复选框。
6. 选择设备后，单击**更新设备访问权**。

您将收到一封电子邮件，其中包含的链接和信息可指导您逐步设置 IBM 标识，用于向此帐户进行认证。如果帐户正在使用 IBM 标识进行认证，那么这些步骤可包括创建新的 IBM 标识。邀请会在 7 天后到期，但您可以联系管理员重新发送邀请。

对于其他所有认证情况，在添加新用户后，用户可以随时登录到客户门户网站。用户可以使用与该帐户关联的各种产品和服务。您可以随时停用该用户。
