---
title: AEM Forms 릴리스
description: 모든 AEM Forms 릴리스 및 해당 패키지의 목록을 포함합니다.
contentOwner: khsingh
exl-id: 65cb9c6b-fb3f-4bf1-aa42-2d724914439a
source-git-commit: e7b7f231d7a379eb6d882ca4aa39e3bec8dbbe4a
workflow-type: tm+mt
source-wordcount: '2688'
ht-degree: 97%

---

# AEM [!DNL Forms] 릴리스 {#aem-forms-releases}

Adobe Experience Manager [!DNL Forms]는 AEM에 배포된 애플리케이션입니다. 매력적인 웹 및 모바일 경험을 엔터프라이즈 양식 및 문서로 확장하여 기업의 복잡한 디지털 상호 작용을 완료하면서도 사용자 경험을 개선하며 비즈니스 범위를 확장할 수 있습니다. AEM 빠른 시작에 포함된 즉시 사용 가능한 AEM [!DNL Forms]에는 제한된 기능 세트가 있습니다. AEM [!DNL Forms] 추가 기능 패키지는 [!DNL Adobe Analytics], [!DNL Adobe Sign], 문서 서비스, 워크플로 엔진 등의 여러 기능과 통합하는 등 고급 기능을 제공합니다.

>[!NOTE]
>
>
>[AEM 6.5 QuickStart](https://experienceleague.corp.adobe.com/docs/experience-manager-65/deploying/deploying/deploy.html)에서 사용 가능한 적응형 양식 기능은 탐색 및 평가 목적으로만 사용하도록 설계되었습니다. 프로덕션 용도로 사용하려면 적응형 양식 기능에 적절한 라이선싱이 필요하므로 AEM Forms에 대해 유효한 라이선스를 확보해야 합니다.


<!--
>[!NOTE]
>
>AEM Forms releases the add-on packages one week after the scheduled AEM Service Pack and Cumulative Fix Pack release date.

The following list contains all the AEM [!DNL Forms] add-on packages released until today, corresponding AEM versions (Pre-requisites), download links of packages, and other helpful information.
-->

## AEM 6.5 [!DNL Forms] 릴리스 {#aem-65-forms-releases}

<table>
  <tbody>
  <tr>
    <td><strong>날짜</strong></td>
    <td><strong>AEM Forms 릴리스</strong></td>
    <td><strong>전제 조건</strong></td>
    <td><strong>사용 가능한 패키지</strong></td>
    <td><strong>빌드 버전</strong></td>
   </tr>
  </tr>
  <tr>
    <td>2023년 12월 8일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/release-notes.html?lang=en#forms-6519">AEM 6.5.19.0용 AEM Forms 서비스 팩 19 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/release-notes.html?lang=ko-KR">AEM 6.5.19.0</a></td>
    <td>
     <ul>
     <br><b>OSGi의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.1120.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.1120.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.1120.zip">Mac OS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0078/jboss/win/adobe-aem-forms-jee-service-pack-6.5.19.0-windows-jboss.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0078/jboss/linux/adobe-aem-forms-jee-service-pack-6.5.19.0-linux-jboss.gz">JBoss®Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0078/weblogic/win/adobe-aem-forms-jee-service-pack-6.5.19.0-windows-weblogic.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0078/weblogic/linux/adobe-aem-forms-jee-service-pack-6.5.19.0-linux-weblogic.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0078/websphere/win/adobe-aem-forms-jee-service-pack-6.5.19.0-windows-websphere.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0078/websphere/linux/adobe-aem-forms-jee-service-pack-6.5.19.0-linux-websphere.gz">WebSphere® Linux</a></li>
      <br><b>Workbench 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/workbench/6-5-0-20231119-1-12345/Workbench_DVD.zip">AEM Forms Workbench 설치 관리자</a> </li>
      <!-- <br><b>SDK</b></br>
      <li><a href="">AEM Forms Client SDK</a> </li>-->
      <br><b>Forms Designer 32비트 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19/Designer6.5.0_English_Cumulative_QF.msp">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19/Designer6.5.0_French_Cumulative_QF.msp">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19/Designer6.5.0_German_Cumulative_QF.msp">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19/Designer6.5.0_Japanese_Cumulative_QF.msp">일본어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19/Designer6.5.0_Spanish_Cumulative_QF.msp">스페인어 언어 설치 관리자</a> </li>
      <br><b>Forms Designer 64비트 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19_x64/aemforms_designer_6_5_0_wwe_win.zip">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19_x64/aemforms_designer_6_5_0_wwf_win.zip">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19_x64/aemforms_designer_6_5_0_d_win.zip">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19_x64/aemforms_designer_6_5_0_j_win.zip">일본어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp19_x64/aemforms_designer_6_5_0_wws_win.zip">스페인어 언어 설치 관리자</a> </li>
      </ul> 
      </td>
    <td><p>AEM Forms JEE 패치 설치 관리자: aemforms-6-5-0-0078 <br/><p>AEM Forms 추가 기능 패키지: 6.0.1120 </p></td>
   </tr>
   <tr>
    <td>2023년 8월 31일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/release-notes.html#forms-6518">AEM 6.5.18.0용 AEM Forms 서비스 팩 18 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/release-notes.html">AEM 6.5.18.0</a></td>
    <td>
     <ul>
     <br><b>OSGi의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aem-forms-addon-6.5.18.0-linux.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aem-forms-addon-6.5.18.0-windows.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aem-forms-addon-6.5.18.0-osx.zip">Mac OS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.48.zip">AEM Forms 호환성 패키지</a></li>
      <br><b>JEE 전체 설치 관리자의 AEM Forms</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20230913-1-12345/jboss/win/aemforms_server_6_5_0_jboss_all_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20230913-1-12345/jboss/unix/aemforms_server_6_5_0_jboss_all_unix.tar.gz">JBoss®Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20230913-1-12345/weblogic/win/aemforms_server_6_5_0_weblogic_all_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20230913-1-12345/weblogic/unix/aemforms_server_6_5_0_weblogic_all_unix.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20230913-1-12345/websphere/win/aemforms_server_6_5_0_websphere_all_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20230913-1-12345/websphere/unix/aemforms_server_6_5_0_websphere_all_unix.tar.gz">WebSphere® Linux</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0069/jboss/win/adobe-aem-forms-jee-service-pack-6.5.18.0-windows-jboss.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0069/jboss/linux/adobe-aem-forms-jee-service-pack-6.5.18.0-linux-jboss.gz">JBoss®Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0069/weblogic/win/adobe-aem-forms-jee-service-pack-6.5.18.0-windows-weblogic.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0069/weblogic/linux/adobe-aem-forms-jee-service-pack-6.5.18.0-linux-weblogic.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0069/websphere/win/adobe-aem-forms-jee-service-pack-6.5.18.0-windows-websphere.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0069/websphere/linux/adobe-aem-forms-jee-service-pack-6.5.18.0-linux-websphere.gz">WebSphere® Linux</a></li>
      <br><b>Workbench 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/workbench/6-5-0-20230828-1-12345/Workbench_DVD.zip">AEM Forms Workbench 설치 관리자</a> </li>
       <br><b>SDK</b></br>
      <li><a href="https://repo1.maven.org/maven2/com/adobe/aemfd/aemfd-client-sdk/6.0.1016/">AEM Forms 클라이언트 SDK</a> </li>
      <br><b>Forms Designer</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp18/Designer6.5.0_English_Cumulative_QF.msp">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp18/Designer6.5.0_French_Cumulative_QF.msp">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp18/Designer6.5.0_German_Cumulative_QF.msp">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp18/Designer6.5.0_Japanese_Cumulative_QF.msp">일본어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp18/Designer6.5.0_Spanish_Cumulative_QF.msp">스페인어 언어 설치 관리자</a> </li>
      </ul> 
      </td>
    <td><p>AEM Forms JEE 전체 설치 관리자: 
    6-5-0-20230913-1-12345 <br/><p>AEM Forms JEE 패치 설치 관리자: aemforms-6-5-0-0069<br/><p>AEM Forms 추가 기능 패키지: 6.5.18.0 </p></td>
   </tr>
   <tr>
    <td>2023년 6월 01일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/release-notes.html#forms-6517">AEM 6.5.17.0용 AEM Forms Service Pack 17 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/release-notes.html">AEM 6.5.17.0</a></td>
    <td>
     <ul>
     <br><b>OSGi의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.968.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.968.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.968.zip">Mac OS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.48.zip">AEM Forms 호환성 패키지</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0065/JBoss/Win/AEMForms-6.5.0-0065_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0065/JBoss/Linux/AEMForms-6.5.0-0065_jboss_linux.tar.gz">JBoss®Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0065/weblogic/win/AEMForms-6.5.0-0065_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0065/weblogic/linux/AEMForms-6.5.0-0065_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0065/WebSphere/win/AEMForms-6.5.0-0065_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0065/WebSphere/linux/AEMForms-6.5.0-0065_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <br><b>Workbench 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/workbench/6-5-0-20230222-1-12345/workbench_DVD.zip">AEM Forms Workbench 설치 관리자</a> </li>
       <br><b>SDK</b></br>
      <li><a href="https://repo1.maven.org/maven2/com/adobe/aemfd/aemfd-client-sdk/6.0.966/">AEM Forms 클라이언트 SDK</a> </li>
      <br><b>Forms Designer</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp17/Designer6.5.0_English_Cumulative_QF.msp">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp17/Designer6.5.0_French_Cumulative_QF.msp">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp17/Designer6.5.0_German_Cumulative_QF.msp">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp17/Designer6.5.0_Japanese_Cumulative_QF.msp">일본어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp17/Designer6.5.0_Spanish_Cumulative_QF.msp">스페인어 언어 설치 관리자</a> </li>
      </ul> 
      </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6-5-0-0065<br/><p>AEM Forms 추가 기능 패키지: 6.0.968</p></td>
   </tr>
   <tr>
    <td>2023년 3월 2일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.16.html#forms-6516">AEM 6.5.16.0용 AEM Forms 서비스 팩 16 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.16.html">AEM 6.5.16.0</a></td>
    <td>
     <ul>
     <br><b>OSGi의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.914.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.914.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.914.zip">Mac OS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.48.zip">AEM Forms 호환성 패키지</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0062/JBoss/win/AEMForms-6.5.0-0062_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0062/JBoss/linux/AEMForms-6.5.0-0062_jboss_linux.tar.gz">JBoss®Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0062/WebLogic/win/AEMForms-6.5.0-0062_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0062/WebLogic/linux/AEMForms-6.5.0-0062_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0062/webSphere/win/AEMForms-6.5.0-0062_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0062/webSphere/Linux/AEMForms-6.5.0-0062_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <br><b>Workbench 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/workbench/6-5-0-20230222-1-12345/workbench_DVD.zip">AEM Forms Workbench 설치 관리자</a> </li>
      <br><b>SDK</b></br>
      <li><a href="https://repo1.maven.org/maven2/com/adobe/aemfd/aemfd-client-sdk/6.0.904/">AEM Forms 클라이언트 SDK</a> </li>
      <br><b>Forms Designer</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp16_650_038/Designer6.5.0_English_Cumulative_QF.msp">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp16_650_038/Designer6.5.0_French_Cumulative_QF.msp">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp16_650_038/Designer6.5.0_German_Cumulative_QF.msp">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp16_650_038/Designer6.5.0_Japanese_Cumulative_QF.msp">일본어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/sp16_650_038/Designer6.5.0_Spanish_Cumulative_QF.msp">스페인어 언어 설치 관리자</a> </li>
      </ul> 
      </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0062<br/><p>AEM Forms 추가 기능 패키지: 6.0.914</p></td>
   </tr>
   <tr>
    <td>2022년 12월 1일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.15.html#forms-6515">AEM 6.5.15.0용 AEM Forms 서비스 팩 15 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.15.html">AEM 6.5.15.0</a></td>
    <td>
     <ul>
     <br><b>OSGi의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.856.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.856.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.856.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.48.zip">AEM Forms 호환성 패키지</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0057/JBoss/Win/AEMForms-6.5.0-0057_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0057/JBoss/Linux/AEMForms-6.5.0-0057_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0057/WebLogic/Win/AEMForms-6.5.0-0057_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0057/WebLogic/Linux/AEMForms-6.5.0-0057_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0057/WebSphere/win/AEMForms-6.5.0-0057_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0057/WebSphere/linux/AEMForms-6.5.0-0057_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <br><b>Workbench 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/workbench/6-5-0-20221122-1-12345/Workbench_DVD.zip">AEM Forms Workbench 설치 관리자</a> </li>
      <br><b>SDK</b></br>
      <li><a href="https://repo1.maven.org/maven2/com/adobe/aemfd/aemfd-client-sdk/6.0.856/">AEM Forms 클라이언트 SDK</a> </li>
      <br><b>Forms Designer</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/designer-full-installer/english/aemforms_designer_6_5_0_wwe_win.zip">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/designer-full-installer/french/aemforms_designer_6_5_0_wwf_win.zip">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/designer-full-installer/german/aemforms_designer_6_5_0_d_win.zip">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/designer-full-installer/japanese/aemforms_designer_6_5_0_j_win.zip">일본어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/designer-full-installer/spanish/aemforms_designer_6_5_0_wws_win.zip">스페인어 언어 설치 관리자</a> </li>
      </ul> 
      </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0057<br /> <p>AEM Forms 추가 기능 패키지: 6.0.856</p></td>
   </tr>
   <tr>
    <td>2022년 9월 5일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.14.html#forms-6514">AEM 6.5.14.0용 AEM Forms 서비스 팩 14 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.14.html">AEM 6.5.14.0</a></td>
    <td>
     <ul>
     <br><b>OSGi의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.772.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.772.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.772.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.46.zip">AEM Forms 호환성 패키지</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0053/JBoss/Win/AEMForms-6.5.0-0053_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0053/JBoss/Linux/AEMForms-6.5.0-0053_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0053/WebLogic/win/AEMForms-6.5.0-0053_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0053/WebLogic/Linux/AEMForms-6.5.0-0053_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0053/WebSphere/Win/AEMForms-6.5.0-0053_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0053/WebSphere/Linux/AEMForms-6.5.0-0053_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <br><b>SDK</b></br>
      <li><a href="https://repo1.maven.org/maven2/com/adobe/aemfd/aemfd-client-sdk/6.0.772/">AEM Forms 클라이언트 SDK</a> </li>
      <br><b>Forms Designer</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-033/Designer6.5.0_English_Cumulative_QF.msp">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-033/Designer6.5.0_French_Cumulative_QF.msp">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-033/Designer6.5.0_German_Cumulative_QF.msp">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-033/Designer6.5.0_Japanese_Cumulative_QF.msp">일본어 언어 설치 관리자</a> </li>
      </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0053<br /> <p>AEM Forms 추가 기능 패키지: 6.0.772</p></td>
   </tr>
   <tr>
    <td>2022년 6월 2일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.13.html#forms-65130">AEM 6.5.13.0용 AEM Forms 서비스 팩 13 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.13.html">AEM 6.5.13.0</a></td>
    <td>
     <ul>
     <br><b>OSGi의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.718.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.718.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.718.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.42.zip">AEM Forms 호환성 패키지</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0044/JBoss/Win/AEMForms-6.5.0-0044_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0044/JBoss/Linux/AEMForms-6.5.0-0044_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0044/WebLogic/Win/AEMForms-6.5.0-0044_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0044/WebLogic/Linux/AEMForms-6.5.0-0044_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0044/WebSphere/Win/AEMForms-6.5.0-0044_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0044/WebSphere/Linux/AEMForms-6.5.0-0044_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <br><b>SDK</b></br>
      <li><a href="https://repo1.maven.org/maven2/com/adobe/aemfd/aemfd-client-sdk/6.0.728/">AEM Forms 클라이언트 SDK</a> </li>
      <br><b>Forms Designer</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-029/Designer6.5.0_English_Cumulative_QF.msp">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-029/Designer6.5.0_French_Cumulative_QF.msp">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-029/Designer6.5.0_German_Cumulative_QF.msp">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-029/Designer6.5.0_Japanese_Cumulative_QF.msp">일본어 언어 설치 관리자</a> </li>
      </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0044<br /> <p>AEM Forms 추가 기능 패키지: 6.0.718</p></td>
   </tr>
   <tr>
    <td>2022년 3월 3일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.12.html#forms-65120">AEM 6.5.12.0용 AEM Forms 서비스 팩 12 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.12.html">AEM 6.5.12.0</a></td>
    <td>
     <ul>
     <br><b>OSGi의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.640.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.640.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.640.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <br><b>JEE의 AEM Forms 전체 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20220302-1-12345/JBoss/Win/aemforms_server_6_5_0_jboss_all_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20220302-1-12345/JBoss/Unix/aemforms_server_6_5_0_jboss_all_unix.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20220302-1-12345/Weblogic/win/aemforms_server_6_5_0_weblogic_all_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20220302-1-12345/Weblogic/Unix/aemforms_server_6_5_0_weblogic_all_unix.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20220302-1-12345/WebSphere/Win/aemforms_server_6_5_0_websphere_all_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/full-installer/6-5-0-20220302-1-12345/WebSphere/Unix/aemforms_server_6_5_0_websphere_all_unix.tar.gz">WebSphere® Linux</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0040/JBoss/Win/AEMForms-6.5.0-0040_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0040/JBoss/Linux/AEMForms-6.5.0-0040_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0040/Weblogic/Win/AEMForms-6.5.0-0040_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0040/Weblogic/Linux/AEMForms-6.5.0-0040_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0040/WebSphere/Win/AEMForms-6.5.0-0040_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0040/WebSphere/Linux/AEMForms-6.5.0-0040_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <br><b>SDK</b></br>
      <li><a href="https://repo1.maven.org/maven2/com/adobe/aemfd/aemfd-client-sdk/6.0.640/">AEM Forms 클라이언트 SDK</a> </li>
      <br><b>Forms Designer</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-027/Designer6.5.0_English_Cumulative_QF.msp">영어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-027/Designer6.5.0_French_Cumulative_QF.msp">프랑스어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-027/Designer6.5.0_German_Cumulative_QF.msp">독일어 언어 설치 관리자</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-027/Designer6.5.0_Japanese_Cumulative_QF.msp">일본어 언어 설치 관리자</a> </li>
      <br><b>Forms Workbench</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/workbench/6-5-0-20220303-3-12345/Workbench_DVD.zip">영어 언어 설치 관리자</a> </li>
      </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0040<br /> <p>AEM Forms 추가 기능 패키지: 6.0.640</p></td>
   </tr>
   <tr>
    <td>2021년 12월 20일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.11.html#forms-65110">AEM 6.5.11.1용 AEM Forms 서비스 팩 11 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.11.html">AEM 6.5.11.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.566-NPR-37836-B0001.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.566-NPR-37836-B0001.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.566-NPR-37836-B0001.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0038/JBoss/Win/AEMForms-6.5.0-0038_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0038/JBoss/Linux/AEMForms-6.5.0-0038_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0038/Weblogic/Win/AEMForms-6.5.0-0038_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0038/Weblogic/Linux/AEMForms-6.5.0-0038_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0038/WebSphere/Win/AEMForms-6.5.0-0038_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0038/WebSphere/Linux/AEMForms-6.5.0-0038_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <br><b>SDK</b></br>
      <li><a href="https://mvnrepository.com/artifact/com.adobe.aemfd/aemfd-client-sdk">AEM Forms 클라이언트 SDK</a>
      </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0038<br /> <p>AEM Forms 추가 기능 패키지: 6.0.566-NPR-37836-B0001</p></td>
   </tr>
   <tr>
    <td>2021년 12월 3일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.11.html#forms-65110">AEM 6.5.11.0용 AEM Forms 서비스 팩 11 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.11.html">AEM 6.5.11.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.566.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.566.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.566.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/JBoss/Win/AEMForms-6.5.0-0037_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/JBoss/Linux/AEMForms-6.5.0-0037_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/JBoss/Solaris/AEMForms-6.5.0-0037_jboss_solaris.tar.gz">JBoss® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/WebLogic/Win/AEMForms-6.5.0-0037_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/WebLogic/Linux/AEMForms-6.5.0-0037_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/WebLogic/Solaris/AEMForms-6.5.0-0037_weblogic_solaris.tar.gz">WebLogic Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/WebSphere/Win/AEMForms-6.5.0-0037_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/WebSphere/Linux/AEMForms-6.5.0-0037_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/WebSphere/Solaris/AEMForms-6.5.0-0037_websphere_solaris.tar.gz">WebSphere® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0037/WebSphere/AIX/AEMForms-6.5.0-0037_websphere_aix.tar.gz">WebSphere® AIX®</a></li>
      <br><b>SDK</b></br>
      <li><a href="https://mvnrepository.com/artifact/com.adobe.aemfd/aemfd-client-sdk">AEM Forms 클라이언트 SDK</a></li>
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0037<br /> </p> AEM Forms 추가 기능 패키지: 6.0.566</p> <p>클라이언트 SDK: 6.0.566<br /></td>
   </tr>
   <tr>
   <tr>
    <td>2021년 9월 2일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.10.html#forms-65100">AEM 6.5.10.0용 AEM Forms 서비스 팩 10 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.10.html">AEM 6.5.10.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.490.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.490.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.490.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.40.zip">AEM Forms 호환성 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/featurepack/livecycle-embed-pkg-5.0.18.zip">JEE의 AEM Forms 임베드 패키지</a></li>
      <br><b>JEE의 AEM Forms 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/JBoss/Win/AEMForms-6.5.0-0032_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/JBoss/Linux/AEMForms-6.5.0-0032_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/JBoss/Solaris/AEMForms-6.5.0-0032_jboss_solaris.tar.gz">JBoss® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/WebLogic/Win/AEMForms-6.5.0-0032_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/WebLogic/Linux/AEMForms-6.5.0-0032_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/WebLogic/solaris/AEMForms-6.5.0-0032_weblogic_solaris.tar.gz">WebLogic Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/WebSphere/win/AEMForms-6.5.0-0032_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/WebSphere/linux/AEMForms-6.5.0-0032_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/WebSphere/Solaris/AEMForms-6.5.0-0032_websphere_solaris.tar.gz">WebSphere® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0032/WebSphere/AIX/AEMForms-6.5.0-0032_websphere_aix.tar.gz">WebSphere® AIX®</a></li>
      <br><b>SDK</b></br>
      <li><a href="https://mvnrepository.com/artifact/com.adobe.aemfd/aemfd-client-sdk">AEM Forms 클라이언트 SDK</a></li>
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0032<br /> </p> AEM Forms 추가 기능 패키지: 6.0.490</p> <p>클라이언트 SDK: 6.0.490<br /> </p><p>AEM Forms 호환성 패키지: 2.0.40</p><p>AEM Forms Designer 패치: 650.017</p><p>JEE의 AEM Forms 임베드 패키지: 5.0.18</p></td>
   </tr>
   <tr>
    <td>2021년 6월 3일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.9.html#forms-6590">AEM 6.5.9.0용 AEM Forms 서비스 팩 9 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.9.html">AEM 6.5.9.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.434.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.434.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.434.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/featurepack/livecycle-embed-pkg-5.0.14.zip">JEE의 AEM Forms 임베드 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/workbench/6-5-0-20210524-1-938669/Workbench_DVD.zip">AEM Forms Workbench</a></li>
      <br><b>JEE 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/jboss/Win/AEMForms-6.5.0-0028_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/jboss/Linux/AEMForms-6.5.0-0028_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/jboss/Solaris/AEMForms-6.5.0-0028_jboss_solaris.tar.gz">JBoss® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/weblogic/win/AEMForms-6.5.0-0028_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/weblogic/linux/AEMForms-6.5.0-0028_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/weblogic/solaris/AEMForms-6.5.0-0028_weblogic_solaris.tar.gz">WebLogic Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/websphere/win/AEMForms-6.5.0-0028_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/websphere/linux/AEMForms-6.5.0-0028_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/websphere/solaris/AEMForms-6.5.0-0028_websphere_solaris.tar.gz">WebSphere® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/aemforms-6-5-0-0028/websphere/aix/AEMForms-6.5.0-0028_websphere_aix.tar.gz">WebSphere® AIX®</a></li>
      <li>AEM Forms 클라이언트 SDK [1]</li>  
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0028<br /> </p> AEM Forms 추가 기능 패키지: 6.0.434</p> <p>클라이언트 SDK: 6.0.434<br /> </p><p>AEM Forms Workbench: 6.5.0.20210524.1.938669</p><p>JEE의 AEM Forms 임베드 패키지: 5.0.14</p></td>
   </tr>
   <tr>
    <td>2021년 3월 18일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.8.html#forms-6580">AEM 6.5.8.0용 AEM Forms 서비스 팩 8 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.8.html">AEM 6.5.8.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.334.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.334.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.334.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.36.zip">AEM Forms 호환성 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/Designer-Patch/650-014/aem-forms-designer-6.5.0-English.msp">AEM Forms Designer 패치</a></li>
      <br><b>JEE 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/JBoss/Win/AEMForms-6.5.0-0025_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/JBoss/Linux/AEMForms-6.5.0-0025_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/JBoss/Solaris/AEMForms-6.5.0-0025_jboss_solaris.tar.gz">JBoss® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/WebLogic/Win/AEMForms-6.5.0-0025_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/WebLogic/Linux/AEMForms-6.5.0-0025_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/WebLogic/Solaris/AEMForms-6.5.0-0025_weblogic_solaris.tar.gz">WebLogic Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/WebSphere/Win/AEMForms-6.5.0-0025_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/WebSphere/Linux/AEMForms-6.5.0-0025_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/WebSphere/Solaris/AEMForms-6.5.0-0025_websphere_solaris.tar.gz">WebSphere® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0025/WebSphere/AIX/AEMForms-6.5.0-0025_websphere_aix.tar.gz">WebSphere® AIX®</a></li>
      <li>AEM Forms 클라이언트 SDK [1]</li>  
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0025<br /> </p> AEM Forms 추가 기능 패키지: 6.0.334</p> <p>AEM Forms 호환성 패키지: 2.0.36</p><p>클라이언트 SDK: 6.0.334<br /> </p><p>AEM Forms Designer 패치: 650.014</p></td>
   </tr>
   <tr>
   <tr>
    <td>2020년 12월 3일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.7.html#forms-6570">AEM 6.5.7.0용 AEM Forms 서비스 팩 7 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.7.html">AEM 6.5.7.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.234.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.234.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.234.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/adobe-aemfd-compat-pkg-2.0.32.zip">AEM Forms 호환성 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/adobe-lc-mobileworkspace-src-2.5.24.zip">AEM Forms 앱 소스</a></li>
      <br><b>JEE 패치 설치 관리자</b></br>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Jboss/Win/AEMForms-6.5.0-0020_jboss_win.zip">JBoss® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Jboss/Linux/AEMForms-6.5.0-0020_jboss_linux.tar.gz">JBoss® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Jboss/Solaris/AEMForms-6.5.0-0020_jboss_solaris.tar.gz">JBoss® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Weblogic/Win/AEMForms-6.5.0-0020_weblogic_win.zip">WebLogic Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Weblogic/Linux/AEMForms-6.5.0-0020_weblogic_linux.tar.gz">WebLogic Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Weblogic/Solaris/AEMForms-6.5.0-0020_weblogic_solaris.tar.gz">WebLogic Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Websphere/Win/AEMForms-6.5.0-0020_websphere_win.zip">WebSphere® Windows</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Websphere/Linux/AEMForms-6.5.0-0020_websphere_linux.tar.gz">WebSphere® Linux</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Websphere/Solaris/AEMForms-6.5.0-0020_websphere_solaris.tar.gz">WebSphere® Solaris™</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEMForms-6-5-0-0020/Websphere/AIX/AEMForms-6.5.0-0020_websphere_aix.tar.gz">WebSphere® AIX®</a></li>
      <li>AEM Forms 클라이언트 SDK [1]</li>  
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: AEMForms-6.5.0-0020<br /> </p> AEM Forms 추가 기능 패키지: 6.0.234</p> <p>AEM Forms 호환성 패키지: 2.0.32</p><p>클라이언트 SDK: 6.0.234<br /> </p></td>
   </tr>
   <tr>
    <td>2020년 9월 3일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.6.html#forms-6560">AEM 6.5.6.0용 AEM Forms 서비스 팩 6 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.6.html">AEM 6.5.6.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-linux-pkg-6.0.192.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-win-pkg-6.0.192.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/adobe-aemfd-osx-pkg-6.0.192.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a> </li>  
      <li>AEM Forms 클라이언트 SDK [1]</li>
      <li>AEM Forms JEE 설치 관리자 [1]</li>
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: 6.5.0-0018<br /> </p> AEM Forms 추가 기능 패키지: 6.0.192</p> <p>클라이언트 SDK: 6.0.192<br /> </p> <p>AEM Forms Designer 패치: 650.012<br /> </p> </td>
   </tr>
   <tr>
    <td>2020년 6월 4일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.5.html#forms-6550">AEM 6.5.5.0용 AEM Forms 서비스 팩 5 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.5.html">AEM 6.5.5.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.5.0-LX.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.5.0-WIN.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.5.0-OSX.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a> </li>  
      <li>AEM Forms 클라이언트 SDK [1]</li>
      <li>AEM Forms JEE 설치 관리자 [1]</li>
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: 6.5.0-0014<br /> </p> <p>AEM Forms 추가 기능 패키지: 6.0.160</p> <p>클라이언트 SDK: 6.0.160<br /> </p> <p>AEM Forms Designer 패치: 650.008<br /> </p> </td>
   </tr>
   <tr>
    <td>2020년 3월 5일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.4.html#forms-6540">AEM 6.5.4.0용 AEM Forms 서비스 팩 4 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.4.html">AEM 6.5.4.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.4.0-LX.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.4.0-WIN.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.4.0-OSX.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/AEM-FORMS-6.5.3.0-COMPAT.zip">AEM Forms 호환성 패키지 [3]</a></li>
      <li>AEM Workbench [1]</li>
      <li>AEM Forms 클라이언트 SDK [1]</li>
      <li>AEM Forms JEE 설치 관리자 [1]</li>
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: 6.5.0-0011<br /> </p> <p>AEM Forms 호환성 패키지: 2.0.26<br /> AEM Forms 추가 기능 패키지: 6.0.138</p> <p>클라이언트 SDK: 6.0.136<br /> </p> <p>AEM Forms Workbench: 6.5.0.20191119.1.935956<br /> </p> </td>
   </tr>
   <tr>
    <td>2019년 12월 12일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.3.html#forms-6530">AEM 6.5.3.0용 AEM Forms 서비스 팩 3 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.3.html">AEM 6.5.3.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.3.0-LX.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.3.0-WIN.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.3.0-OSX.zip">macOS X용 AEM Forms 추가 기능 패키지 [2]</a> </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/AEM-FORMS-6.5.3.0-COMPAT.zip">AEM Forms 호환성 패키지</a></li>
      <li>AEM Workbench [1]</li>
      <li>AEM Forms 클라이언트 SDK [1]</li>
      <li>AEM Forms JEE 설치 관리자 [1]</li>
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: 6.5.0-0007</p> <p>AEM Forms 호환성 패키지: 2.0.26</p> <p>AEM Forms 추가 기능 패키지 및 클라이언트 SDK: 6.0.122</p> <p>AEM Forms Workbench: 6.5.0.20191119.1.935956</p> </td>
   </tr>
   <tr>
    <td>2019년 9월 19일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.2.html#forms-6520">AEM 6.5.2.0용 AEM Forms 서비스 팩 2 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.2.html">AEM 6.5.2.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.2.0-LX.zip">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.2.0-WIN.zip">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-FORMS-6.5.2.0-OSX.zip">macOS X용 AEM Forms 추가 기능 패키지</a> [2] </li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/AEM-FORMS-6.5.2.0-COMPAT.zip">AEM Forms 호환성 패키지</a></li>
      <li>AEM Workbench <sup>[1]</sup></li>
      <li>AEM Forms 클라이언트 SDK [1]</li>
      <li>AEM Forms JEE 설치 관리자<sup> [1]</sup></li>
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: 6.5.0-0004_3</p> <p>AEM Forms 호환성 패키지: 2.0.22</p> <p>AEM Forms 추가 기능 패키지 및 클라이언트 SDK: 6.0.106</p> <p>AEM Forms Workbench: 6.5.0.20190917.1.337048</p> </td>
   </tr>
   <tr>
    <td>2019년 7월 3일</td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.1.html#forms">AEM 6.5.1.0용 AEM Forms 서비스 팩 1 Forms 추가 기능 패키지</a></td>
    <td><a href="https://experienceleague.adobe.com/docs/experience-manager-65/release-notes/service-pack/6.5.1.html">AEM 6.5.1.0</a></td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-Forms-6.5.1.0-LX" target="_blank">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-Forms-6.5.1.0-WIN">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/servicepack/fd/AEM-Forms-6.5.1.0-OSX">macOS X용 AEM Forms 추가 기능 패키지</a><sup> [2] </sup></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/compatpack/AEM-FORMS-6.5.1.0-COMPAT.zip">AEM Forms 호환성 패키지</a></li>
      <li><a href="https://licensing.adobe.com/">AEM Designer 설치 관리자</a> <sup>[1]</sup></li>
      <li>AEM Forms JEE 설치 관리자<sup> [1]</sup><br /> </li>
     </ul> </td>
    <td><p>AEM Forms JEE 설치 관리자: 6.5.0-0004</p> <p>AEM Forms Designer 패치: 6.5.0-005</p> <p>AEM Forms 호환성 패키지:<strong> </strong>1.1.16</p> <p>AEM Forms 추가 기능 패키지: 6.0.88</p> </td>
   </tr>
   <tr>
    <td>2019년 4월 08일</td>
    <td>AEM 6.5 Forms 추가 기능 패키지</td>
    <td>AEM 6.5</td>
    <td>
     <ul>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/AEM-FORMS-6.5-LX">Linux용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/AEM-FORMS-6.5-WIN">Windows용 AEM Forms 추가 기능 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/AEM-FORMS-6.5-OSX">macOS X용 AEM Forms 추가 기능 패키지</a><sup> [2]</sup></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/AEM-FORMS-6.5-WEBSPHERE-GLOBALSEC-CONFIG">AEM WebSphere® 전역 보안 구성 패키지</a> </li>
      <li><a href="https://licensing.adobe.com/">AEM Forms JEE 설치 관리자</a><sup> [1]</sup></li>
      <li><a href="https://licensing.adobe.com/">AEM Workbench</a> <sup>[1]</sup></li>
      <li><a href="https://licensing.adobe.com/">AEM Designer 설치 관리자</a> <sup>[1]</sup></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/AEM-FORMS-6.5-FORMS-APP-SRC-PKG">AEM Forms 앱 소스</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/AEM-FORMS-6.5-FSI-REF-SITE">AEM Forms FSI 참조 사이트 패키지</a></li>
      <li><a href="https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq650/fd/AEM-FORMS-6.5-GOV-REF-SITE">AEM Forms Gov 참조 사이트 패키지</a></li>
     </ul> </td>
    <td><p>AEM Forms 추가 기능 패키지 및 클라이언트 SDK: 6.0.80</p> <p>AEM WebSphere® 전역 보안 구성 패키지: 6.5.0.20190329.1.935745</p> <p>AEM Forms 앱 소스: 5.0.16</p> <p> </p> </td>
   </tr>
  </tbody>
 </table>

`[1]` 워크벤치, Rights Management SDK, PPL(Portable Protection Library) 및 향상된 PPL의 설치 관리자를 받으려면 [Adobe 지원 센터](https://experienceleague.adobe.com/?support-solution=General&amp;support-tab=home#support)에 문의하십시오.

`[2]` macOS X용 AEM [!DNL Forms] 추가 기능 패키지는 프로덕션 환경에서 지원되지 않으므로 데모용으로만 사용해야 합니다. macOS X 패키지에서는 PDF Generator 기능을 사용할 수 없습니다.

`[3]` 6.5.4.0용 AEM [!DNL Forms] 호환성 패키지는 6.5.3.0 릴리스와 동일하게 유지됩니다.

## 기억해야 할 사항 {#things-to-remember}

* 위에 나열된 AEM Forms 추가 기능 패키지는 OSGi의 AEM [!DNL Forms] 및 JEE의 AEM [!DNL Forms]에 모두 적용할 수 있습니다.
* 모든 AEM [!DNL Forms] 추가 기능 패키지 및 빠른 수정 사항은 누적됩니다. 즉, 추가 기능 패키지 및 빠른 수정에는 해당 버전의 구성 요소에 대한 이전 모든 추가 기능과 빠른 수정 사항이 포함되어 있습니다. 예를 들어 빠른 수정 2.4.50을 설치하는 경우 이미 AEM [!DNL Forms] 추가 기능 패키지 2.4.26이 포함되어 있습니다.

  >[!NOTE]
  >
  >누적 추가 기능 패키지와 빠른 수정 사항은 처음 두 개 숫자 버전이 동일함을 의미합니다.

* 항상 사용 가능한 최신 서비스 팩/기능 팩 추가 기능을 설치하십시오. 기본 버전의 일반 공급 이후에 릴리스된 보안, 성능, 안정성 및 주요 고객 수정 사항 및 개선 사항이 포함되므로 적극 권장합니다.
* 서비스 팩을 설치하거나 이전 버전의 AEM에서 최신 버전으로 업그레이드할 때마다 항상 해당 AEM [!DNL Forms] 추가 기능 패키지를 설치하십시오. 예를 들어 AEM 6.1 [!DNL Forms] 추가 기능 패키지 버전 2.2.4에서 AEM 6.1 서비스 팩 1로 업그레이드하는 경우 AEM 6.1 서비스 팩 1을 설치한 후 AEM [!DNL Forms] 추가 기능 패키지 버전 2.4.50을 설치하십시오.
* AEM [!DNL Forms] 추가 기능 패키지의 제거가 지원되지 않습니다.
