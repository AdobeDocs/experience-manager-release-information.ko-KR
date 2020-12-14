---
title: 이전 버전의 AEM, CQ 및 CRX
description: 이전 버전의 Adobe Experience Manager, CQ 및 CRX에 대한 설명서 패키지
translation-type: tm+mt
source-git-commit: 47b391ed659264b611f08d2fa9e45a923be5c445
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 23%

---


# 이전 버전의 [!DNL Adobe Experience Manager], CQ 및 CRX {#older-versions-aem-cq-crx}

## 이전 버전의 [!DNL Experience Manager] 설명서 {#older-version-aem-documentation}

이 페이지에 나열된 [!DNL Experience Manager], CQ 및 CRX 버전은 단종이며 더 이상 Adobe에서 공식적으로 판매되지 않습니다. 이러한 이전 버전에 대한 공식적인 설명서의 최신 버전은 자가 도움말 요구 시 사용할 수 있습니다. 최신 버전(현재 [[!DNL Experience Manager] 6.5](https://experienceleague.adobe.com/docs/experience-manager-65.html))으로 업그레이드하는 것이 좋습니다.

>[!NOTE]
>
>[!DNL Experience Manager] 버전이 핵심 지원이 종료되는 시기를 알려면 [제품 및 기술 지원 기간](https://helpx.adobe.com/kr/support/programs/eol-matrix.html) 및 `AEM`을(를) 참조하십시오.

### 설치하기 전에 {#before-installation}

패키지를 다운로드하기 전에 컨텐츠를 누가 사용할 것인지 결정하십시오. 이 결정에 따라 배포 방법이 결정됩니다.

* 개발자는 빠른 참조를 위해 로컬에서 설치할 수 있습니다.
* 보다 광범위한 조직의 문서화 요구를 위해서는 패키지가 내부적으로 액세스할 수 있는 비프로덕션 AEM 작성자 인스턴스에 배포되는 것이 좋습니다.

>[!NOTE]
>
>[!DNL Experience Manager] 작성자에서 이 콘텐츠에 액세스하려면 사용자가 [!DNL Experience Manager] 인스턴스에 로그인해야 합니다. 이 컨텐츠는 기본적으로 AEM 게시(/ libs 아래에 있음)에서 액세스할 수 없습니다.

## 소프트웨어 배포 위치 {#software-distribution-locations}

유효한 Adobe ID이 필요합니다.

* Adobe ID이 없는 경우 www.adobe.com에서 만들 수 있습니다.
Adobe ID 만들기 또는 관리에 도움이 필요한 경우 [이 안내서](https://helpx.adobe.com/manage-account.html)를 참조하십시오.

| [!DNL Experience Manager] 버전 | 소프트웨어 배포 링크 |
|:-----------:|:--------------------------------------------------:|
| [!DNL Experience Manager] 6.1 | [소프트웨어 배포에서 AEM-DOCS-6.1 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/aem-docs-6-1.zip) |
| [!DNL Experience Manager] 6.0 | [소프트웨어 배포에서 AEM-DOCS-6.0 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/aem-docs-6-0.zip) |
| [!DNL Experience Manager] 5.6.1 | [소프트웨어 배포에서 AEM-DOCS-5.6.1 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/aem-docs-5-6-1.zip) |
| [!DNL Experience Manager] 5.6 | [소프트웨어 배포에서 AEM-DOCS-5.6 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/aem-docs-5-6.zip) |
| CQ 5.5 | [소프트웨어 배포에서 CQ-DOCS-5.5 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Faem-docs%2Faem-docs-5-5.zip) |
| CQ 5.4 | [소프트웨어 배포에서 CQ-DOCS-5.4 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/aem-docs-5-4.zip) |
| CQ 5.3 | [소프트웨어 배포에서 CQ-DOCS-5.3 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/aem-docs-5-3.zip) |
| CRX 2.3 | [소프트웨어 배포에서 CRX-DOCS-2.3 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/crx-docs-2-3.zip) |
| CRX 2.2 | [소프트웨어 배포에서 CRX-DOCS-2.2 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/crx-docs-2-2.zip) |
| CRX 2.1 | [소프트웨어 배포에서 CRX-DOCS-2.1 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/crx-docs-2-1.zip) |
| CRX 2.0 | [소프트웨어 배포에서 CRX-DOCS-2.0 다운로드](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/aem-docs/crx-docs-2-0.zip) |

## 설명서 패키지를 설치하는 방법 {#how-to-install-documentation-package}

기존 설명서 패키지를 설치하려면 로컬 드라이브나 네트워크 드라이브에 [!DNL Experience Manager]이(가) 설치되어 있어야 합니다.

### 설명서 패키지 {#download-documentation-package} 다운로드

1. 위의 표에서 다운로드할 [!DNL Experience Manager] 설명서 버전의 링크를 선택합니다. 예: AEM 5.6.1.

1. Adobe ID을 사용하여 로그인합니다. ID가 없는 경우 ID를 만드십시오.

1. **[!UICONTROL 다운로드]** 단추를 선택합니다.

1. 다음은 표시되는 예제입니다.

![소프트웨어 배포 예](assets/screen_shot_2020-07-10at161922.jpg)

### 로컬 인스턴스 {#install-package-local-instance}에 패키지를 설치합니다.

1. [!DNL Experience Manager] 사용자 인터페이스를 엽니다. 웹 브라우저에서 다음을 입력합니다.`http://localhost:4502/`. 관리자로 로그인합니다.

1. **[!UICONTROL 도구]** > **[!UICONTROL 배포]** > **[!UICONTROL 패키지]**&#x200B;를 선택합니다.

1. 패키지 관리자 UI에서 **[!UICONTROL 패키지 업로드]**&#x200B;를 선택합니다.

1. AEM 5.6.1 패키지(aem-docs-5-6-1.zip)를 다운로드한 위치로 이동합니다.

1. 패키지를 선택하고 **[!UICONTROL 확인]**&#x200B;을 클릭합니다.

1. 패키지가 업로드되었으면 패키지를 설치해야 합니다.

1. 패키지 관리자 UI에서 패키지를 찾아 **[!UICONTROL 설치]**&#x200B;를 선택합니다.

1. 확인 대화 상자에서 **[!UICONTROL 설치]**&#x200B;를 다시 선택합니다. 참고: 설치하는 데 몇 분 정도 소요됩니다.

1. 웹 브라우저에서 설명서 페이지를 시작합니다. AEM 5.6.1 예를 사용하면 URL은 다음과 같습니다.http://localhost:4502/libs/aem-docs/content/en/cq/5-6-1.html을 참조하십시오.

## [!DNL Experience Manager] 커뮤니티 {#get-help-from-aem-community}에서 도움 받기

Experience Manager 사용에 대한 질문이 있는 경우[forums [!DNL Experience Manager] 에서 경험이 많은 커뮤니티 전문가에게 문의하는 것이 좋습니다.](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
