---
title: "[!DNL Experience Manager] 최근 설명서 업데이트"
description: ' [!DNL Experience Manager] 설명서의 새로운 기능, 업데이트 또는 변경 사항'
contentOwner: trushton
exl-id: 8c136a03-f961-4854-af38-45457b85d289
source-git-commit: ce1026216ccb79a3c268b3f6b24698fa3a3388dc
workflow-type: tm+mt
source-wordcount: '2459'
ht-degree: 100%

---

# [!DNL Experience Manager] 설명서: 최신 설명서 업데이트 {#aem-documentation-recent-documentation-updates}

이 페이지에는 새해부터 적용되는 Adobe Experience Manager에 대한 중요 문서 변경 사항 및 업데이트가 기재되어 있습니다.

[이전 문서 업데이트](previous-documentation-updates.md)도 조회할 수 있습니다.

## [!DNL Experience Manager] as a [!DNL Cloud Service] {#aem-as-a-cloud-service}

이 페이지에는 [!DNL Adobe Experience Manager]에 대한 설명서의 중요 변경 사항 및 업데이트가 기재되어 있습니다.

[이전 문서 업데이트](previous-documentation-updates.md)도 조회할 수 있습니다.

## [!DNL Adobe Experience Manager] as a [!DNL Cloud Service] {#aem-cloud-service}

>[!NOTE]
>
>Experience Manager as a Cloud Service는 매월 릴리스됩니다.
>
>개별 릴리스(현재 및 이전 버전)와 관련된 설명은 [릴리스 정보](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/release-notes/release-notes/release-notes-current.html)를 참조하십시오.

