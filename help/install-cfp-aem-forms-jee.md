---
title: AEM Forms JEE에 누적 수정 팩 설치
description: AEM Forms JEE에 CFP(누적 수정 팩)를 설치 및 구성하는 단계 요약
contentOwner: AK
exl-id: eed01a42-f4ab-4392-8b8e-eb5bbe2410a0
source-git-commit: 5a549a95acf4d1b78b9040411c9e1720911afeb9
workflow-type: ht
source-wordcount: '910'
ht-degree: 100%

---

# AEM[!DNL  Forms] JEE에 누적 수정 팩 설치{#installing-cumulative-fix-packs-on-aem-forms-jee}

## AEM 6.3 [!DNL Forms JEE]에 CFP 설치 {#install-cfp-forms-6-3}

AEM 6.3 [!DNL Forms JEE]에 누적 수정 팩을 설치하려면 다음 일련의 단계를 수행하십시오.

1. CFP에 대한 AEM 6.3 [!DNL Forms JEE] 설치 관리자를 얻으려면 [Adobe 지원 센터](https://experienceleague.adobe.com/?support-solution=General&amp;support-tab=home#support)에 문의하십시오.
1. [AEM 설치 및 구성 [!DNL Forms JEE]](#install-and-configure-aem-forms-jee)의 설명에 따라 CFP 설치 관리자를 실행하고 AEM [!DNL Forms JEE]를 구성하십시오.
1. 최신 AEM CFP 6.3.3.x 설치
1. AEM CFP [6.3.3.x](aem-forms-releases.md)용 [!DNL Forms] 추가 기능 패키지 설치

### AEM [!DNL Forms JEE] 번들 패키지 설치 {#install-aem-forms-jee-bundles-package}

AEM [!DNL  Forms JEE] 패키지(aemfd-jee-bundles-package-6.3CFP1, 버전 1.0.2)에서는 AEM [!DNL Forms JEE]의 [!DNL Forms] 사용자에게 AEM [!DNL Forms OSGi]의 사용자와 동일한 권한 및 기능을 제공합니다. 패키지 관리자에서 설치된 패키지를 확인하고 아직 설치하지 않은 경우 패키지를 설치합니다.

### CQ-4208044에 대한 추가 지침 {#additional-instructions-for-cq}

AEM 6.3 [!DNL Forms JEE] 서버를 Oracle 데이터베이스와 함께 사용하는 경우, 구성 관리자를 실행한 후 CFP1을 배포하고 다음 설정을 구성합니다. 이 설정은 엔터프라이즈 도메인 동기화가 실행될 때 사용자, 그룹 및 그룹 구성원을 동기화하는 데 필요합니다.

1. **관리** UI에 로그인합니다.
1. **[!UICONTROL 설정]** > **[!UICONTROL 사용자 관리]** > **[!UICONTROL 구성]** > **[!UICONTROL 구성 파일 가져오기 및 내보내기]**&#x200B;로 이동합니다.
1. config.xml 파일을 내보냅니다.
1. *config.xml*&#x200B;의 도메인 구성 아래에 있는 &quot;`groupMemberDBQueryBatchSize`&quot;의 항목을 수정합니다. 샘플 항목:

   &lt;entry key=&quot;groupMemberDBQueryBatchSize&quot; value=&quot;999&quot;/>

1. 수정된 파일을 다시 가져온 다음 동기화를 다시 실행합니다.

## AEM 6.2 [!DNL  Forms JEE]에 CFP 설치 {#install-cfp-on-aem-62-forms-jee}

AEM 6.2 [!DNL Forms JEE]에 누적 수정 팩을 설치하려면 다음 일련의 단계를 수행하십시오.

1. CFP에 대한 AEM 6.2 [!DNL Forms JEE] 설치 관리자를 얻으려면 [Adobe 지원 센터](https://experienceleague.adobe.com/?support-solution=General&amp;support-tab=home#support)에 문의하십시오.
1. [AEM 설치 및 구성 [!DNL Forms JEE]](install-cfp-aem-forms-jee.md#install-and-configure-aem-forms-jee)의 설명에 따라 CFP 설치 관리자를 실행하고 AEM [!DNL Forms JEE]를 구성하십시오.
1. AEM 핫픽스 12785 버전 7.0을 설치합니다.
1. AEM 6.2 서비스 팩 1을 설치합니다.
1. 최신 release-notes-aem-6-2-cumulative-fix-pack.md를 설치합니다.
1. AEM 6.2 서비스 팩 1 CFP의 [!DNL Forms] 추가 기능 패키지를 설치하십시오.

### AEM [!DNL Forms JEE] 번들 패키지 설치 {#install-aem-forms-jee-bundles-package-1}

AEM Forms JEE 패키지(aemfd-jee-bundles-package-6.2CFP5, 버전 1.0.2)에서는 AEM [!DNL Forms JEE]의 [!DNL Forms] 사용자에게 AEM [!DNL Forms OSGi]의 사용자와 동일한 권한 및 기능을 제공합니다. 패키지 관리자에서 설치된 패키지를 확인하고 아직 설치하지 않은 경우 패키지를 설치합니다.

### 구성 요소 수준에서 작업에 대한 시간 제한 구성(NPR-16774) {#configuring-timeout-for-operations-at-component-level-npr}

>[!NOTE]
>
>AEM 6.2 CFP4 이후에는, 업그레이드 프로세스 중 시간 초과로 인해 문제가 발생할 경우 다음 지침에 따라 DSC 작업에 대한 시간 제한을 구성할 수 있습니다.

DSC 배포의 소요 시간은 달라질 수 있어 실패의 원인이 됩니다. 설치, 로드, 시작, 중지 등의 DSC 작업에 대한 시간 제한을 변경하려면 -D 옵션과 함께 JVM 인수를 사용하여 `adobe.component.registry.timeout`을 설정해야 합니다.

키 값을 초 단위로 지정합니다. 예를 들어`-Dadobe.component.registry.timeout=300`

다음 3가지 속성을 사용하여 구성 요소 수준에서 시간 제한을 변경할 수도 있습니다.

1. `adobe.all-component.timeout`: 제품 내의 모든 서비스의 시간 제한을 덮어씁니다.
1. `adobe.<serviceName>.timeout`: 키에 언급된 서비스(&lt;serviceName>)에 대해서만 시간 제한을 덮어씁니다. 서비스 수준의 값이 설정된 경우 이 명령을 사용하면 지정된 서비스가 애플리케이션 수준에서 설정된 경우에만 해당 서비스에 대한 시간 초과 값을 덮어씁니다.
1. `adobe.<serviceName>.<operationName>.timeout`: 키에 언급된 특정 서비스의 작업 시간 제한(&lt;serviceName>&lt;operationName>)만 덮어씁니다. 이 값이 작업 수준에서 설정된 경우, 이 명령을 사용하면 지정된 서비스가 애플리케이션 수준 또는 서비스 수준에서 설정된 경우에만 해당 서비스에 대한 시간 제한 값을 덮어씁니다.

**예:**

다음 명령을 사용하여 구성 요소 수준에서 시간 제한을 설정합니다.

1. 모든 서비스 작업의 시간 제한을 600초로 설정하려면 다음 작업을 수행합니다.

   `JAVA_OPTS=%JAVA_OPTS% -Dadobe.all-component.timeout=600` 설정

1. `DesigntimeService` 작업 값 시간 제한을 500초로 설정하려면 다음을 사용합니다.

   `JAVA_OPTS=%JAVA_OPTS% -Dadobe.DesigntimeService.timeout=500` 설정

1. `DesigntimeService's previewLCA` 작업 값 시간 제한을 700초로 설정하려면 다음을 사용합니다.

   `"JAVA_OPTS=%JAVA_OPTS% -Dadobe.DesigntimeService.previewLCA.timeout=700` 설정

1. 로드 및 설치와 같은 `DSC operations`을 600초로 설정하려면 다음을 사용합니다.

   “`JAVA_OPTS=%JAVA_OPTS% -Dadobe.component.registry.timeout=600`” 설정

## AEM [!DNL Forms JEE] 설치 및 구성 {#install-and-configure-aem-forms-jee}

1. /deploy 폴더의 백업을 수행합니다. 빠른 수정 사항을 제거하려는 경우 필요합니다.
1. 애플리케이션 서버를 중지합니다.
1. 패치 설치 관리자 아카이브 파일을 하드 드라이브에 추출합니다.
1. 사용 중인 운영 체제에 따라 이름이 지정된 디렉터리에서 다음 작업을 수행합니다.

   **Windows**

   설치 관리자를 복사한 하드 디스크의 설치 미디어 또는 폴더로 이동합니다.

   * (Windows 32비트): Disk1\InstData\Windows\VM
   * (Windows 64비트): Disk1\InstData\Windows_64bit\VM

   그리고 다음 파일을 더블 클릭합니다.

   * aemforms63_cfp_install.exe **(AEM [!DNL Forms] 6.3**)
   * aemforms62_cfp_install.exe **(AEM [!DNL Forms] 6.2**)
   * aemforms61_cfp_install.exe(**AEM [!DNL Forms] 6.1**)

   **Linux®, Solaris™, AIX®**

   적절한 디렉터리로 이동합니다.

   * (Linux®): Disk1/InstData/Linux/ NoVM
   * (Solaris™): Disk1/InstData/Solaris/ NoVM
   * (AIX®): Disk1/InstData/AIX/VM

   명령 프롬프트에서 다음을 입력합니다.

   * ./aemforms63_cfp_install.bin(**AEM [!DNL Forms] 6.3**)
   * ./aemforms62_cfp_install.bin(**AEM [!DNL Forms] 6.2**)
   * ./aemforms61_cfp_install.bin(**AEM [!DNL Forms] 6.1**)

   설치 마법사가 시작되어 설치 과정을 안내합니다.

1. 소개 패널에서 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.
1. 설치 폴더 선택 화면에서 표시되는 기본 위치가 기존 설치에 맞는지 확인하거나 **[!UICONTROL 찾아보기]**&#x200B;를 클릭하여 AEM [!DNL Forms]가 설치된 대체 폴더를 선택하고 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.
1. 빠른 수정 패치 요약 정보를 읽고 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.
1. 사전 설치 요약 정보를 읽고 **[!UICONTROL 설치]**&#x200B;를 클릭합니다.
1. 설치가 완료되면 **[!UICONTROL 다음]**&#x200B;을 클릭하여 설치된 파일에 빠른 수정 업데이트를 적용합니다.
1. 기본적으로 구성 관리자 시작 확인란이 선택됩니다. **[!UICONTROL 완료]**&#x200B;를 클릭하여 구성 관리자를 실행합니다.

   나중에 구성 관리자를 실행하려면 **[!UICONTROL 완료]**&#x200B;를 클릭하기 전에 **[!UICONTROL 구성 관리자 시작]** 옵션을 선택 해제합니다. *`[AEM_forms_root]`/configurationManager/bin* 디렉터리에 있는 적절한 스크립트를 사용하여 나중에 구성 관리자를 시작할 수 있습니다.

1. 애플리케이션 서버에 따라 다음 문서 중 하나를 선택하고 *AEM[!DNL Forms]* 구성 및 배포 섹션의 지침을 따릅니다.

   AEM [!DNL Forms] 6.3의 경우 다음을 참조하십시오.

   * JBoss®용 AEM [!DNL Forms] 설치 및 배포
   * WebSphere®용 AEM [!DNL Forms] 설치 및 배포
   * WebLogic용 AEM [!DNL Forms] 설치 및 배포

1. AEM [!DNL Forms] JEE 서버를 다시 시작합니다.