| 날짜 | 주제 | 변경 사항 |
| --- | --- | --- |
| 2021년 11월 25일 | Dynamic Media 포함 AEM - 구성 | 이제 Dynamic Media 데스크탑 애플리케이션을 사용하지 않고도 AEM의 Dynamic Media 내에서 바로 일반 설정과 게시 설정을 구성할 수 있습니다.<br>[이미지 서버에 대한 Dynamic Media 일반 설정 구성](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/dm-general-settings.html?lang=ko-KR) 및 [Dynamic Media 게시 설정 구성](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/dm-publish-settings.html?lang=ko-KR)을 참조하십시오.<br>또한 [Dynamic Media 구성 - Scene7 모드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=ko-KR)를 참조하십시오. |
| 2021년 11월 4일 | Dynamic Media 포함 AEM - 스마트 자르기 | 최신 Adobe Sensei 서비스를 사용하여 이미지 에셋의 스마트 자르기 및 스마트 색상 견본 기능을 개선했습니다. 다음 사항을 포함하도록 설명서가 업데이트되었습니다.<br>• 이미지 프로필의 자르기 옵션 대화 상자에 새로운 **[!UICONTROL 대상 해상도 전체에서 자르기 콘텐츠 유지]** 옵션이 도입되었습니다.<br>• 여러 에셋의 스마트 자르기 창을 수동으로 재정렬하거나 크기를 조정하면 나중에 해당 에셋을 재처리하는 경우에도 이러한 편집 내용이 유지되고 보존됩니다. 단, 이미지 프로필의 **[!UICONTROL 반응형 이미지 자르기]** 영역에서 폭, 높이 또는 두 가지 모두를 편집하면 해당 에셋이 재처리됩니다.<br>• 스마트 자르기 및 색상 견본에 대해 지원되는 이미지 파일 형식의 표가 새로 도입되었습니다.<br>이러한 업데이트에 대해 [이미지 프로필](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/image-profiles.html)을 참조하십시오. |
| 2021년 11월 3일 | 스마트 자르기 비디오 뷰어 API | 이제 Dynamic Media 뷰어 참조 안내서에서 새로운 [스마트 자르기 비디오 뷰어 API 설명서](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/smartcropvideo/c-html5-aem-smartcropvideo-viewer-reference.html?lang=ko)를 이용할 수 있습니다. |
| 2020년 12월 2일 | 일괄처리 집합 사전 설정 | Dynamic Media에서 일괄처리 집합 사전 설정을 사용하여 이미지 세트 및 스핀 세트 생성을 자동화하는 방법을 알아봅니다. [일괄처리 집합 사전 설정](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/batch-set-presets-dm.html)을 참조하십시오. |
| 2020년 12월 2일 | Dynamic Media의 액세스 가능성 | Dynamic Media 및 Dynamic Media 뷰어는 작성 사용자 인터페이스에서 키보드 제어와 JAWS 및 NVDA 화면 판독기와 같은 보조 기술을 지원합니다. ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/accessibility-dm.html)Dynamic Media의 액세스 가능성[을 참조하십시오. |
| 2020년 10월 29일 | 코어 구성 요소 | 코어 구성 요소 릴리스 2.12.0에서는 새로운 POST 양식 핸들러, 컨텍스트 인식 구성을 통해 사용자 정의 CSS, JavaScript 및 메타데이터 태그를 포함하는 기능 및 **DataLayerBuilderutility**&#x200B;로 사용자 정의 구성 요소의 데이터 레이어 통합을 단순화는 기능이 도입되었습니다. 이 릴리스는 [작성 설명서](https://experienceleague.adobe.com/docs/experience-manager-core-components/using/introduction.html?lang=ko-KR)와 [GitHub에 제공된 개발자 세부 사항 및 프로젝트 다운로드](https://github.com/adobe/aem-core-wcm-components)와 함께 제공됩니다. |
| 2020년 9월 24일 | 새 Dynamic Media 구성 이후 받은 편지함 알림 | 새 Dynamic Media 구성의 설정을 마치면 Experience Manager의 받은 편지함 내에 상태 알림을 받게 됩니다. 이 알림은 구성이 성공했는지 여부를 알려줍니다. 구성이 실패하면 알림에 오류 코드가 표시됩니다. Adobe 지원 센터에 문의할 때 이 오류 코드를 사용하십시오.<br>[새 Dynamic Media 구성 문제 해결을 참조하십시오.](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/config-dm.html?lang=ko) |
| 2020년 9월 24일 | Dynamic Media 구성 내에서 암호 재설정 | Dynamic Media Classic이 아니라 Dynamic Media 내에서 처음 임시 암호 및 이후 암호를 재설정할 수 있도록 허용합니다. [클라우드 서비스에서 Dynamic Media 구성 만들기](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/config-dm.html?lang=ko#configuring-dynamic-media-cloud-services), 6단계 및 7단계와 [Dynamic Media의 암호 변경](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/config-dm.html?lang=ko#change-dm-password)을 참조하십시오. |
| 2020년 9월 24일 | Dynamic Media의 선택적 게시 작업 | 폴더 수준에서 Experience Manager 또는 Dynamic Media로/에서 에셋을 게시 또는 게시 취소하도록 선택할 수 있습니다. Dynamic Media 인스턴스의 모든 폴더에 전역 설정을 적용하는 Dynamic Media 구성에 전적으로 의존하는 대신 게시 관리 또는 빠른 게시를 사용하여 해당 작업을 수행할 수 있습니다.<br>[Dynamic Media의 선택적 게시 작업](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/selective-publishing.html?lang=ko)을 참조하십시오. |
| 2020년 9월 11일 | SPA(Single Page Applications) | SPA(Single Page Application) Editor JavaScript SDK는 이제 [오픈 소스](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/hybrid/reference-materials.html?lang=ko)입니다. |
| 2020년 8월 27일 | Dynamic Media의 CDN 무효화 | CDN 캐시가 몇 분 내에 만료될 수 있도록 Dynamic Media 내에서 요청을 보낼 수 있습니다. 이 기능은 Assets에 대한 업데이트를 만들 때 해당 변경을 즉시 웹 사이트에 적용하려는 경우 유용합니다.<br>[Dynamic Media의 방식으로 CDN 캐시 무효화](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/invalidate-cdn-cache-dynamic-media.html?lang=ko)를 참조하십시오. |
| 2020년 8월 11일 | 페이지 게시의 켜기 및 끄기 시간 | [켜기 및 끄기 시간](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/fundamentals/page-properties.html?lang=ko#basic)을 사용하여 페이지를 게시할 때 페이지 속성의 기본 탭이 표시되어 이제 [자동 복제를 사전 구성할 수 있습니다.](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/operations/replication.html?lang=ko#on-and-off-times-trigger-configuration) |
| 2020년 7월 23일 | 코어 구성 요소 | 코어 구성 요소 릴리스 2.11.0은 AMP 지원이 도입되었으며 이제 [작성 설명서](https://experienceleague.adobe.com/docs/experience-manager-core-components/using/introduction.html?lang=ko-KR)와 [GitHub에서 사용 가능한 개발자 세부 사항 및 프로젝트 다운로드](https://github.com/adobe/aem-core-wcm-components)와 함께 제공됩니다. |
| 2020년 7월 15일 | 슬링 치트시트 | [슬링 치트시트](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/full-stack/sling-cheatsheet.html?lang=ko)가 [HTL](https://experienceleague.adobe.com/docs/experience-manager-htl/content/overview.html?lang=ko)을 참조하도록 업데이트되었습니다. |
| 2020년 6월 24일 | 콘텐츠 조각 | [이제 Models가 표준이어서 설명서가 업데이트되었습니다. ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/content-fragments/content-fragments.html?lang=ko) |
| 2020년 6월 19일 | Experience Manager | Adobe에서는 당사의 규약과 설명서, 경험 전반에 걸쳐 일관되고 동일한 용어를 사용하고자 합니다.<br>이에 따라 이 설명서 세트가 업데이트되었습니다. |
| 2020년 6월 19일 | 코어 구성 요소 | 코어 구성 요소 릴리스 2.10.0은 PDF 뷰어 구성 요소를 도입하였으며 이제 [작성 설명서](https://experienceleague.adobe.com/docs/experience-manager-core-components/using/introduction.html?lang=ko-KR) 및 [GitHub에서 사용 가능한 개발자 세부 사항 및 프로젝트 다운로드](https://github.com/adobe/aem-core-wcm-components)와 함께 제공됩니다. |
| 2020년 6월 4일 | Brand Portal로 Experience Manager Assets를 클라우드 서비스로 구성 | Adobe I/O가 새 브랜드, 사용자 인터페이스 및 워크플로를 사용하여 Adobe Developer Console로 업그레이드되었습니다. 이 설명서는 [Brand Portal을 사용하여 Experience Manager Assets를 클라우드 서비스로 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/brand-portal/configure-aem-assets-with-brand-portal.html?lang=ko)하도록 최신 Adobe Developer Console 워크플로를 기반으로 업데이트되었습니다. |
| 2020년 6월 1일 | 리치 텍스트 편집기 (RTE) | Adobe Experience Manager as a Cloud Service에 다음 리치 텍스트 편집기(RTE) 문서가 제공됩니다. <br>- [RTE 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/configuring-and-extending/rich-text-editor.html?lang=ko)<br>- [개별 플러그인 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/configuring-and-extending/configure-rich-text-editor-plug-ins.html?lang=ko)<br>- [RTE를 구성하여 액세스 가능한 페이지 만들기](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/configuring-and-extending/rte-accessible-content.html?lang=ko)<br>- [RTE를 사용하여 콘텐츠 작성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/fundamentals/rich-text-editor.html?lang=ko) |
| 2020년 5월 29일 | 코어 구성 요소 | 코어 구성 요소 릴리스 2.9.0에는 Adobe 클라이언트 데이터 레이어 및 새 진행률 표시줄 구성 요소와의 통합이 도입되었으며 이제 GitHub의 작성 설명서와 개발자 세부사항 및 프로젝트 다운로드와 함께 제공됩니다. |
| 2020년 5월 19일 | 액세스 가능성 및 WCAG 2.1 지침 | WCAG 2.1 지침 관련 업데이트:<br>- [Adobe Experience Manager as a Cloud Service 및 웹 접근성 지침](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/compliance/accessibility/web-accessibility.html?lang=ko)<br>- [WCAG 2.1에 대한 빠른 안내서](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/compliance/accessibility/quick-guide-wcag.html?lang=ko)<br>- [액세스 가능한 콘텐츠 만들기(WCAG 2.1 호환)](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/fundamentals/accessible-content.html?lang=ko) |
| 2020년 5월 4일 | Dynamic Media에서 지원되지 않는 이미지 형식 | Dynamic Media에서 지원되지 않는 래스터 이미지 파일 형식의 하위 유형 정보입니다.<br>[Dynamic Media에서 지원되지 않는 래스터 이미지 형식](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/assets-formats.html?lang=ko)을 참조하십시오. |
| 2020년 4월 20일 | 콘텐츠 조각 | [콘텐츠 조각 사용자 정의 및 확장](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/configuring-and-extending/content-fragments-customizing.html?lang=ko)과 [렌더링을 위해 구성 요소를 구성하는 콘텐츠 조각](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/configuring-and-extending/content-fragments-configuring-components-rendering.html?lang=ko) 등 [Experience Manager Assets HTTP API의 콘텐츠 조각 지원](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/admin/assets-api-content-fragments.html?lang=ko) 정보입니다. |
| 2020년 4월 9일 | Brand Portal로 Experience Manager Assets를 클라우드 서비스로 구성 | 이제 Brand Portal이 Experience Manager Assets 클라우드 서비스에서 지원됩니다. Adobe I/O에서 Experience Manager Assets 클라우드 서비스를 통해 Brand Portal 테넌트를 구성할 수 있습니다. <br>- [Brand Portal로 Experience Manager Assets를 클라우드 서비스로 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/brand-portal/configure-aem-assets-with-brand-portal.html?lang=ko)<br>- [에셋을 Brand Portal에 게시](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/brand-portal/publish-to-brand-portal.html?lang=ko) |
| 2020년 4월 9일 | Adobe Asset Link v2.0 릴리스 | Adobe Asset Link 2.0에서는 여러 Adobe Experience Manager 환경에서 작업할 수 있으며 Experience Manager as a Cloud Service를 지원합니다. Experience Manager에서는 AAL을 사용하여 에셋을 폴더에 업로드할 때 자동 실행 에셋 처리 워크플로를 구성하고자 하는 마케터를 지원합니다. <br> [Adobe Asset Link](https://helpx.adobe.com/kr/enterprise/using/adobe-asset-link.html)를 참조하십시오. |
| 2020년 3월 24일 | Dynamic Media Cloud Service 구성 | Dynamic Media Cloud Service 구성 시 새 옵션이 제공됩니다.<br>**선택적 게시** - 이 옵션을 선택하면 에셋이 보안 미리보기용으로만 자동 게시됩니다. 공용 도메인에서 게재하기 위해 DMS7에 게시하지 않고 Experience Manager에 명시적으로 게시할 수 있습니다.<br>[Dynamic Media Cloud Service 구성](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/config-dm.html?lang=ko)을 참조하십시오. |
| 2020년 3월 2일 | Dynamic Media - 스마트 자르기 | 새 옵션은 Dynamic Media 구성 요소에서 스마트 자르기로 작업하는 경우 제공됩니다. <br>**종횡비 일치 활성화** - 이 옵션을 선택하면 Dynamic Media에서 원본 이미지의 종횡비에 가장 일치하는 스마트 자르기 렌디션을 선택할 수 있습니다.<br>[스마트 자르기로 작업하는 경우](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/adding-dynamic-media-assets-to-pages.html?lang=ko)를 참조하십시오. |
| 2020년 2월 25일 | 역할 기반 권한 | Cloud Manager에는 적절한 권한이 있는 미리 구성된 역할이 있습니다. 각 역할에는 특정 권한, 사전 구성된 작업 또는 각 역할에 연관된 권한이 있습니다. [역할 기반 권한 페이지](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/onboarding/journey/cloud-manager.html?lang=ko)에는 사용 가능한 기능 및 기능을 실행할 수 있는 역할이 나열됩니다. |
| 2020년 2월 15일 | 클라우드의 디스패처 | [Dispatcher 및 CDN](https://experienceleague.adobe.com/docs/experience-manager-dispatcher/using/dispatcher.html?lang=ko#using-dispatcher-with-a-cdn)과 [명시적 Dispatcher 캐시 무효화](https://experienceleague.adobe.com/docs/experience-manager-dispatcher/using/configuring/page-invalidate.html?lang=ko) 섹션이 사용 가능한 옵션과 그 작동 방법을 명확히 설명하도록 업데이트되었습니다. |

## [!DNL Experience Manager] 6.5 {#aem-65}

| 날짜 | 주제 | 변경 사항 |
| --- | --- | --- |
| 2021년 11월 25일 | [!DNL Experience Manager] 6.5 서비스 팩 11 | [[!DNL Experience Manager] 6.5 서비스 팩 11](https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.11.html?lang=ko)을 사용할 수 있습니다. |
| 2021년 11월 3일 | 스마트 자르기 비디오 뷰어 API | 이제 Dynamic Media 뷰어 참조 안내서에서 새로운 [스마트 자르기 비디오 뷰어 API 설명서](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/smartcropvideo/c-html5-aem-smartcropvideo-viewer-reference.html?lang=ko)를 이용할 수 있습니다. |
| 2021년 8월 26일 | [!DNL Experience Manager] 6.5 서비스 팩 10 | [[!DNL Experience Manager] 6.5 서비스 팩 10](https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.10.html?lang=ko)을 사용할 수 있습니다. |
| 2021년 5월 27일 | [!DNL Experience Manager] 6.5 서비스 팩 9 | [[!DNL Experience Manager] 6.5 서비스 팩 9](https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.9.html?lang=ko)를 사용할 수 있습니다. |
| 2021년 3월 11일 | [!DNL Experience Manager] 6.5 서비스 팩 8 | [[!DNL Experience Manager] 6.5 서비스 팩 8](https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.8.html?lang=ko)을 사용할 수 있습니다. |
| 2020년 11월 25일 | Dynamic Media의 액세스 가능성 | Dynamic Media 및 Dynamic Media 뷰어는 작성 사용자 인터페이스에서 키보드 제어와 JAWS 및 NVDA 화면 판독기와 같은 보조 기술을 지원합니다. ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/accessibility-dm.html#dynamic)Dynamic Media의 액세스 가능성[을 참조하십시오. |
| 2020년 11월 26일 | Experience Manager 6.5 서비스 팩 7 | [Experience Manager 6.5 서비스 팩 7](https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.7.html?lang=ko)을 사용할 수 있습니다. |
| 2020년 9월 3일 | Dynamic Media의 CDN 무효화 | CDN 캐시가 몇 분 내에 만료될 수 있도록 Dynamic Media 내에서 요청을 보낼 수 있습니다. 이 기능은 Assets에 대한 업데이트를 만들 때 해당 변경을 즉시 웹 사이트에 적용하려는 경우 유용합니다.<br>[Dynamic Media의 방식으로 CDN 캐시 무효화](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/invalidate-cdn-cache-dynamic-media.html?lang=ko)를 참조하십시오. |
| 2020년 9월 3일 | Dynamic Media의 선택적 게시 작업 | 폴더 수준에서 Experience Manager 또는 Dynamic Media로/에서 에셋을 게시 또는 게시 취소하도록 선택할 수 있습니다. Dynamic Media 인스턴스의 모든 폴더에 전역 설정을 적용하는 **Dynamic Media 구성**&#x200B;에 전적으로 의존하는 대신 **[!UICONTROL 게시 관리]** 또는 **[!UICONTROL 빠른 게시]**&#x200B;를 사용하여 해당 작업을 수행할 수 있습니다.<br>[Dynamic Media의 선택적 게시 작업](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/selective-publishing.html?lang=ko)을 참조하십시오. |
| 2020년 9월 3일 | Experience Manager 6.5 서비스 팩 6 | [Experience Manager 6.5 서비스 팩 6](https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.6.html?lang=ko)을 사용할 수 있습니다. |
| 2020년 7월 29일 | 다중 사이트 관리자 | [동기화 작업 만들기](https://experienceleague.adobe.com/docs/experience-manager-65/developing/extending-aem/extending-msm.html?lang=ko#creating-a-new-synchronization-action) 및 [롤아웃 구성 만들기](https://experienceleague.adobe.com/docs/experience-manager-65/developing/extending-aem/extending-msm.html?lang=ko#creating-a-new-rollout-configuration) 절차에 업데이트가 있습니다. |
| 2020년 7월 15일 | 슬링 치트시트 | [슬링 치트시트](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/sling-cheatsheet.html?lang=ko)가 [HTL](https://experienceleague.adobe.com/docs/experience-manager-htl/content/overview.html?lang=ko)을 참조하도록 업데이트되었습니다. |
| 2020년 6월 19일 | Adobe Experience Manager | Adobe에서는 당사의 규약과 설명서, 경험 전반에 걸쳐 일관되고 동일한 용어를 사용하고자 합니다.<br>이에 따라 이러한 공정성을 반영하는 이 설명서 세트에 대한 업데이트가 이루어졌습니다. |
| 2020년 6월 4일 | Brand Portal로 Experience Manager Assets 구성 | Adobe I/O가 새 브랜드, 사용자 인터페이스 및 워크플로를 사용하여 Adobe Developer Console로 업그레이드되었습니다. 이 설명서는 최신 Adobe Developer Console 워크플로를 기반으로 Brand Portal로 Experience Manager Assets를 구성하도록 업데이트되었습니다. <br>- [Brand Portal로 Experience Manager Assets 구성](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html?lang=ko)<br>- [Adobe Developer Console에 대한 기존 구성 업그레이드](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html?lang=ko#upgrade-integration-65) |
| 2020년 6월 4일 | Experience Manager 6.5 서비스 팩 5 | [Experience Manager 6.5 서비스 팩 5](https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.5.html?lang=ko)를 사용할 수 있습니다. |
| 2020년 5월 25일 | 액세스 가능성 및 WCAG 2.1 지침 | WCAG 2.1 지침 관련 업데이트:<br>- [Adobe Experience Manager as a Cloud Service 및 웹 접근성 지침](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/compliance/accessibility/web-accessibility.html?lang=ko)<br>- [WCAG 2.1에 대한 빠른 안내서](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/compliance/accessibility/quick-guide-wcag.html?lang=ko)<br>- [액세스 가능한 콘텐츠 만들기(WCAG 2.1 호환)](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/fundamentals/accessible-content.html?lang=ko) |
| 2020년 4월 13일 | 에셋 버전 관리 | [Experience Manager 에셋의 버전](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/manage-assets.html?lang=ko#asset-versioning)으로 되돌리거나 생성하거나 미리 보는 방법에 대한 콘텐츠 및 비디오가 업데이트되었습니다. |
| 2020년 4월 13일 | 에셋 처리 | 에셋 처리에 워크플로를 사용하는 방법에 관하여 새 개요가 추가되었습니다. 또한 새 주제에서 [에셋을 처리하는 워크플로 자동 트리거](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/assets-workflow.html?lang=ko) 방법을 설명합니다. |
| 2020년 3월 30일 | Dynamic Media - 스마트 이미징 | 전체 스마트 이미징 도움말 주제가 업데이트되어 추가된 스마트 이미징 최적화를 설명하는 이미지 에셋 예제 등의 새 정보가 포함되었습니다.<br>[스마트 이미징](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html?lang=ko)을 참조하십시오. |
| 2020년 3월 5일 | Experience Manager 6.5 서비스 팩 4 | [Experience Manager 6.5 서비스 팩 4](https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.4.html?lang=ko)를 사용할 수 있습니다. |
| 2020년 3월 4일 | Dynamic Media 구성 - Scene7 모드 | 이제 도구 > 클라우드 서비스의 Dynamic Media 구성 페이지에서 새로운 “모든 콘텐츠 동기화” 옵션을 사용할 수 있습니다.<br>[Dynamic Media 구성 만들기](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=ko#configuring-dynamic-media-cloud-services)를 참조하십시오. |