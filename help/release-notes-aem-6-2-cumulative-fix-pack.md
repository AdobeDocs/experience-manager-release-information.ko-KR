---
title: AEM 6.2 누적 수정 팩
description: AEM 6.2 누적 수정 팩 릴리스 노트.
source-git-commit: 69f4db4e2ef94c370ed590ec7e9859781a909270
workflow-type: tm+mt
source-wordcount: '19928'
ht-degree: 99%

---

# AEM 6.2 누적 수정 팩 릴리스 노트{#release-notes-aem-cumulative-fix-pack}

<!-- TBD: Should we keep this article published after AEM 6.2 content is archived via UGP-1894. If an AEM version is EOL should we discard its details RNs but still retain its docs?
-->

## 릴리스 노트 {#release-information}

| **제품** | Adobe Experience Manager |
|---|---|
| **버전** | 6.2 |
| **릴리스** | 누적 수정 팩 6.2 SP1-CFP20 |
| **전제 조건** | [AEM 6.2 서비스 팩 1](https://docs.adobe.com/docs/en/aem/6-2/release-notes/sp1.html) |
| **일반 출시** | 2019년 6월 06일 |

### 누적 수정 팩 {#cumulative-fix-pack}

Adobe는 수정 사항을 릴리스하기 위해 단일 제공 모델을 도입했습니다. Adobe는 이제 개별 문제에 대한 핫픽스를 릴리스하지 않고 매달 CFP(누적 수정 팩)를 릴리스합니다(품질 검사 통과 여부에 따름). CFP는 여러 수정 사항을 집계한 콘텐츠 패키지로, 주로 버그 수정 사항이 포함되지만, 기능 팩이 포함될 수도 있습니다. 개별 핫픽스 릴리스와 비교해 다음과 같은 이점이 있습니다.

* 기본적으로 누적(예: CFP에 이전 CFP를 통해 게재된 수정 사항이 포함됨)
* 개선된 품질 보증
* 간단한 설치(사용자가 최신 서비스 팩을 제외하고, 종속성이 없는 단일 패키지로 CFP를 설치함)

CFP 및 기타 릴리스 유형에 대한 자세한 내용은 [유지 관리 릴리스 수단](https://docs.adobe.com/content/docs/ko-KR/aem/6-2/deploy/maintenance-release-vehicle-definitions.html)을 참조하십시오.

## 릴리스 노트 {#about-the-release}

AEM 누적 수정 팩 6.2 SP1-CFP20은 AEM 6.2의 마지막 누적 수정 팩이며 [AEM 6.2 SP1](https://helpx.adobe.com/experience-manager/6-2/release-notes/sp1.html)의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

>[!CAUTION]
>
>설치된 기능 팩 간의 호환성을 확인하지 않고 CFP를 적용하면 시스템 오류가 발생하거나 사용자 지정 구성이 손실될 수 있으며, 이를 해결하기 위해 백업에서 복원해야 할 수 있습니다.

>[!NOTE]
>
>* 새 Sling `discovery-  api` 번들 Johnzon 1.0.0은 AEM 누적 수정 팩 6.2 SP1-CFP10에 포함되어 있습니다. 또한 서비스 사용자 sling-discovery는 CRX 저장소의 노드 */var/discovery*&#x200B;에 대한 읽기 및 쓰기 권한이 있는 상태로 추가됩니다.
>
>* **com.day.commons.osgi.wrapper/com.day.commons.osgi.wrapper.commons-email/1.2.0-0002**&#x200B;를 대체하는 apache commons **org.apache.commons/commons-email/1.5**&#x200B;의 이메일 번들입니다.
>
>* Adobe에서는 AEM 인스턴스의 사용자가 많은 고객을 위해 설치 폴더를 통해 CFP를 배포하도록 권장합니다.

>


## 포함된 문제 {#issues-included}

이 섹션에는 현재 CFP에 포함된 모든 문제와 핫픽스가 나와 있습니다.

또한 이 CFP에는 [이전 누적 수정 팩](#previous)에 제공된 핫픽스가 포함되어 있습니다.

### 통합 {#integration}

* 여러 캠페인 타깃팅 개인화 개선 사항을 지원합니다. NPR-29163: CQ-4264126용 핫픽스
* com.day.cq.personalization.impl.TeaserResourceEventHandler가 무한 루프로 이동하고 게시 인스턴스의 노드에 대한 업데이트가 발생합니다. NPR-28561: CQ-4263096용 핫픽스

### DAM - 일반 {#dam-general}

* 관리자가 아닌 사용자를 위해 특정 dam 폴더에서 복제 버튼을 표시하거나 숨길 수 없습니다. NPR-29026: CQ-4265361용 핫픽스

### 취약성 {#vulnerability}

* CSRF 보호 프레임워크가 AEM Foundation Forms에서 작동하지 않습니다. NPR-28612: GRANITE-22231용 핫픽스

### 양식 {#forms}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package}

>[!NOTE]
>
>AEM Forms 고객의 경우 AEM 서비스 팩, 누적 수정 팩 또는 기능 팩을 설치한 후 AEM Forms 추가 기능 패키지를 설치해야 합니다.

>[!NOTE]
>
>AEM Forms 추가 기능 패키지는 양식 기능을 AEM 서비스 팩 및 누적 수정 팩과 맞추는 데 도움이 됩니다. 따라서 반드시 AEM 서비스 팩, 누적 수정 팩 또는 기능 팩을 설치한 후 AEM Forms 추가 기능 패키지를 설치해야 합니다.

#### 적응형 양식 {#adaptive-forms}

* iOS 12.1 디바이스용 스크리블 구성 요소 사용 문제 NPR-29082: CQ-4261765용 핫픽스

#### 양식 - 문서 보안 {#forms-document-security}

* PAdES(PDF 고급 전자 서명)를 사용하여 PDF에서 모든 서명을 확인하면 InvalidOperationException이 발생합니다. NPR-27848: CQ-4244837용 핫픽스

#### Forms - 서신 {#forms-correspondence}

* 편지를 PDF로 미리 볼 때 마스터 페이지에 배치된 텍스트 필드에 데이터 탭에서 입력한 값이나 지정된 데이터 링크 내용이 적용되지 않습니다. NPR-29239: CQ-4266856용 핫픽스.

#### 양식 - 대화형 통신 {#forms-interactive-communication}

* 아포스트로피 문자를 추가하면 편지에 미리 입력된 필드가 일반 알파벳이 아닌 ASCII 문자로 표시됩니다. NPR-28863: CQ-4262900용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer}

* Forms JEE 설치 관리자에서 새 AEM Forms가 수정되지 않습니다.

## 이전 누적 수정 팩에 포함된 핫픽스 및 기능 팩 {#hotfixes-and-feature-packs-included-in-previous-cumulative-fix-packs}

### 누적 수정 팩 19 {#cumulative-fix-pack-1}

AEM 누적 수정 팩 6.2 SP1-CFP19는 [AEM 6.2 SP1](https://helpx.adobe.com/experience-manager/6-2/release-notes/sp1.html)의 일반 공급 이후 릴리스된 주요 고객 수정 사항을 포함하는 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* AEM 6.2에 대한 MS Translator API v3.0 지원이 활성화되었습니다.
* 모든 SP, CFP 및 HF 패키지를 설치한 후 로그 메시지가 추가되었습니다.

### 자산 {#assets}

* ACL 편집 권한이 없으면 DAM 폴더의 이름을 변경할 수 없습니다. NPR-27555: CQ-104652용 핫픽스
* 6.2.1 CFP 17 이상에서 이미지 사전 설정 편집기 도구가 응답하지 않습니다. NPR-28147: CQ-4261041용 핫픽스

### 사이트 {#sites}

* 링크 확인 작업이 완료되지 않고 링크가 응답하지 않아 정지 상태가 됩니다. NPR-27373: CQ-4256030용 핫픽스
* 세그먼트의 경로를 벗어나는 추가 루트 경로로 인해 세그먼트 파일이 제대로 로드되지 않습니다. NPR-28014: CQ-4260332용 핫픽스

### 통합 {#integration-1}

* LiveCopy 상속 취소가 타깃팅된 컨테이너에서 제대로 작동하지 않습니다. NPR-28129: CQ-4259813용 핫픽스
* cq: 작업은 타깃팅된 구성 요소에서 고려하지 않습니다. NPR-27616: CQ-4257497용 핫픽스

* 상속을 중단하기 위한 아이콘 표시에 일관성이 없습니다. NPR-27671: CQ-4257779용 핫픽스

### Felix {#felix}

* AEM 6.2 SP1 인스턴스에 CFP 18을 설치한 후 웹 콘솔 구성 요소 세부 사항이 코드 500으로 실패합니다. NPR-28350: CQ-4261095용 핫픽스

### 번역 {#translation}

* MS Translator를 API v3.0으로 업그레이드하면 AEM 6.3에서 MS Translator 서비스를 지원합니다. NPR-28123: CQ-4259096용 핫픽스

### UI - 기초 {#ui-foundation}

* OOTB 사이트 달력에 잘못된 날짜가 표시됩니다. NPR-28392

### Granite {#granite}

* sling:basename을 사용하는 리소스 번들에 대한 사전은 무효화되지 않습니다. NPR-27624

### 지속성 {#sustenance}

* 패키지 관리자 활동 로그는 별도의 로그 파일에 추출해야 합니다. NPR-27323: Granite-14866용 핫픽스
* 설치가 완료될 때 표시되는 error.log의 표준화된 구문/문구/로그 라인입니다. NPR-27835
* Granite 패키지 플러그인은 낮은 버전의 org.apache.sling.i18n에 대한 종속성을 선택합니다. CQ-4263245용 핫픽스
* com.adobe.cq.com.adobe.cq.ui.commons 번들은 6.2SP1-CFP15 이후 최신 CFP를 설치할 때 삭제됩니다. CQ-4258808용 핫픽스

### 양식 {#forms-1}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-1}

#### 적응형 양식 {#adaptive-forms-1}

* AEM Forms에 XML 삽입 취약성이 있습니다. NPR-27843: CQ-4257315용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-1}

* Forms JEE 설치 관리자에서 새 AEM Forms가 수정되지 않습니다.

### OSGi 번들 및 콘텐츠 패키지가 포함됨 {#osgi-bundles-and-content-packages-included}

다음 텍스트 문서에는 CFP에 포함된 OSGi 번들 및 콘텐츠 패키지 목록이 있습니다.

AEM 6.2 SP1-CFP19에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/cfp19_osgi_bundles.txt)

AEM 6.2SP1-CFP19에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/cfp19_content_packages.txt)

### 누적 수정 팩 18 {#cumulative-fix-pack-2}

AEM 누적 수정 팩 6.2 SP1-CFP18은 [AEM 6.2 SP1](https://helpx.adobe.com/experience-manager/6-2/release-notes/sp1.html)의 일반 공급 이후 릴리스된 주요 고객 수정 사항을 포함하는 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 오래 실행되는 프로세스를 종료하기 위한 DAM CommandLineProcess 지원이 추가되었습니다.
* ReplicationEventListener의 세션 누수가 수정되었습니다.
* 코어 페이지 구성 요소에 리디렉션 지원을 추가했습니다.

### 자산 {#assets-1}

* Camera Raw 프로세스가 대량의 처리 기간 중 중단되어 그 결과 모든 워크플로 처리가 차단됩니다. NPR-26990: NPR-23860용 핫픽스
* 다운로드 기능은 익명의 사용자가 모든 에셋을 다운로드할 수 있도록 하는 assetdownload 서블릿을 통해 AEM Assets를 활용합니다. NPR-27054, CQ-4254732용 핫픽스
* AEM의 이메일 템플릿의 제목 줄에 특수 문자가 깨진 상태로 표시됩니다. NPR-26470: CQ-4252368용 핫픽스

### 사이트 {#sites-1}

* ConfigPostProcessor 클래스의 잘못된 동작으로 인해 일시 중단 중인 상위 이미지가 cq : LiveRelationship 혼합 유형을 하위 페이지에서 제거합니다. NPR-26745: CQ-4254163용 핫픽스
* 코어 페이지 구성 요소에 리디렉션 지원을 추가했습니다. NPR-26576: CQ-110529용 핫픽스
* 컨텍스트 허브를 jquery 3으로 마이그레이션합니다. NPR-26956: CQ-4255472용 핫픽스
* 앵커 입력 필드는 최대화하기 전까지 대화 상자의 브라우저 표시 섹션 외부에 표시됩니다. NPR-26852: CQ-4255019용 핫픽스
* 콘텐츠 조각에 원하지 않는 &lt;br>을 삽입하는 텍스트를 복사하여 붙여넣습니다. NPR-26660: CRTE-151용 핫픽스
* 클래식 siteadmin은 일부 페이지의 오른쪽 창에 있는 목록을 렌더링하지 않습니다. NPR-27247: CQ-4251621용 핫픽스
* (클래식 UI) 페이지 이동/이름 변경을 시도하면 &quot;페이지 이동 중 오류가 발생했습니다.&quot;라는 오류가 발생합니다. NPR-27179: CQ-4235907용 핫픽스

### 통합 {#integration-2}

* com.day.cq.personalization.impl.BrandsRetriever가 사용 가능한 브랜드를 수집하도록 전체 트리를 안내합니다. NPR-27060: CQ-4255790용 핫픽스

### WCM - Foundation 구성 요소 {#wcm-foundation-components}

* Foundation 목록 구성 요소의 검색 기능 문제. NPR-26817: CQ-4250324용 핫픽스

### 플랫폼 {#platform}

* 특수 문자 em 대시로 인해 게시자에서 캐시를 플러싱하는 문제가 발생했습니다. NPR-27199: CQ-4242790용 핫픽스

### Granite {#granite-1}

* 패키지 유효성 검사기는 CFP/SP에 포함된 패키지의 유효성을 검사하지 않습니다. NPR-26775: Granite-22825용 핫픽스

### 복제 {#replication}

* ReplicationListener의 JCR 세션 누수. NPR-27063: CQ-4232088용 핫픽스

### 양식 {#forms-2}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-2}

* Forms 추가 기능 패키지에서 새 AEM Forms가 수정되지 않습니다.

### Forms JEE 설치 관리자 {#forms-jee-installer-2}

* Forms JEE 설치 관리자에서 새 AEM Forms가 수정되지 않습니다.

#### OSGi 번들 및 콘텐츠 패키지가 포함됨 {#osgi-bundles-and-content-packages-included-1}

AEM 6.2 SP1-CFP18에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/62cfp18updated_bundles.txt)

AEM 6.2 SP1-CFP18에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/content_package_62sp1_cfp18.txt)

### 누적 수정 팩 17 {#cumulative-fix-pack-3}

AEM 누적 수정 팩 6.2 SP1-CFP17은 [AEM 6.2 SP1](https://helpx.adobe.com/experience-manager/6-2/release-notes/sp1.html)의 일반 공급 이후 릴리스된 주요 고객 수정 사항을 포함하는 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* at-integration.js에서 사이트 확장 없는 URL에 대한 지원을 추가했습니다.
* S7 클라우드 서비스 구성에서 S7 폴링 가져오기를 제거했습니다.
* 멀티 테넌트 구현을 위한 폴더 구조를 지원하기 위한 대상 보기의 변경 사항입니다.
* jqueryui clientlib v1.12.1로 업데이트합니다.

### 자산 {#assets-2}

* 에셋 UI에서 워크플로를 시작하려면 사용자에게 쓰기/삭제/수정 권한이 있어야 합니다. NPR-25688: CQ-4250140용 핫픽스
* 복제 권한이 없는 사용자에게도 게시 및 게시 취소 버튼이 계속 표시됩니다. NPR-25094
* (워크플로) 스마트 태그 에셋 워크플로는 AEM 프록시 구성을 통해 처리되지 않습니다. NPR-25915: CQ-4248202용 핫픽스
* S7 클라우드 서비스 구성에서 S7 폴링 가져오기를 제거합니다. NPR-25239: CQ-95236용 핫픽스

### 사이트 {#sites-2}

* 편집기 -> 페이지 정보에서 시작된 워크플로는 페이로드의 컨텍스트 경로를 포함합니다. NPR-26389: CQ-76804용 핫픽스
* (외부 링크 확인) 잘못된 https 링크가 유효한 링크로 표시됩니다. NPR-25541: CQ-4201333용 핫픽스
* (클래식 UI) 라이브 카피 아래에 독립형 페이지를 만들 때 페이지가 라이브 카피로 생성됩니다. NPR-25610: CQ-4249801용 핫픽스
* 페이지가 활성화될 때 디자인 Importer 구성 요소와 연관된 리소스를 게시하는 데 관련된 문제 NPR-25638: CQ-102532용 핫픽스
* RTE 리치 텍스트 도구 모음에는 선택 목록이 있습니다. NPR-25165: CQ-4248948용 핫픽스
* contexthub를 jquery 3으로 마이그레이션합니다. NPR-25059: Granite-19902용 핫픽스
* 중첩된 parsys 구성 요소의 경우, 사용 가능한 여러 구성 요소에서 항상 첫 번째로 만족스러운 디자인(중첩된 경로가 가장 적게 있음)을 적용합니다. 자세한 내용은 [디자인 경로 해상도](https://helpx.adobe.com/experience-manager/6-3/sites/developing/using/page-templates-static.html)를 참조하십시오. NPR-25250: CQ-4246276용 핫픽스

### 통합 {#integration-3}

* OOTB 대상 통합을 사용하여 구성 요소를 타깃팅하면 빈 타깃팅된 구성 요소 대신 전체 페이지가 렌더링됩니다. NPR-25273: CQ-4248003용 핫픽스
* 타깃팅 모드에서 상속을 중단해도 구성 요소는 편집 모드에서 중단되지 않은 상속으로 타깃팅된 것으로 표시됩니다. NPR-25324: CQ-4248162용 핫픽스
* 페이지에 개인화가 정의되어 있고 대상이 해결되면 해당 경험이 편집 모드로 표시됩니다. NPR-25731: CQ-4249465용 핫픽스
* 기본값이 아닌 컨텍스트 경로가 있는 AEM을 사용할 때의 잘못된 티저 URL입니다. NPR-25971: CQ-4250953용 핫픽스
* 옵트아웃 사용 시 빈 렌더링입니다. NPR-25295: CQ-4246792용 핫픽스
* 작성 환경에서 삭제된 경험은 페이지 활성화 시 게시 사이트에서 제거되지 않습니다. NPR-24869: CQ-4247832용 핫픽스

### DAM - DM 클라이언트 {#dam-dm-client}

* (Chrome, Firefox) VideoPlayer는 터치 지원 디바이스에서 마우스 클릭을 무시합니다. CQ-4247370용 핫픽스

### 플랫폼 {#platform-1}

* 패키지를 가져오거나 릴리스할 때 최대 재시도 횟수를 구성할 수 있습니다. NPR-25328: Granite-22376용 핫픽스
* 복제 오류 시 로깅이 잘못되었습니다. NPR-25308: CQ-4249402용 핫픽스
* Forms AEM 6.2 Forms CFP8을 CFP14에 설치하면 Apache POI가 실패합니다. NPR-25053: Granite-21771용 핫픽스

### Granite {#granite-2}

* OakConstraint0022 예외로 인해 사용자 동기화 프로세스가 실패했습니다. NPR-25729: Oak-7428용 핫픽스

### 커뮤니티 {#communities}

* cq -social-as-provider 번들은 mongo 드라이버 3.x 버전에서 시작하지 않습니다. NPR-26271: CQ-4252710용 핫픽스

### UI - 기초 {#ui-foundation-1}

* jqueryui clientlib v1.12.1에 대한 업데이트. NPR-25090: Granite-21981용 핫픽스, CQ-4248897

* (Omnisearch): &#39;Title&#39; 속성은 사이트의 XSS(크로스 사이트) 스크립팅에 취약합니다. NPR-24994: Granite-19933용 핫픽스

### 양식 {#forms-3}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-3}

#### 적응형 양식 {#adaptive-forms-2}

* 적응형 양식에서 데이터를 제출하는 동안 인코딩이 잘못되었습니다. NPR-25539

#### 양식 - 관리 {#forms-management}

* 페이지를 게시하는 동안 관련 없는 양식 에셋이 참조로 보고되었습니다. NPR-26167: CQ-4251004용 핫픽스

### Forms - JEE 설치 관리자 {#forms-jee-installer-3}

#### 문서 보안 {#document-security}

* 변수는 데이터 유형 List로 채워지고 하위 유형은 문자열이지만 &quot;오브젝트를 강제 변환할 수 없습니다.&quot; 오류가 발생합니다. NPR-26194: CQ-4252287용 핫픽스
* 6.2-SP1-CFP15를 설치한 후 워터마크 구성에 액세스할 수 없습니다. NPR-26130: CQ-4250984용 핫픽스

### OSGi 번들 및 콘텐츠 패키지가 포함됨 {#osgi-bundles-and-content-packages-included-2}

AEM 6.2 SP1-CFP17에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/62cfp17updated_bundles.txt)

AEM 6.2SP1-CFP17에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/content_package_62sp1_cfp17_2.txt)

### 누적 수정 팩 16 {#cumulative-fix-pack-4}

AEM 누적 수정 팩 6.2 SP1-CFP16은 [AEM 6.2 SP1](https://helpx.adobe.com/experience-manager/6-2/release-notes/sp1.html)의 일반 공급 이후 릴리스된 주요 고객 수정 사항을 포함하는 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 일별 CQ 메일 서비스에 STARTTLS 지원이 추가되었습니다.
* 프로필 팝오버에서 ContextHub 아이콘 정렬을 수정했습니다.
* 드롭다운 구성 요소의 표시/숨기기 기능이 수정되었습니다.
* 최신 Jackson 버전 2.8.11로 업그레이드

### 자산 {#assets-3}

* 목록 보기에서 워크플로를 시작할 수 없습니다. NPR-24393: CQ-4245788용 핫픽스
* (Firefox/Chrome) 에셋 공유 페이지에서 에셋을 다운로드할 수 없습니다. NPR-24523: CQ-4224408용 핫픽스
* AEM에서의 비디오 미리보기에 대한 기본 품질을 개선했습니다. NPR-24148: CQ-4244310용 핫픽스

### 통합 {#integration-4}

* 구성 요소가 게시 인스턴스에서 타깃팅되면 타깃팅된 구성 요소 전의 기본 경험이 깜박거리는 것처럼 표시됩니다. NPR-23992: CQ-4242038용 핫픽스
* 작성 환경에서 삭제된 경험은 페이지 활성화 시 게시 사이트에서 제거되지 않습니다. NPR-24869: CQ-4247832용 핫픽스

### 플랫폼 {#platform-2}

* 보안 수정 사항을 포함하는 clientlib의 jQuery 1.12.4 패치입니다. NPR-24129: Granite-20058용 핫픽스
* 일별 CQ 메일 서비스에 STARTTLS 지원이 추가되었습니다. NPR-23941: CQ-4240397용 핫픽스
* 기본 MERGE_PRESERVE aclHandling을 제거합니다. NPR-24593: Granite-21889용 핫픽스
* 요청에 잘못된 쿼리 매개 변수가 포함되어 있으면 LineChecker에서 링크를 외부화할 수 없습니다. NPR-24127: CQ-4241893용 핫픽스

### MSM {#msm}

* XSS(크로스 사이트 스크립팅) 공격에 대한 사전 예방적 핫픽스입니다. NPR-21893: CQ-4223385용 핫픽스
* MSM LiveRelationship: BlueprintConfig가 루트에 있는 경우 유효 RolloutConfig가 잘못되었습니다. NPR-23999: CQ-4243000용 핫픽스

### 사이트 {#sites-3}

* 라이브 카피 영역에서 새 경험을 만들려면 구성하는 상속을 중단해야 합니다. NPR-24995, CQ-4248209용 핫픽스
* (Touch UI) 페이지를 잠그거나 잠금 해제할 때 상단 도구 모음에 있는 여러 개의 아이콘이 사라집니다. NPR-23954: CQ-4243345용 핫픽스
* 이 필드가 contexthub에서 올바르게 정렬되지 않습니다. NPR-23958
* 잠긴 페이지에서 게시 작업을 수행하면 작성이 중단됩니다. NPR-23970: CQ-4243203용 핫픽스
* /etc/reports/의 OOTB 보고서가 제대로 작동하지 않고 내역 데이터 그래프가 표시되지 않습니다. NPR-20035: CQ-4220180용 핫픽스
* 프로젝트에서 &#39;실행 요청&#39; 워크플로를 시작하는 동안 Launch 작성에 실패합니다. NPR-24255: CQ-4245030용 핫픽스
* 이메일에 의해 무시된 HTML 태그 및 속성은 CFP10 설치를 게시합니다. NPR-24287: CQ-4240028용 핫픽스
* TagPicker: 태그 메타데이터 스키마 태그 필드의 태그 제안은 태그 가능한 노드를 쿼리하므로 로드하는 데 오랜 시간이 소요됩니다. NPR-24347: CQ-4244291용 핫픽스
* Salesforce 통합이 프록시 구성에서 실패합니다. NPR-24418: CQ-4245300용 핫픽스
* (WCM) PageManager는 개정 생성 중에 예외에서 페이지를 체크인 상태로 유지합니다. NPR-24565: CQ-4246203용 핫픽스
* CFP14를 적용하면 디바이스 에뮬레이터 버튼이 편집 및 미리보기 모드에서 사라집니다. NPR-24566: CQ-4247060용 핫픽스
* (클래식 UI) 대화 상자에서 작성하면 전체 태그가 비어 있는 것으로 표시됩니다. NPR-24688, CQ-4246407용 핫픽스
* 첫 번째 시도에서 버전을 만들 수 없습니다. NPR-24774: CQ-4232176용 핫픽스
* /etc/reports/의 OOTB 보고서가 제대로 작동하지 않고 내역 데이터 그래프가 표시되지 않습니다. NPR-24138: CQ-4220180용 핫픽스

### 취약성 {#vulnerability-1}

* Salesforce 통합은 SSRF(Server Side Request Forgery)에 취약합니다. NPR-24289: CQ-4245277용 핫픽스
* ReportingServicesProxyServlet의 SSRF(Server Side Request Forgery) 취약성 NPR-24657: CQ-4246880용 핫픽스

### Granite {#granite-3}

* 메타데이터 읽기 작업이 종료되지 않습니다. NPR-24240: Granite-19866용 핫픽스
* Jetty를 9.4.11.v20180605으로 업데이트하여 취약점을 해결합니다. NPR-25033: Granite-22120용 핫픽스

### WCM - Foundation 구성 요소 {#wcm-foundation-components-1}

* 페이지를 정렬하는 동안 PageComparator에서 ClassCastException이 발생합니다. NPR-24123: CQ-4244048용 핫픽스
* 양식 드롭다운 구성 요소의 기능 표시/숨기기 기능이 예상대로 작동하지 않습니다. NPR-24562: CQ-4222853용 핫픽스

### 사용자 인터페이스 {#user-interface}

* 관리자 검색 기능의 많은 요청으로 인해 높은 CPU 사용률이 관찰됩니다. NPR-23588: Granite-21286용 핫픽스
* (클래식 UI) 연관된 양식 데이터 모델 서비스가 빈 필드로 설정된 경우에도 구성 요소에 기본값이 표시됩니다. NPR-21903: GRANITE-19744용 핫픽스
* 요청에 대한 FormData가 없을 때 다중 필드에서 NPE가 발생합니다. NPR-24513: Granite-21055용 핫픽스

## 양식 {#forms-4}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-4}

#### 코어 {#core}

* (OSGI) AEM Forms OSGI가 Jackson 데이터 바인딩 보안 경고의 영향을 받습니다. NPR-24274: CQ-4230245용 핫픽스

#### 권한 관리 {#rights-management}

* Apache POI에서 설치 후 AEM 6.2 SP1-CFP14에 실패합니다. NPR-25054, NPR-25052: CQ-4245898, CQ-4244778용 핫픽스

#### HTML5 양식 {#html-forms}

* 데이터는 HTML 미리보기에서 다중 라인 필드의 미리 채우기로 작성되지 않습니다. NPR-23357: CQ-4244212용 핫픽스
* 미리보기 버튼을 클릭할 때는 레이아웃 조각 매핑이 표시되지만 기본 미리보기를 통해 편지를 미리 보는 경우에는 레이아웃 조각 매핑이 표시되지 않습니다. NPR-22993: CQ-4237745용 핫픽스
* 템플릿에 미국 사회 보장 번호 패턴을 적용할 때 텍스트 필드의 HTML 미리보기에서 문제가 발생합니다. NPR-23205

#### 적응형 양식 {#adaptive-forms-3}

* parsys 구성 요소에 AEM 양식을 추가하는 동안 “Guidelib가 정의되지 않았습니다.” 오류가 발생했습니다. NPR-24269: CQ-4244546용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-4}

#### Forms-Install-LCM {#forms-install-lcm}

* Shell 스크립트 파일의 Window 줄 끝으로 인해 LCM이 UNIX에서 실행되지 않습니다. NPR-22958

### OSGi 번들 및 콘텐츠 패키지가 포함됨 {#osgi-bundles-and-content-packages-included-3}

AEM 6.2 SP1-CFP16에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/6_2cfp16_bundlecomparison-list.txt)

AEM 6.2SP1-CFP16에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/6_2cfp16_contentpackage-list.txt)

### 누적 수정 팩 15 {#cumulative-fix-pack-5}

AEM 누적 수정 팩 6.2 SP1-CFP15는 [AEM 6.2 SP1](https://helpx.adobe.com/experience-manager/6-2/release-notes/sp1.html)의 일반 공급 이후 릴리스된 주요 고객 수정 사항을 포함하는 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 디자인 일관성을 유지하기 위한 Foundation 테이블의 사전 보안 수정 사항
* 값을 문자열로 저장하도록 typeHint 지원 추가
* Forms 미리 채우기 서비스에 대한 보안 개선
* Reader 확장의 수정을 위해 최신 adobe-reader-extensions-dsc.jar 파일로 업데이트
* 증폭 번호 입력에 &quot;:invalid&quot; 항목을 고려하도록 유효성 검사 후크 조정

### 자산 {#assets-4}

* EmbedXMP 데이터가 Ptiff 생성 프로세스에 대해 항상 &quot;활성&quot;으로 설정됩니다. NPR-22776: CQ-4234498용 핫픽스
* 복수 값 필드에 기본값을 여러 개 설정할 수 없습니다. NPR-22900: CQ-4239000용 핫픽스
* (Dynamic Media) 동적 렌디션 확인란을 선택하면 다운로드된 zip 파일의 원본 TIFF 이미지가 0바이트 파일로 생성됩니다. NPR-22410: CQ-4198471용 핫픽스
* (Touch UI) 열 보기의 에셋에 대한 기본 업로드 위치입니다. NPR-23475: CQ-4237057용 핫픽스

### 통합 {#integration-5}

* 대상 모드에서 작성자가 상속을 취소하지 않고도 블루프린트에서 상속된 구성 요소를 수정할 수 있습니다. NPR-22751: CQ-4237907용 핫픽스
* 경로 변수가 올바르게 인코딩되지 않아 지속적이지 않은 XSS(교차 사이트 스크립팅)가 발생합니다. NPR-22851

### MSM {#msm-1}

* 다중 롤아웃 구성이 있는 LiveCopy를 롤아웃하는 동안 ResourceNameConflict가 루트 아래에 발생하면 모든 분기를 포함하지 않고 롤아웃 흐름이 종료됩니다. NPR-22842: CQ-4236188용 핫픽스

### 플랫폼 {#platform-3}

* 한 개의 요청에서 역방향 애플리케이션에 대한 폴링 제한을 구현합니다. NPR-23351: Granite-21135용 핫픽스****
* 메시지 패턴 변경이 사용자 정의 로거에는 반영되지 않습니다. NPR-23486: CQ-4241974용 핫픽스

### 사이트 {#sites-4}

* 리치 텍스트 편집기의 텍스트에 공백이나 다른 특수 문자가 있는 문서에 대한 링크를 만들 수 없습니다. NPR-22289: CQ-4224321용 핫픽스
* 큰 값(10000000000)이 있는 세그먼트를 저장하면 증폭이 0으로 설정되어 오류 메시지가 표시됩니다. NPR-22524: CQ-4237006용 핫픽스
* 다중 필드 구성 요소에서 항목 추가를 클릭할 수 없습니다. NPR-22552: CQ-4237404용 핫픽스
* 세그먼트에 긴 제목이 있으면 가로 스크롤바가 표시되지 않습니다. NPR-22615: CQ-4237001용 핫픽스
* 빈 대상을 로드하면 잘못된 JavaScript 코드가 생성됩니다. NPR-22974: CQ-4238734용 핫픽스
* 활성화 또는 비활성화를 예약할 때 워크플로 제목은 필수 항목이므로 사용자 정의 워크플로 제목은 타임라인에서 번역되지 않습니다. NPR-23121: CQ-4237552용 핫픽스
* Sites의 Target 세그먼트 관련 문제에 대한 수정 사항을 요청합니다. NPR-23128
* (Firefox) 선택한 사용자에 대한 확인란이 올바른 확인란이 아닙니다. NPR-23345
* 다른 모드에 대한 레이블은 아이콘과 함께 표시됩니다. NPR-23275
* AEM 6.0에서 AEM 6.2로 구성 요소를 마이그레이션하는 중 &#39;올바르지 않은 재귀 선택기 값&#39; 오류가 발생했습니다. NPR-23503: CQ-4241258용 핫픽스

### 커뮤니티 {#communities-1}

* 메시지 오류로 인해 웹 및 메일 통지가 그룹으로 트리거되지 않습니다. NPR-23447: CQ-4242880용 핫픽스

### 번역 {#translation-1}

* 번역 구성에서 “번역 안 함” 에셋이 설정되면 에셋 언어 사본이 생성됩니다. NPR-22540: CQ-4237962용 핫픽스

### 사용자 인터페이스 {#user-interface-1}

* Omnisearch를 하이픈 쿼리와 함께 사용하면 서버 오류가 반환됩니다. NPR-22999: Granite-19674용 핫픽스
* DatePicker가 숨김 필드에 의해 수동으로 설정된 외부 유형 힌트를 지원하지 않습니다. 이 유형 힌트를 변경하면 변환 오류가 발생합니다. NPR-23333: Granite-21194용 핫픽스

### WCM - Foundation 구성 요소 {#wcm-foundation-components-2}

* 보안 강화를 위해 CAPTCHA 구성 요소를 더 이상 사용하지 않습니다. CAPTCHA 구성 요소를 사용하는 경우 6.2 SP2-CFP15 이후 릴리스를 설치하면 &quot;Captcha 구성 요소는 삭제되었으므로 더 이상 사용해서는 안 됩니다.&quot;라는 메시지가 표시됩니다. 보안 강화를 위해 reCAPTCHA를 포함하도록 AEM 구성 요소를 사용자 지정할 수 있습니다. NPR-22151: CQ-4220052용 핫픽스
* WCM Foundation 구성 요소 &#39;Table&#39;은 저장된 교차 사이트 스크립팅에 취약합니다. NPR-23206: CQ-4240760용 핫픽스

### 취약성 {#vulnerability-2}

* 관리자 UI 프로젝트의 XSS(교차 사이트 스크립팅)가 연결됩니다. NPR-23272: CQ-4241795용 핫픽스

## 양식 {#forms-5}

### Forms 추가 기능 패키지 {#forms-add-on-package-5}

#### 서신 관리 {#correspondence-management}

* 미리보기 버튼을 클릭할 때는 레이아웃 조각 매핑이 표시되지만 기본 미리보기를 통해 편지를 미리 보는 경우에는 레이아웃 조각 매핑이 표시되지 않습니다. NPR-23335: CQ-4237745용 핫픽스
* XDP에 정의된 바인딩에 해당하는 편지의 데이터는 직접 문자 URL을 사용하여 채워지지 않습니다. NPR-24145: CQ-4244290용 핫픽스

#### Mobile Forms {#mobile-forms}

* (서신 관리) 대상 XML로 편지를 로드하는 동안 데이터가 올바르지 않게 정렬됩니다. NPR-22993: CQ-4237663용 핫픽스

#### Reader 확장 서비스 {#reader-extensions-service}

* Adobe PDF에서 Reader 확장을 적용할 수 없습니다. NPR-23067

#### Forms Manager {#forms-manager}

* 사이트에 임베드된 Forms는 사이트 페이지를 다시 게시할 때 게시되지 않습니다. NPR-23014: CQ-4236566용 핫픽스

#### 취약성 {#vulnerability-3}

* 크로스 사이트 스크립팅에 대한 사전 예방적 핫픽스 NPR-20624: CQ-4206055용 핫픽스
* Forms Manager의 메모 탭에 저장된 XSS(교차 사이트 스크립팅)에 취약성이 발견되었습니다. NPR-27157: CQ-4255556용 핫픽스

#### 암호화 서비스 {#encryption-service}

* (OSGI) [JEE] &quot;PDF 유효성 확인 프로세스&quot;를 사용하여 확인하는 동안 PDF에 대한 잘못된 서명 상태가 첨부되어 있습니다. NPR-23269, NPR-23737

### Forms JEE 설치 관리자 {#forms-jee-installer-5}

#### 코어 {#core-1}

* Core-ext의 정적 코드 분석에 보고된 문제를 해결해야 합니다. NPR-13947

#### PDFG 서비스 {#pdfg-service}

* HTML 대 PDF 변환기가 작동하지 않습니다. NPR-21545

### OSGi 번들 및 콘텐츠 패키지가 포함됨 {#osgi-bundles-and-content-packages-included-4}

다음 텍스트 문서에는 CFP에 포함된 OSGi 번들 및 콘텐츠 패키지 목록이 있습니다.

AEM 6.2 SP1-CFP15에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/6_2cfp15updated_bundles.txt)

AEM 6.2SP1-CFP15에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/6_2_cfp15contentpackage-list.txt)

### 누적 수정 팩 14 {#cumulative-fix-pack-6}

AEM 누적 수정 팩 6.2 SP1-CFP14는 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 에셋의 메타데이터 속성 편집이 개선되었습니다.
* 이미 만료된 상태의 에셋에 대한 암호 만료 알림 작업을 다시 구성했습니다.
* 추가 로케일을 확장하도록 사용자 지정된 Touch UI 콘솔입니다.
* 효율적인 Livecopyindex 동기화를 위해 cq-msm-core가 업데이트되었습니다.
* 다양한 롤아웃에 대한 복제 기능이 간소화되었습니다.

### 자산 {#assets-5}

* 사용자가 면책조항이 있으며 긴 파일 이름을 사용하는 에셋을 다운로드할 수 없습니다. NPR-22163: CQ-4235274용 핫픽스
* 작은 따옴표를 사용하면 빠른 도구 모음 작업을 사용하여 에셋의 속성을 열 때 일괄 보기에서 메타데이터 업데이트가 수행되지 않으며 UI가 완전히 중단됩니다. NPR-22317, NPR-22353: CQ-4236990, CQ-4236469용 핫픽스
* 에셋 만료 알림 작업은 만료된 에셋을 비활성화하지 않습니다. NPR-22346: CQ-4237188용 핫픽스
* Safari의 에셋에서 디지털 권한 관리를 사용할 때 에셋 다운로드가 실패합니다. NPR-22378: CQ-4236460용 핫픽스
* 작은 이미지에 대한 웹 렌디션의 픽셀 크기가 부정확합니다. NPR-22435: CQ-4236742용 핫픽스

### 사이트 {#sites-5}

* (Touch UI) 이동한 태그가 페이지 속성의 이전 및 새 위치에 표시됩니다. NPR-21921, CQ-4238598용 핫픽스
* (Touch UI) 리치 텍스트 편집기가 &lt;a> 태그에서 ID 이외의 모든 특성을 제거합니다. NPR-22045: CQ-4234133용 핫픽스
* CTRL+V를 사용하여 리치 텍스트 편집기에서 바로 콘텐츠를 붙여넣으면 줄바꿈을 건너뜁니다. NPR-22117: CUI-5881용 핫픽스
* (Touch UI) 네임스페이스 아래에 40개 이상의 태그를 표시할 수 없습니다. NPR-22290: CQ-99114용 핫픽스
* RSS 피드 문제, AEM 6.2에 대한 포트 -1. NPR-22158: CQ-4233339용 핫픽스
* (IE) 리치 텍스트 필드에서 처음 문자를 작성할 때 문자 뒤에 공백이 추가됩니다. NPR-22443: CQ-4235343용 핫픽스
* 패키지 이름과 일치하려고 하면 패키지 선언의 후행 공백 문자로 인해 Java Use 오브젝트가 SightlyJavaCompilerService를 중지합니다. NPR-22557: Granite-20836용 핫픽스
* Touch UI 콘솔에서는 태깅에 사용할 새 언어를 선택하지 않습니다. NPR-22250: CQ-4239194용 핫픽스

### Mobile On-Demand {#mobile-on-demand}

* (Digital Publishing Suite) 발행 날짜와 표지 날짜 필드는 모두 Folio를 DPS로 업로드하기 전에 설정해야 하는 필수 필드입니다. NPR-22484

### 상거래 {#commerce}

* 상거래 카탈로그 만들기 마법사의 여러 XSS(크로스 사이트 스크립팅) 취약성입니다. NPR-22344: CQ-4237017용 핫픽스

### MSM {#msm-2}

* LiveCopyIndex 동기화를 수행하면 긴 색인을 업데이트하는 동안 스레드가 정체됩니다. NPR-22214: CQ-90667용 핫픽스
* livecopy의 다른 필드를 편집할 때 cq:cugEnabled 속성이 비활성화되므로 페이지가 보호되지 않습니다. NPR-22246: CQ-4236050용 핫픽스
* 페이지가 일시 중단되면 페이지 롤아웃 작업에서 하위 페이지가 업데이트되지 않습니다. NPR-22483: CQ-4236956용 핫픽스
* 마스터에서 이동된 구조를 롤아웃하면 잘못된 cq:moveTarget으로 이동됩니다. NPR-22373: CQ-4232536용 핫픽스

### 통합 {#integration-6}

* 오퍼 선택기 라이브러리에서 오퍼를 정렬하려고 하면 잘못된 동작이 발생합니다. NPR-22208: CQ-4235439용 핫픽스
* 쿼리를 장기 실행하는 동안 TargetContentImpl이 AEM을 느리게 만듭니다. NPR-22361: CQ-4236907용 핫픽스
* Target 엔진(mbox.js, at.js)이 mangled URL을 사용하지 않고, 콜론이 포함된 URL을 사용하므로 특정 배포에서 실패할 수 있습니다. NPR-22366: CQ-4237854용 핫픽스
* 페이지 개인화를 사용하려면 브랜드 노드에서 바로 게시가 필요합니다. NPR-22370: CQ-4236895용 핫픽스

### Foundation {#foundation}

* Apache Sling Scripting Sightly 모델은 제공업체 번들 **org.apache.sling.scripting.sightly.models.provider/1.0.18**&#x200B;을 사용합니다. NPR-22614: Sling-5944, Sling-6866에 대한 핫픽스

### 프로젝트 {#projects}

* Workflow Starter에서 String의 TypeHint 값을 사용할 수 없습니다. NPR-22436: CQ-4237855용 핫픽스

### 번역 {#translation-2}

* 미리보기 기능을 사용하여 문제를 조사합니다. NPR-22201: CQ-4223753용 핫픽스

### 사용자 인터페이스 {#user-interface-2}

* (클래식 UI) 연관된 양식 데이터 모델 서비스가 빈 필드로 설정된 경우에도 구성 요소에 기본값이 표시됩니다. NPR-21903: GRANITE-19744용 핫픽스

### WCM - Foundation 구성 요소  {#wcm-foundation-components-3}

* Adobe Campaign의 Importer 페이지를 가리키는 라이브 카피 페이지를 게시할 때 오류가 발생했습니다. NPR-22470: CQ-4237164용 핫픽스
* 경험 구성요소 편집기를 여는 동안 JavaScript 오류가 발생했습니다. NPR-22598: CQ-4238415용 핫픽스

### 워크플로우 {#workflow}

* 일별 CQ 워크플로 이메일 알림 서비스는 WorkflowCompleted 및 WorkflowAborted 알림에 대해 Mongo 노드당 하나의 이메일을 트리거합니다. NPR-22486: CQ-4238172용 핫픽스

## 양식 {#forms-6}

### Forms 추가 기능 패키지 {#forms-add-on-package-6}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

#### 적응형 양식 {#adaptive-forms-4}

* IE11 및 Chrome에서 적응형 양식의 드롭다운 자리 표시자 값이 일치하지 않습니다. NPR-22405: CQ-4227096용 핫픽스

### Forms JEE 설치 프로그램 {#forms-jee-installer-6}

#### LCM 설치 {#install-lcm}

* 설치 관리자 및 LCM에서 Jsafe Jars를 Cryptoj 6.1.3.1로 업데이트합니다. NPR-22744

### 기능 팩이 포함됨 {#feature-packs-included}

#### 프로세스 관리 {#process-management}

* (HTML 작업 공간) 사용자가 작업을 요청하면 해당 사용자에 대한 큐 개수를 새로 고치지만 다른 사용자의 경우 페이지를 새로 고쳐야만 큐 개수를 새로 고칩니다. NPR-19778: CQ-4233665용 핫픽스

### CFP14에 포함된 OSGI 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-cfp}

AEM 6.2 SP1-CFP14에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/6_2cfp14updated_bundles.txt)

AEM 6.2 SP1-CFP14에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/6_2_cfp14contentpackage-list.txt)
AEM 누적 수정 팩 6.2 SP1-CFP13은 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* AT.js를 클라이언트 라이브러리로 사용하는 동안 타겟 구성 요소 설정 내에서 정적 매개 변수 필드 구성을 활성화했습니다.
* 드롭다운 구성 요소의 표시/숨기기 기능이 수정되었습니다.
* 대상 동기화 대상 사용에 대한 수정 사항.
* 특수 문자를 포함하기 위해 서신 관리를 위한 다기능성을 개선했습니다.

### 자산 {#assets-6}

* 버전 삭제에서 이전 버전의 에셋을 제거하지 못했습니다. NPR-21682: CQ-4212996용 핫픽스
* 재정렬 가능한 폴더에 있는 폴더를 다시 정렬하면 정렬이 유지되지 않습니다. NPR-21964: CQ-4231761용 핫픽스

### 사이트 {#sites-6}

* (TouchUI)(ClassicUI) HTL 및 코어 구성 요소의 다중 XSS(크로스 사이트 스크립팅) 취약점. NPR-21532: CQ-4232305 및 CQ-4232511용 핫픽스
* 선택한 텍스트에 대한 콘텐츠 만들기/서식(예: 새 목록 스타일 지정/제거)이 Internet Explorer 11에서 제대로 작동하지 않습니다. NPR-21533: CQ-4230689용 핫픽스
* (Safari) 사용자가 에셋 파인더 패널에서 모든 에셋을 볼 수 없습니다. NPR-21981: CQ-4213720용 핫픽스
* 날짜를 변경할 때 시간 비틀기를 수행하면 페이지가 깨진 상태로 &quot;RecursionTooDeepException&quot; 오류를 반환하고 새 버전이 만들어지지 않습니다. NPR-21707: CQ-4199536용 핫픽스
* 편집기에서 페이지를 로드할 때 WorkflowStatusprovider(pageinfo.json)가 3번 로드되면서 AEM 인스턴스가 느리게 실행됩니다. NPR-21778: CQ-59232용 핫픽스

### 통합 {#integration-7}

* 모바일 유형 및 브라우저의 대상 만들기가 AEM에서 Target 작성 모드로 작동하지 않습니다. NPR-21676, NPR-21681: CQ-4232100용 핫픽스
* 타깃팅된 구성 요소를 새로 고치는 동안 지연 시간이 길어지는 중 구성 요소를 완전히 새로 고치기 전에 다른 오퍼를 추가할 수 있습니다. NPR-21744: CQ-4233158/CQ-4234293용 핫픽스
* 클라우드 구성에서 클라이언트 라이브러리로 AT.js를 사용하여 테스트할 때 볼 수 있는 mbox 호출에서 정적 매개 변수의 테스트 값을 볼 수 없습니다. NPR-21930: CQ-4234520용 핫픽스

### 플랫폼 {#platform-4}

* 사용자 또는 그룹 수가 많을 때 사용자를 동기화하면 성능 문제가 발생합니다. NPR-20431: CQ-4223282용 핫픽스
* Sling 배포를 사용하여 사용자 동기화를 통해 사용자가 동기화되지 않습니다. NPR-21911: Granite-20404용 핫픽스
* Geometrixx 페이지의 검색 발췌 시 중지 단어가 강조 표시되지 않습니다. NPR-21835: Granite-21067용 핫픽스\
   참고: 이 수정 사항을 적용하려면 Oak CFP 1.4.20 이상이 필요합니다.

### 번역 {#translation-3}

* 번역 프로젝트를 만드는 동안 개시자의 사용자 ID에 대한 jcr 속성이 누락되었습니다. NPR-21715: CQ-4230713용 핫픽스

### WCM - Foundation 구성 요소 {#wcm-foundation-components-4}

* 양식 드롭다운 구성 요소의 기능 표시/숨기기 기능이 예상대로 작동하지 않습니다. NPR-22164: CQ-4235288용 핫픽스

## 양식 {#forms-7}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-7}

#### 적응형 양식 {#adaptive-forms-5}

* 적응형 양식에 XML 외부 엔티티 주입(XXE)이 포함되어 있습니다. NPR-21982: CQ-109878용 핫픽스
* (iOS11) 첨부 파일 구성 요소를 클릭하면 디바이스 파일 브라우저 대신 파일의 첨부 파일에서 카메라가 열립니다. NPR-21926: CQ-4214348용 핫픽스
* 테마 만들기 UI에서 제목이 누락되어 대화 상자가 렌더링되지 않고 예외가 발생했습니다. CQ-4236143용 핫픽스

#### 서신 관리 {#correspondence-management-1}

* 특수 문자가 포함된 xml 데이터의 렌더링 문제가 있습니다. NPR-21712: CQ-4229137용 핫픽스

### Forms JEE 설치 프로그램 {#forms-jee-installer-7}

#### 어셈블러 서비스 {#assembler-service}

* 6.2.0-ASM-1017-003을 사용하여 생성된 PDF 파일이 손상되었습니다. NPR-21427: CQ-4228046용 핫픽스

#### PDFG 서비스 {#pdfg-service-1}

* PNG, JPEG 및 TIFF 파일의 예기치 않은 페이지 크기(PDF)로 인해 OCR이 실패했습니다. NPR-19489: CQ-4209079용 핫픽스

## CFP13에 포함된 OSGI 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-cfp-1}

AEM 6.2 SP1-CFP13에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/cfp13_bundlecompare-list.txt)

AEM 6.2 SP1-CFP13에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/cfp13_contentpackage-list.txt)

AEM 누적 수정 팩 6.2 SP1-CFP12.1은 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 복수 값 필드에 대한 메타데이터 처리가 개선되었습니다.
* 번역 워크플로에서 복수 문자(2개 이상) 국가 코드를 지원합니다.
* 중첩 구성 요소가 여러 개 있는 페이지의 렌더링을 개선했습니다.
* AEM과 Adobe Digital Publishing Suite 간 에셋에 대한 게시 날짜 동기화를 개선했습니다.

### 자산 {#assets-7}

* OmniSearch에 문자가 너무 많아 AEM 서버가 충돌합니다. NPR-21083: CQ-4223602용 핫픽스
* 메타데이터 스키마의 복수 값 필드에서 두 번째 옵션에 지정된 값은 CRX-de에 이전에 지정한 값에 추가되지 않습니다. NPR-21220: CQ-4224526용 핫픽스
* Safari의 에셋에서 디지털 권한 관리를 사용할 때 에셋 다운로드가 실패합니다. NPR-21387: CQ-4230287용 핫픽스

### 사이트 {#sites-7}

* (DAM) (클래식 UI) AEM CQ 작성자/게시 빠른 시작에서 일부 SWF 파일의 다중 크로스 사이트 스크립팅(XSS) 취약점. NPR-21073, NPR-21074: NPR-20612용 핫픽스
* 태그 선택기에서 여러 언어로 사용할 수 있는 태그를 번역하지 않습니다. NPR-21221: CQ-78855용 핫픽스
* AEM 기사 콘솔에서 문제를 렌더링하면 중첩된 구성 요소를 여러 개 사용하는 것처럼 속도가 느려집니다. NPR-21271: CQ-4224158용 핫픽스

### 통합 {#integration-8}

* Target 프레임워크를 추가할 때 편집기의 선택 모드 목록에서 타깃팅 모드를 사용할 수 없습니다. NPR-21047

### Mobile-on-demand {#mobile-on-demand-1}

* (Digital Publishing Suite) AEM의 Folio에 대한 발행 날짜가 Folio Producer에 표시되는 날짜와 일치하지 않습니다. NPR-21145

### MSM {#msm-3}

* LC에서 첫 번째 로컬 페이지를 삭제하면 라이브 카피 재설정 프로세스가 중지됩니다. NPR-21276: CQ-4229743용 핫픽스

### 플랫폼 {#platform-5}

* AEM 6.3으로 업그레이드한 후 스크립트로 구현된 태그를 참조하는 사용자 지정 taglib을 찾을 수 없습니다. NPR-20149: Granite-18433용 핫픽스

### 번역 {#translation-4}

* 번역 워크플로는 lang_country 코드가 2자를 초과하는 경우 실패합니다. NPR-21088: CQ-4197439용 핫픽스
* 프로젝트가 완료될 때까지 에셋 페이지를 번역 프로젝트에 다시 제출할 수 없습니다. NPR-21219: CQ-4209908용 핫픽스

### 사용자 인터페이스 {#user-interface-3}

* 선택 구성 요소는 양식을 제출하는 동안 대상 속성을 삭제하지 않습니다. NPR-21163: GRANITE-14125용 핫픽스
* HTTP.encodePathOfURI가 확장되면 더하기 기호 &#39;+&#39;를 두 번 인코딩합니다. NPR-21417: GRANITE-16340용 핫픽스

### 취약성 {#vulnerability-4}

* DAM 메타데이터 편집기의 XSS(크로스 사이트 스크립팅). NPR-21434: CQ-83472용 핫픽스
* XSS(크로스 사이트 스크립팅)에 취약할 수 있는 여러 SWF 파일. NPR-20612: CQ-4213297용 핫픽스

## 양식 {#forms-8}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-8}

#### 서신 관리 {#correspondence-management-2}

* (IE11) HTML 콘텐츠의 초기 렌더링은 왼쪽에서만 수행되는 반면 오른쪽은 전체 UI가 로드된 후 간헐적으로 로드됩니다. NPR-21554
* AEM 6.2 SP1-CFP9를 설치하면 편지 미리보기 제출 버튼이 비활성화됩니다. NPR-21547
* 에셋 링크 유형을 선택할 때 에셋 선택기 창이 편지 데이터 바인딩 편집 마법사에서 열리지 않습니다. NPR-21164: CQ-4194567용 핫픽스
* 인라인 또는 편집 가능한 텍스트 모듈을 편집하려면 관련 편집 아이콘을 누르거나 편지 미리보기에서 관련 텍스트 모듈을 더블 클릭합니다. NPR-21402

#### 적응형 양식 {#adaptive-forms-6}

* AEM Forms 제출 버튼 구성 요소에 type=&quot;submit&quot; 대신 type=&quot;button&quot;이 표시됩니다. NPR-21007
* 데이터는 반복 가능한 패널의 새 패널을 추가하거나 삭제할 때 계속 유지됩니다. NPR-21408

### Forms JEE 설치 프로그램 {#forms-jee-installer-8}

#### 코어 {#core-2}

* 최신 Java 8 업데이트 131로 업그레이드하면 예외가 발생합니다. &quot;JsafeJCE 공급자가 비활성화되었습니다. FIPS 140 필수 자체 무결성 검사에 실패했습니다.&quot; NPR-21355

   **참고:** 이 NPR에는 추가 설정이 필요합니다. 자세한 내용은 [최신 Java 8 업데이트](release-notes-aem-6-2-cumulative-fix-pack.md#latest-java-update-throws-an-exception-npr)를 참조하십시오.

* 코어, 암호화, 서명 및 문서 보안의 cryptoj 6.1.3.1로 jsafe jar을 업데이트합니다. NPR-21360, NPR-21361, NPR-21356, NPR-21358

#### LCM 설치 {#install-lcm-1}

* 설치 관리자 및 LCM에서 Jsafe Jar을 Cryptoj 6.1.3.1로 업데이트합니다. NPR-21362

#### PDFG 서비스 {#pdfg-service-2}

* PDFG에서 Jsafe Jar을 Crypj 6.1.3.1로 업데이트합니다. NPR-21359

#### 프로세스 관리 {#process-management-1}

* (HTML 작업 공간) 이름 카테고리가 잘리지 않도록 열 크기 조정을 활성화합니다. NPR-19770: CQ-4233668용 핫픽스

#### Reader 확장 서비스 {#reader-extensions-service-1}

* RE에서 jsafe jar을 cryptoj 6.1.3.1로 업데이트합니다. NPR-21357

## CFP12.1에 포함된 OSGI 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-cfp-2}

AEM 6.2 SP1-CFP12.1에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/cfp12_bundlecomparsion-list1.txt)

AEM 6.2 SP1-CFP12.1에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/cfp12_contentpackage-list.txt)

AEM 누적 수정 팩 6.2 SP1-CFP11은 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 효율적인 Livecopyindex 동기화를 위해 cq-msm-core를 업데이트했습니다.
* 콘텐츠 조각에 대한 편집 효율성이 개선되었습니다.
* ACL 권한을 감지하기 위한 유효성 검사 옵션을 패키지 관리자에서 제공합니다.
* 고객 서신에 이메일 ID를 포함하는 Campaign 기능을 도입했습니다.
* Dynamic Media 파일에 대한 비디오 인코딩 기능이 개선되었습니다.
* Sightly 구성 요소 및 라이브 카피의 수정 사항.

### 자산 {#assets-8}

* 이름에 공백이 포함된 파일은 Dynamic Media 비디오 인코딩에 실패합니다. NPR-20818: CQ-102469용 핫픽스
* AEM CQ 작성자/게시 빠른 시작에서 일부 SWF 파일의 다중 크로스 사이트 스크립팅(XSS) 취약점. NPR-21071, NPR-21072
* 사용자가 면책조항이 있으며 긴 파일 이름을 사용하는 에셋을 다운로드할 수 없습니다. NPR-20255: CQ-4222139용 핫픽스

### 사이트 {#sites-8}

* AEM 및 Campaign 통합: Adobe Campaign에서 특수 링크를 다시 작성하면 고객이 이메일에서 mailto: 하이퍼링크를 보낼 수 없습니다. NPR-20787: CQ-4225760용 핫픽스
* (Touch UI) 언어가 프랑스어로 설정된 경우, AEM 사용성 문제 및 성능 문제가 발생합니다. NPR-20854: CQ-4227628용 핫픽스
* RTE에서 링크 플러그인을 사용하여 인코딩된 에셋 파일을 연결하면 빈 링크가 반환됩니다. NPR-20626, NPR-21059: CQ-4223011용 핫픽스
* 콘텐츠 조각 메타데이터 편집기를 사용하면 콘텐츠 작성자가 콘텐츠 조각에 변경 사항을 저장할 수 없습니다. NPR-20641: CQ-4224755용 핫픽스
* 페이지 속성 별칭은 발행 요청/발행 취소 요청으로 이어집니다. NPR-20731: CQ-4226227용 핫픽스
* RTE 요소의 링크 인코딩에 관련된 텍스트 구성 요소 문제입니다. NPR-20755: CQ-4224321용 핫픽스

### 플랫폼 {#platform-6}

* ResourceResolverImpl.map()은 ResourceDecorator를 호출하지 않습니다. NPR-20788: GRANITE-19718용 핫픽스
* org.apache.sling.i18n.DefaultLocaleResolver에서 org.apache.sling.engine.SlingRequestProcessor를 통해 요청을 처리할 수 없습니다. NPR-20706: CQ-94880용 핫픽스
* 특정 패키지에서 ACL 권한/권한이 변경되었는지 확인하기 위해 패키지 관리자에 유효성 검사 옵션을 추가하도록 요청합니다. CQ-4229196용 핫픽스

### 통합 {#integration-9}

* (Search &amp; Promote) 콘텐츠 패키지에 대한 필터 정의가 모호하면 설치 시 경로를 덮어씁니다. NPR-20808: CQ-4227615용 핫픽스

### 워크플로우 {#workflow-1}

* AEM 프로덕션 서버 배포에 안정성 문제가 있습니다. NPR-20979: Granite-19104용 핫픽스

### 프로젝트 {#projects-1}

* (Touch UI) 팀 구성원을 프로젝트에 추가할 수 없습니다. NPR-20990: CQ-4205375용 핫픽스

### WCM-Foundation 구성 요소 {#wcm-foundation-components-5}

* Sightly 이미지 구성 요소 &#39;link to&#39;는 .html 확장명이 누락되어 403 오류를 생성합니다. NPR-20823: CQ-4195909용 핫픽스
* LiveCopy를 사용하는 블루프린트 사이트에서 양식 구성 요소를 삭제하려고 하면 NullPointerException이 발생하고 양식 구성 요소를 삭제하는 대신 다시 추가합니다. NPR-20855: CQ-4204628용 핫픽스
* LiveCopyIndex 동기화를 수행하면 긴 색인을 업데이트하는 동안 스레드가 정체됩니다. NPR-20634: CQ-90667용 핫픽스

### 보안 {#security}

* 사전 예방적 XSS 라이브러리 업데이트. NPR-21174
* 이메일 전송을 위한 간소화된 API를 제공하는 Apache Commons Email 1.5로 업그레이드하십시오. NPR-20509: Granite-18240용 핫픽스
* Apache Sling XSS 보호 API에 보안 패치를 적용하여 XSS 우회 가능성을 제거했습니다. NPR-21290: GRANITE-19924용 핫픽스
* XSSAPI#getValidHref 함수의 XSS 우회. NPR-21174: Granite-19924용 핫픽스

### 모바일 앱 {#mobile-apps}

* AEM의 OOTB 에셋에 대한 curl Head 요청 문제가 수정되었습니다. NPR-20511: CQ-4221520 및 CQ-103024용 핫픽스

## 양식 {#forms-9}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

AEM Forms의 주요 사항은 다음과 같습니다.

* Workbench 사용자에 대해 인증서 인증을 사용하도록 설정했습니다.
* 서신 관리, HTML5 양식 및 AEM Forms 작업 공간에 대한 유용성 수정 사항.

### Forms 추가 기능 패키지 {#forms-add-on-package-9}

#### HTML5 양식 {#html-forms-1}

* iOS 10 및 11 디바이스에서의 스크리블 구성 요소 사용 문제. NPR-21092

#### 서신 관리 {#correspondence-management-3}

* (서신 UI) 한 번의 클릭으로 제출 버튼을 비활성화할 수 있습니다. NPR-21078

### Forms JEE 설치 프로그램 {#forms-jee-installer-9}

#### 어셈블러 서비스 {#assembler-service-1}

* docConverter에서 &quot;요소 &quot;stEvent:action&quot;의 접두사 &quot;stEvt&quot;가 바인딩되지 않음&quot;이라는 오류가 발생하여 PDF/A를 생성하지 못했습니다. NPR-21032: CQ-4222540용 핫픽스
* 서비스 OMPFSubmission/PDFA/PDFtoPDFA를 호출하는 동안 java.lang.IllegalArgumentException message:No enum constant com.adobe.internal.pdfm.docbuilder.signature.PathValidationFailureReason.SIGNED_IN_FUTURE라는 이름의 예외가 발생했습니다. 이 경우 서버를 다시 시작할 때까지 단기 서명 확인 프로세스를 완료할 수 없습니다. NPR-20792

#### Workbench {#workbench}

* Workbench 사용자에 대해 인증서 인증을 사용하도록 설정합니다. NPR-17548: CQ-4214486용 핫픽스

#### 프로세스 관리 {#process-management-2}

* 데이터 준비 프로세스는 모바일 양식을 dataref 매개 변수로 렌더링할 때 여러 번 호출합니다. NPR-19801: CQ-4230427용 핫픽스: CQ-4230400

## CFP11에 포함된 OSGI 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-cfp-3}

AEM 6.2 SP1-CFP11에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/cfp11_bundlecomparsion-list.txt)

AEM 6.2 SP1-CFP11에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/cfp11_contentpackage-list.txt)

AEM 누적 수정 팩 6.2 SP1-CFP10은 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 테스트를 위해 onDialogLoaded에 새 유틸리티 함수를 추가했습니다.
* ClientLibraryProxyServlet에 프런트 엔드 단위 테스트 및 구성을 추가했습니다.
* 복수 이미지 즉석 편집기 구성 요소의 성능 수정 사항.
* Apache Sling JCR ResourceBundleProvider의 구성 업데이트.

### 자산 {#assets-9}

* 에셋 업데이트 워크플로가 비활성화된 경우 에셋 미리보기가 작동하지 않습니다. NPR-20543: CQ-4204986용 핫픽스
* granite에 클래스의 렌더링 문제가 추가됨: 클래스 속성(cq-damadmin-admin-assets-upload). NPR-20514: CQ-4219238용 핫픽스
* 제목에 특수 문자가 있는 썸네일 에셋은 NPR-20347의 alt 속성에 java 오브젝트를 표시합니다.CQ-4223620 핫픽스
* 라이선스 문제로 인해 버전 비교 코드를 Adobe 자체 코드로 대체합니다. NPR-20273: CQ-4223758용 핫픽스
* 여러 알파 레이어가 있는 CMYK PSB 파일을 업로드할 때 처리 문제가 발생합니다. NPR-20251: CQ-4220869용 핫픽스
* 국제화 사전은 서버가 org.apache.sling.i18n 2.5.6에서 다시 시작하지 않으면 작동하지 않습니다. NPR-20525: Granite - 19490 핫픽스
* 기본 스레드 덤프 수집 프로그램 구성(기본 AEM 시작)을 사용하는 스케줄러 기간에 따라 스레드 덤프가 생성되지 않습니다. NPR-20288: GRANITE-19488 / GRANITE-12741 / CQ-90647용 핫픽스.

### 사이트 {#sites-9}

* 저장된 검색을 연 후 수정된 날짜 필터가 변경되는 경우, 결과에 영향을 주지 않으며 표시되는 결과는 수정된 날짜 필터의 이전 저장된 값과 동일합니다. NPR-19739: CQ-4219425용 핫픽스
* 중첩된 구성 요소가 있는 페이지를 로드하지 못했습니다. NPR-20312
* 삭제 워크플로에 대한 요청은 워크플로 패키지를 삭제할 때 트리거됩니다. NPR-20266: CQ-4221686용 핫픽스
* (Touch UI) OS 클립보드 및 내부 AEM 클립보드를 사용하여 복사/붙여넣기를 할 때 발생하는 문제. NPR-20228: CQ-4220383용 핫픽스
* 에셋을 여러 개(100개 이상) 로드하면 AEM 인스턴스에서 목록 보기가 느려집니다. NPR-20034: CQ-4222695용 핫픽스
* (Touch UI) 클래식 UI 콘솔을 통해 시작 페이지를 삭제하면 모든 페이지가 편집할 수 없게 됩니다. NPR-20520: CQ-4225074용 핫픽스
* Target 드롭다운이 대화 상자의 여러 RTE 구성 요소에서 작동하지 않습니다. NPR-20345: CQ-4220981용 핫픽스

### 플랫폼 {#platform-7}

* 익명 세션을 사용하여 액세스할 때 ClientLibraryProxyServlet에서 게시 인스턴스의 클라이언트 라이브러리에 대한 요청을 프록시하지 않으며 HTTP 404 찾을 수 없음 오류를 표시합니다. NPR-20195: Granite-14409용 핫픽스

### 통합 {#integration-10}

* 대상 엔진을 Adobe Target으로 선택하면 구성 요소가 로드되지 않고 서버 로그에 오류가 발생합니다. NPR-20058: CQ-88071, CQ-109698, CQ-4201600용 핫픽스

### 상거래 {#commerce-1}

* 동일한 페이지의 제품을 만들 때 확인 또는 리디렉션 팝업 메시지가 표시되지 않습니다. NPR-20257: CQ-4223414용 핫픽스

### 사용자 인터페이스 {#user-interface-4}

* Datepicker가 여러 필드 중 한 개인 필드인 경우 날짜 필드에 저장된 값은 구성 요소를 편집하는 동안 지속되지 않습니다. NPR-20077: GRANITE-19147용 핫픽스
* 잘못된 결과를 생성하는 연속 쿼리가 트리거되는 경우 이전 쿼리가 중단되지 않습니다. NPR-20397: GRANITE-19306용 핫픽스

### WCM - Foundation 구성 요소 {#wcm-foundation-components-6}

* ImageMap 속성은 여러 이미지 즉석 편집기 구성 요소에서 이미지를 제거한 후에도 계속 존재합니다. NPR-20142: CQ-4222982용 핫픽스

## 양식 {#forms-10}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-10}

#### 적응형 양식 {#adaptive-forms-7}

* valueCommit 스크립트를 UI를 통해 변경하면 DropDownList에 대해 두 번 실행됩니다. NPR-19989: CQ-110212용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-10}

**프로세스 관리**

* CFP 패키지에는 AEM Forms HTML 작업 공간 버전 2.2.26. NPR-20099가 있습니다.
* 모바일 양식을 PDF로 보도록 구성한 경우 미리 채워진 양식이 작동하지 않습니다. NPR-20566

**권한 관리**

* CAC/상호 인증 인증서 선택 대화 상자에는 EKU(고급 키 사용)가 있는 인증서가 클라이언트 인증 또는 스마트 카드 로그온으로 표시되어야 합니다. NPR-20708
* Forms JEE가 PKCS#11 상호 인증을 지원합니다. NPR-15001

## CFP10에 포함된 OSGI 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-cfp-4}

AEM CFP 6.2 SP1-CFP10에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/bundle-list-cfp10.txt)

AEM CFP 6.2 SP1-CFP10에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/contentpackage-list-cfp10.txt)

AEM 누적 수정 팩 6.2 SP1-CFP9는 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 암호 입력을 위해 Analytics 클래식 UI 구성이 적용되었습니다.
* Contexthub의 독립 지속성 캐시에 대한 수정 사항.
* 에셋 차원의 정확한 계산.
* Brand Portal에 에셋을 게시할 때 AEM 성능이 최적화되었습니다.
* 캔버스 노드의 Resourcetype 값에 대한 수정 사항.
* 문서 조각 콘텐츠에 대해 대/소문자 구분 및 특수 문자 검색 기능을 사용할 수 있습니다.
* Safari에서 PDF를 첨부 파일로 첨부할 수 있도록 적응형 양식이 개선되었습니다.\
   새로운 Dynamic Media 게시 인프라에 연결하여 보다 빠르고 확장 가능한 복제를 지원하는 새 Dynamic Media를 제공합니다.

### 자산 {#assets-10}

* InDesign 에셋에 해당 에셋에 대한 중복된 링크가 포함되어 있어서 AEM Assets에서 하위 에셋 참조를 추출할 수 없습니다. NPR-19006: CQ-4204186용 핫픽스
* 전자 상거래 컬렉션 내부의 에셋에 대해 정렬 옵션이 작동하지 않습니다. NPR-19508: CQ-4213622용 핫픽스
* 기존 에셋과 이름이 같은 에셋을 같은 위치로 이동하면 에셋의 cq: lastReplicationAction 값이 서로 교체되어 잘못된 메타데이터가 생성됩니다. NPR-19531
* 모든 에셋이 올바르게 게시되지만 에셋을 게시할 때 오류 메시지가 표시되는 경우가 많습니다. NPR-19629: CQ-4219611용 핫픽스
* 정적 렌디션은 고정된 차원으로 나열되며 실제 렌디션의 크기를 반영하지 않습니다. NPR-20004
* 여러 에셋(4개 이상)이 Brand Portal에 게시되는 경우 AEM 인스턴스 속도가 느려집니다. NPR-20009

### 사이트 {#sites-10}

* 사용자가 다른 사용자가 잠근 페이지의 게시/게시 취소/만들기 버전을 게시하려고 하면 AEM에 예기치 않은 동작이 표시됩니다. NPR-19249, CQ-4215298 및 CQ-4203856용 핫픽스
* 중첩된 시작을 수동으로 승격하는 동안 하위 페이지가 삭제됩니다. NPR-19704
* ContextHub 저장이 초기화 중에 덮어쓰기 기본 지속성 레이어를 겹쳐 쓰는 경우 지속성 문제가 발생합니다. NPR-19979: CQ-4218399용 핫픽스
* 콘텐츠 조각이 다른 버튼과 겹칩니다. NPR-19980: CQ-4221519용 핫픽스
* SiteAdmin에서 별칭을 사용하여 확인할 때 사이트 페이지가 표시되지 않습니다. NPR-20053: CQ-4221478용 핫픽스
* Adobe Campaign의 Importer 페이지를 가리키는 라이브 카피 페이지를 게시할 때 오류가 발생했습니다. NPR-20066: CQ-4220846용 핫픽스

### 플랫폼 {#platform-8}

* PPT 슬라이드의 배경 이미지를 변환에 포함할 수 있도록 Apache POI를 버전 3.16으로 업그레이드했습니다. NPR-18286
* 동일한 폴더에 여러 에셋을 업로드하는 동안 Internet Browser 11 및 Edge에서 렌더링 문제가 발생합니다. NPR-20062

### 통합 {#integration-11}

* 익명 사용자로 액세스할 때 사용자 지정 at.js 파일이 게시되지 않습니다. NPR-19542: CQ-4219592용 핫픽스
* Analytics 기존 인증서를 WSSE 인증으로 마이그레이션하는 중입니다. NPR-19962

### Brand Portal {#brand-portal}

* AEM에서 tagadmin/tagging 콘솔의 Brand Portal에 태그를 게시하도록 설정합니다. NPR-20271

## 양식 {#forms-11}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-11}

#### 서신 관리 {#correspondence-management-4}

* 편지를 미리 볼 때 문서 조각에서 실제 텍스트를 검색할 수 있는 기능을 활성화했습니다. NPR-19712

#### 적응형 양식 {#adaptive-forms-8}

* Safari에서 PDF를 첨부 파일로 첨부할 수 있도록 적응형 양식이 개선되었습니다. 기존 양식에서 동일한 기능을 지원하려면 첨부 파일 위젯의 구성을 변경하고 &quot;지원되는 파일 유형&quot;에서 .pdf 대신 값 application/pdf를 업데이트해야 합니다. NPR-19623

#### Forms Manager {#forms-manager-1}

* 적응형 양식 필드에 validationState가 정의되지 않은 경우 elementFocusChanged 이벤트가 발생하면 오류 이벤트(errorState)가 Adobe Analytics 서버로 반환됩니다. NPR-19513

### Forms JEE 설치 관리자 {#forms-jee-installer-11}

#### 코어 {#core-3}

* 종료하는 동안 연결 관리자를 사용할 수 없습니다. Jboss에서는 작성자 EAR을 배포하지 않은 이유로 손상 문제가 발생하기 전에 JDBC 종속성을 제거합니다. NPR-19703

## 기능 팩 포함됨 {#feature-packs-included-1}

* Dynamic Media의 썸네일 수정 및 투명도 개선. NPR-15207

## CFP9에 포함된 OSGI 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-cfp-5}

AEM 6.2 SP1-CFP9에서 업데이트된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/content_package-list62sp1-cfp9.txt)

AEM 6.2 SP1-CFP9에서 업데이트된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/content_package-list62sp1-cfp9-1.txt)

AEM 누적 수정 팩 6.2 SP1-CFP8은 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* Adobe 이메일 템플릿 서비스에서 사용자 정의 사용자 템플릿에 태그 도입.
* 데스크탑 앱에 대한 TouchUI 버튼 개선 사항.
* 번역 페이지에서 양식을 여러 개 전송하지 않도록 클릭 시 제출 버튼을 비활성화했습니다.
* 대화 상자에 여러 RTE 구성 요소를 구성했습니다.
* 라이브 카피에서 ReferenceUpdates를 보완했습니다.
* 문서 조각 콘텐츠에 대한 대/소문자를 구분하는 검색 기능을 사용할 수 있습니다.
* AEM Forms 설치 설명서에 Linux 라이브러리 목록을 추가했습니다.

### 자산 {#assets-11}

* Safari 브라우저에서 스마트 컬렉션에 Omnisearch 필터를 적용하는 문제. NPR-19511
* PDF 에셋과 연관된 키워드가 여러 개 있는 경우 PDF 키워드 메타데이터가 제대로 추출되지 않고 잘못 수정됩니다. 이 문제를 해결하기 위해 PDF 에셋에 대한 제목 필드 메타데이터 속성이 제거되었습니다. 그러나 메타데이터 스키마를 편집하여 제목 필드에 대한 여러 값 텍스트 필드를 추가할 수 있습니다. NPR-19126
* 워크플로 알림 서비스는 사용자가 클릭한 후 로드할 수 없는 이메일의 링크를 인코딩하지 않습니다. NPR-19490: CQ-4218055용 핫픽스
* Chrome을 사용하여 열 보기에 전체 페이지/에셋 목록을 로드할 수 없습니다. NPR-19458: CQ-4214248용 핫픽스
* 활성화 요청 워크플로를 활성화하면 AEM 받은 편지함에 잘못된 해제 시간 아이콘이 표시됩니다. NPR-19365: CQ-4216174
* 목록 보기의 정렬 문제. NPR-19217: CQ-95602
* 에셋 폴더 설정에서 제목 또는 썸네일 그림을 변경할 때 폴더의 원래 그룹 및 권한이 무시됩니다. NPR-19283: CQ-4216080용 핫픽스
* Windows 10 워크스테이션은 터치 모드로 자동 전환되면서 일부 버튼이 작동하지 않습니다. NPR-19183

### 사이트 {#sites-11}

* 대화 상자에 여러 RTE 구성 요소가 있는 문제. NPR-19311: NPR-19587
* vanilla AEM 6.2의 자동 버전 제거는 VersionManagerImpl이 초기화된 후에만 작동합니다. NPR-19315: CQ-4217175용 핫픽스
* 워크플로 인스턴스가 &quot;Salesforce.com 내보내기&quot; 워크플로 단계에서 멈춥니다. NPR-19222: CQ-4212976용 핫픽스
* 라이브 카피에서 만든 언어 사본 페이지를 편집할 수 없습니다. NPR-18967
* ReferencesUpdateAction에서 계층 변경이 있는 중첩된 LiveCopy로 링크를 업데이트하지 못했습니다. NPR-18715: CQ-4214105용 핫픽스

### 플랫폼 {#platform-9}

* Adobe 이메일 템플릿 서비스는 사용자 지정 사용자 템플릿에 태그를 추가합니다. NPR-19190: CQ-4217113용 핫픽스

### 프로젝트 {#projects-2}

* 프로젝트 편집기에서 프로젝트 에셋 폴더에 에셋을 복사할/붙여넣을 수 없습니다. NPR-19619
* 6.2 SP1-CFP1을 설치한 후 번역 프로젝트에 대한 미리보기를 생성할 수 없습니다. NPR-16481: CQ-4204655

### 통합 {#integration-12}

* 문서에 대한 액세스 속성이 클래식 UI의 Adobe Digital Publishing Solution에서 잘못 설정됩니다. NPR-19366
* AEM 기사 콘솔의 전체 화면 기사로 인해 썸네일의 렌더링이 느려집니다. NPR-19086: CQ-4217148
* 사용자가 여러 영역에 액세스할 수 있는 경우 Campaign을 통해 오퍼를 개인화할 때 잘못된 자동 접기 동작이 수행됩니다. NPR-19290: CQ-4218029용 핫픽스
* 대상 모듈을 편집하고 두 번 이상 저장하면 타깃팅 대화 상자가 타깃팅 모드에 표시되지 않습니다. NPR-19144: CQ-4216708용 핫픽스

### 워크플로우 {#workflow-2}

* 받은 편지함 클래식 UI에서 사용자/그룹별로 받은 편지함의 알림을 필터링할 수 없습니다. NPR-19122: CQ-4215374용 핫픽스
* 이미지 맵은 HTL 이미지 구성 요소에서 선택한 좌표를 유지하지 않습니다. NPR-18911: CQ-4211584

## 양식 {#forms-12}

* AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-12}

* Microsoft Word 또는 웹 브라우저에서 서신 관리자 텍스트 편집기로 콘텐츠를 복사하면 스타일이 손실됩니다. NPR-19530
* 줄 바꿈이 없는 콘텐츠는 텍스트 편집기에서 콘텐츠를 둘러싸지 않습니다. NPR-19481
* 편지를 미리 볼 때 문서 조각에서 실제 텍스트를 검색할 수 있는 기능을 활성화했습니다. NPR-17792: CQ-4214501용 핫픽스

#### 서신 관리 {#correspondence-management-5}

>[!NOTE]
>
>텍스트 조각에 대한 이 검색 기능에는 다음과 같은 몇 가지 제한 사항이 있습니다.
>
>* 문서 조각 콘텐츠는 대소문자를 구분하지만 제목은 대소문자를 구분하지 않습니다.
>* 검색된 단어 일부가 다른 스타일을 사용하거나 &quot; 또는 &#39; 또는 \ 등의 특수 문자를 포함하는 경우에는 검색 결과가 강조 표시되지 않습니다.
>* 문서 조각 내의 동적 콘텐츠(예: 데이터 사전 요소 값 또는 변수 값)에 대해서는 검색이 작동하지 않습니다.


#### Forms Manager {#forms-manager-2}

* 적응형 양식의 XML 스키마 속성은 AEM 6.2에서 CFP6을 적용한 후에는 편집할 수 없습니다. CQ-4219684 핫픽스
* AEM Forms Manager 코어 번들의 모든 서비스가 서버를 다시 시작할 때 시작되지 않습니다. CQ-4217014용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-12}

#### LCM 설치 {#install-lcm-2}

* Microsoft Windows의 관리자 화면에 CFP6 설치 후 버전 번호 6.0이 표시됩니다. CQ-4217573용 핫픽스

## 기능 팩 포함됨 {#feature-packs-included-2}

* 데스크탑 앱에 대한 TouchUI 버튼 개선 사항. NPR-18676

## CFP8에 포함된 OSGi 번들 {#osgi-bundles-included-in-cfp}

AEM 6.2 SP1-CFP8에서 업데이트된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/updated-bundles-list-cfp8.txt)

AEM 6.2 SP1-CFP8에서 업데이트된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/6_2sp1-cfp8-contentpackagelist.txt)

AEM 누적 수정 팩 6.2 SP1-CFP7은 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* dc: 제목 속성이 String [](multifield)으로 설정된 이미지에 대한 이미지 카드의 제목을 표시할 때 동작이 변경됩니다.
* Dynamic Media 클라우드 서비스, Touch UI 및 보안 UI 인터페이스의 성능 문제 수정.
* Apache Felix Http Bridge 3.0.8 수정 사항
* 작성자 및 게시 환경 간 바이너리 없는 복제(BLR) 문제를 해결했습니다.
* 대상 라이브러리 파일, AT.JS, 일반적인 웹 구현 및 단일 페이지 애플리케이션 모두를 위해 설계된 Adobe Target과의 클라이언트 측 통합을 위한 구현 라이브러리입니다.
* Marketing Cloud 솔루션(Analytics, DTM, Target 및 S&amp;P)에 대한 사용자 구성 가능한 연결 시간 초과 기간을 도입하여 AEM 성능이 개선되었습니다.

### 자산 {#assets-12}

* Dynamic Media Cloud Services로 구성된 AEM 6.3을 사용하여 비디오 처리를 테스트하는 동안 &quot;열려 있는 파일이 너무 많습니다.&quot; 예외가 발생합니다. NPR-18734, CQ-4211407용 핫픽스
* AEM 인스턴스를 다시 시작한 후 페이지의 에셋에 대한 별칭 URL 설정이 작동하지 않습니다. NPR-18634, Granite-18085용 핫픽스
* TouchUI에서 에셋을 게시할 권한이 없는 사용자를 위해 게시 버튼이 표시됩니다. NPR-18620, CQ-4214042용 핫픽스
* 사용권 계약이 설정되면 에셋에 대한 다운로드 대화 상자에는 동적 렌디션 옵션이 표시되지 않습니다. NPR-18607, CQ-4212342용 핫픽스
* 이름에 공백이 있는 에셋에 대한 동적 렌디션을 다운로드할 수 없습니다. NPR-18571, CQ-4211738용 핫픽스
* Creative Cloud와 에셋 폴더를 공유할 때 두 명 이상의 사용자를 저장할 수 없습니다. NPR-18489, CQ-103297용 핫픽스
* dc: 제목과 dc: 설명이 crx/de의 복수 필드 값으로 변경되지 않습니다. NPR-18474, CQ-4209086용 핫픽스
* 에셋 이동 작업으로 인해 성능이 저하됩니다. NPR-18346
* 기본 모두 표시 옵션이 설정된 상태로 타임라인에서 항목을 열면 해당 항목이 표시되지 않습니다. NPR-18302, CQ-4211957용 핫픽스
* ASCII/UTF-8로 인코딩된 텍스트 파일이 AEM Assets에 업로드되고 썸네일 생성이 실패하는 경우 오류가 발생합니다. NPR-18006: CQ-4209345용 CFP
* 사용자에게 복제 액세스 권한이 없더라도 게시 작업 버튼이 표시됩니다. NPR-17353, CQ-4209269용 핫픽스
* min:gcc;obfuskate=true를 사용하여 축소를 활성화하는 경우 Siteadmin 및 Miscadmin 모두 작동하지 않습니다. NPR-18593, CQ-4209220용 핫픽스
* 매번 화면을 새로 고치지 않으면 사용자 지정 메뉴 항목이 표시되지 않습니다. NPR-18500, CQ-4213581용 핫픽스
* moment.js를 2.10.6으로 업그레이드. NPR-18596, Granite-11881용 핫픽스
* DM 매크로에 대한 권한을 적용하면 관리자의 보기가 중단됩니다. NPR-18544, CQ-4211729용 핫픽스
* 에셋에 대한 나중에 게시를 수행하면 잘못된 ArgumentException이 발생합니다. CQ-4214532

### 사이트 {#sites-12}

* 시간이 콘텐츠에 설정된 정시에 도달하면 MongoDB가 있는 활성 상태의 작성자 클러스터에서 두 작성자가 동일한 콘텐츠에 대한 복제를 트리거하려고 합니다. NPR-18708, CQ-4210982용 핫픽스
* jcr이 없는 참조가 있는 리소스를 이동할 때 NPE: 콘텐츠 노드. NPR-18664
* 자리 표시자가 여러 개의 parsys 구성 요소가 포함된 페이지에 표시되지 않습니다. NPR-18645, CQ-110253용 핫픽스
* AbstractCopyMoveCommand의 동시 실행 문제 NPR-18591
* 다른 AEM 인스턴스에서 parsys 구성 요소에 텍스트를 복사할 때 resourceType이 설정되지 않은 상태로 parsys가 만들어집니다. NPR-18511, CQ-4212306용 핫픽스

### 플랫폼 {#platform-10}

* JCR 설치 관리자은 패키지 설치 후 번들 버전을 업데이트하지 않습니다. NPR-18728, NPR-15135용 핫픽스
* BLR(Binaryless replication)이 작성 및 게시 환경 사이의 바이너리로 실패합니다. NPR-18704
* AEM 환경에서의 Apache Felix Http Bridge 해상도 요청. NPR-18297
* 구조가 비슷한 여러 페이지를 Sling 콘텐츠 배포와 동시에 복제하면 복제가 실패합니다. NPR-18665, Granite-13712용 핫픽스
* Sling 배포 패키지가 작성되며 자동으로 정리되지 않습니다. NPR-18601, Granite-16183용 핫픽스

### 통합 {#integration-13}

* 라이브러리 폴더에서 게시된 오퍼를 보면 NPE가 발생합니다. NPR-18732, CQ-4214593용 핫픽스
* 활동의 시작/종료 날짜를 특정 날짜에서 &quot;활성화/비활성화 시&quot;로 변경할 때 JCR 및 Target에서 업데이트되지 않습니다. NPR-18612, CQ-104831용 핫픽스
* AEM과 Analytics 통합에는 httpclient 연결에 대해 설정된 연결 또는 소켓 시간 초과가 없습니다. NPR-18497
* AEM과 DTM 통합에는 httpclient 연결에 대해 설정된 연결 또는 소켓 시간 초과가 없습니다. NPR-18495
* AEM과의 Target 통합에는 httpclient 연결에 대해 설정된 연결 또는 소켓 시간 초과가 없습니다. NPR-18494
* AEM과 Search &amp; Promote 통합에는 httpclient 연결에 대해 설정된 연결 또는 소켓 시간 초과가 없습니다. NPR-18493
* Target 활동은 추가 경험을 추가한 후에 비활성화됩니다. NPR-18227, CQ-4201895용 핫픽스

### WCM-Foundation 구성 요소 {#wcm-foundation-components-7}

* 이미지 맵은 HTL 이미지 구성 요소에서 선택한 좌표를 유지하지 않습니다. NPR-18530, CQ-4211584용 핫픽스

### 번역 {#translation-5}

* 번역 검색 결과에 번역 프로젝트의 이름이 포함되지 않습니다. NPR-18224, CQ-4210658용 핫픽스

### Brand Portal {#brand-portal-1}

* AEM에서 tagadmin/tagging 콘솔의 Brand Portal에 태그를 게시하도록 설정합니다. CQ-4212165

## 양식 {#forms-13}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-13}

#### 서신 관리 {#correspondence-management-6}

* 조각을 저장할 때까지 정확한 데이터가 편집 패널에 표시되지 않습니다. NPR-19092
* 편지에 문서 조각을 추가하는 데에는 상당한 시간이 소요됩니다. NPR-18958
* 데이터 XML 파일에 XML 선언이 있고 POST 요청을 통해 편지 렌디션이 시작된 경우 해당 편지에는 데이터가 표시되지 않습니다. NPR-18870
* CM 에셋에 대해 수행한 작업에 대한 감사 로그가 생성되지 않습니다. NPR-16618

>[!NOTE]
>
>아래의 두 가지 상황으로 인해 문제가 발생하는 경우 이 CFP 추가 기능 패키지를 설치하지 마십시오.
>
>* Word/웹에서 CM 텍스트 편집기로의 복사 붙여넣기 기능은 줄바꿈 콘텐츠를 보여 줍니다. NPR-19530
>* CM 텍스트 편집기에서 줄바꿈하지 않는 콘텐츠는 감싸지지 않습니다. NPR-19449

>
>이러한 요구 사항은 향후 CFP에서 논의될 것입니다.

#### 적응형 양식 {#adaptive-forms-9}

* 반복 가능한 패널에 새 패널을 추가하면 이전 패널의 드롭다운 필드 값이 삭제됩니다. NPR-18772
* 정수만 수락하도록 표시된 적응형 양식 필드는 숫자 패드에서 일부 특수 문자도 사용할 수 있습니다. NPR-18680
* 안내서 루트 패널의 초기화 시 버튼 제목을 변경하는 스크립트가 작동하지 않습니다. NPR-18476
* 규칙 편집기에 생성된 규칙에 대한 스크롤바가 오른쪽 패널에 표시되지 않습니다. NPR-18716

#### AEM Forms 앱 {#aem-forms-app}

* Forms는 오프라인 모드이거나 네트워크에 연결되지 않은 경우 AEM Forms 앱에서 제대로 렌더링되지 않습니다. CQ-4218368

### Forms JEE 설치 관리자  {#forms-jee-installer-13}

#### PDFG 서비스 {#pdfg-service-3}

* PDF 생성기가 지정된 책갈피 수준으로 PDF 문서를 생성하지 못했습니다. CQ-4211102용 핫픽스

## CFP7에 포함된 OSGi 번들 {#osgi-bundles-included-in-cfp-1}

AEM 6.2 SP1-CFP7에서 업데이트된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/bundle-list-6_2sp1cfp7.txt)

AEM 6.2 SP1-CFP7에서 업데이트된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/cfp7_content_packages.txt)

AEM 누적 수정 팩 6.2 SP1-CFP6은 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 태블릿의 레이아웃 모드에서 숨겨진 구성 요소를 효율적으로 관리할 수 있습니다.
* 하이브리드 디바이스에 대한 빠른 작업을 도입했습니다.
* 라이브 카피 관련 구성 요소 수준 동기화 문제 해결을 제공합니다.

### 자산 {#assets-13}

* 권한이 없는 사용자가 에셋에 대한 작업을 이동하려고 하면 고객이 차단됩니다. NPR-18330, CQ-4212560용 핫픽스
* 여러 스마트 콘텐츠 서비스 구성을 병합하면 유용성 문제가 발생합니다. NPR-18273, CQ-4201557용 핫픽스
* 승인 후 타임라인 콘솔에서 체크아웃 작업/워크플로를 사용할 수 없습니다. 80개의 조각이 Assets 폴더에 추가됩니다. NPR-18257, CQ-4211214 및 NPR-18251용 핫픽스, CQ-4211216용 핫픽스.
* 메모리 부족 시 시스템 충돌이 발생하고 Assets 보고서 중 페이지 매김이 부족하게 됩니다. NPR-17865, CQ-4209759용 핫픽스
* 게시된 비디오가 인코딩된 비디오 에셋에서 재생되지 않습니다. NPR-17849, Hotfix for CQ-4210739
* PDF용 썸네일이 생성되지 않습니다. NPR-17831, NPR-17750, CQ-4210547용 핫픽스
* 만료된 에셋이 Adobe CQ DAM 만료 알림 작업에 의해 비활성화되지 않습니다. NPR-17666, CQ-107766용 핫픽스
* 에셋에 지정된 소유자가 없으면 에셋 만료 활동이 중지됩니다. NPR-17665, CQ-4197946용 핫픽스
* 들어오는 참조가 150개 이상인 에셋 폴더를 이동하면 null 포인터 예외가 발생합니다. CQ-4200981

### 사이트 {#sites-13}

* 개인화는 IP 범위에 대한 세그멘테이션 규칙이 설정된 경우 첫 번째 IP에서만 작동합니다. NPR-18121, CQ-83767용 핫픽스
* historyShow 속성이 활성화된 경우 NumberFormatException으로 인해 로그인에 실패합니다. NPR-18073, CQ-101965용 핫픽스
* 표시된 삭제 페이지가 Touch UI에 표시됩니다. NPR-18025, CQ-86694용 핫픽스
* 대상이 큰(2000 이상) 페이지를 로드할 때 성능 문제가 발생합니다. NPR-17884, CQ-4209567용 핫픽스
* 페이지에서 다른 이미지를 제거한 후에는 이미지를 선택할 수 없습니다. NPR-17711, CQ-4201323용 핫픽스

### 플랫폼 {#platform-11}

* 필수 권한이 없는 사용자에게 Touch UI 컨트롤을 숨기지 않습니다. NPR-17945, CQ-4211231용 핫픽스
* 태그 선택기 필드에 일본어 태그가 없습니다. NPR-17768, CQ-4210456용 핫픽스
* FastQuerySize가 활성화되면 getsize() 쿼리에서 잘못된 결과를 반환합니다. NPR-18018
* 대기 인스턴스의 웹 콘솔에 액세스할 수 없습니다. NPR-17861, Granite-14582용 핫픽스

### 상거래 {#commerce-2}

* 카탈로그 블루프린트에 섹션에 대해 정의된 조건이 없으면 쿼리 순회가 발생합니다. NPR-18229, CQ-4211924용 핫픽스

### 커뮤니티 {#communities-2}

* PollingImporterImpl. AEM 종료를 지연합니다. NPR-18298, CQ-96133용 핫픽스

### 통합 {#integrations}

* AEM Day HTTP Client 3.1 OSGI가 다이제스트 인증을 필요로 하는 프록시로 구성된 경우 발생할 수 있는 AEM 검색 구성 요소 오류가 해결되었습니다. NPR 18128
* 상속을 되돌리는 데 필요한 확인란이 없습니다. NPR-17753, CQ-4210139용 핫픽스 요청
* 여러 활동이 있는 하나의 구성 요소를 타깃팅할 때 우선 순위를 설정할 수 없습니다. NPR-18658, CQ-4210727용 핫픽스
* /etc/segmentation/group1 폴더에 작성된 대상을 선택하기 위해 folder /etc/segmentation 폴더를 찾을 수 없습니다. NPR-18522

### 보안 {#security-1}

* 사용자에게 대상 폴더에 대한 쓰기 권한이 없는 경우 에셋 이동 마법사가 중단됩니다. NPR-18300
* XSS 취약성을 선점하기 위해 Apache Sling API에서 업그레이드된 버전의 org.apache.sling.servlets.post 서블릿(2.3.22)을 사용하도록 요청합니다. NPR-18963

### 번역 {#translation-6}

* 프로젝트가 완료될 때까지 에셋 페이지를 번역 프로젝트에 다시 제출할 수 없습니다. NPR-18249, CQ-4209908용 핫픽스

### WCM-Foundation 구성 요소 {#wcm-foundation-components-8}

* 편집 가능한 템플릿에서 WCM 기반 iparsys 구성 요소를 사용할 수 없습니다. NPR-18223, CQ-4210384용 핫픽스
* 이미지 맵은 HTL 이미지 구성 요소에서 선택한 좌표를 유지하지 않습니다. NPR-18032, CQ-4211584용 핫픽스
* HTL 이미지 구성 요소가 렌더링될 때 URL의 파일 이름이 바뀌면서 잘못된 URL이 발생합니다. NPR-17908, CQ-4211587용 핫픽스
* 변경한 후 페이지 속성을 종료할 수 없습니다. NPR-17832, CQ-96110용 핫픽스

## 양식 {#forms-14}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-14}

**서신 관리**

* 데이터 사전을 편지 렌더링 중에 반복적으로 읽습니다. NPR-18482, CQ-4210805용 핫픽스
* com.adobe.livecycle.content 클래스에 대한 JavaDocs가 추가되었습니다. NPR-18467
* 편지를 작성할 때 편지에 대한 설명이 저장되지 않습니다. NPR-18039
* 텍스트 모듈이 저장되고 텍스트 모듈의 표현식에 열기 또는 닫기 표현식 태그가 없으면 오류 메시지가 표시되지 않습니다. 텍스트 모듈에 오류 메시지가 표시되고 편지에서 렌더링되지 않습니다. NPR-17798
* 추가 기능 패키지 설치 시 로그에 예기치 않은 오류가 표시됩니다. NPR-18295

**Forms Manager**

* AEM Forms UI는 가장 오래된 첫 번째 주문의 모든 에셋을 나열합니다. 사용자가 최신 순서로 에셋을 재정렬할 수 없습니다. NPR-18451

### Forms JEE 설치 관리자  {#forms-jee-installer-14}

**출력 서비스**

* AEM Forms 6.2용 출력 서비스의 성능 문제가 개선되었습니다. NPR-18033

**서명 서비스**

* 원격 하드웨어 보안 모듈을 사용하여 PDF 문서에 서명할 수 없습니다. NPR-18017

## CFP6에 포함된 OSGi 번들 {#osgi-bundles-included-in-cfp-2}

AEM 6.2 SP1-CFP6에서 업데이트된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/6.2sp1-cfp6-bundlelist.txt)

AEM 6.2 SP1-CFP6에서 업데이트된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/6_2sp1-cfp6-contentpackagelist.txt)

AEM 누적 수정 팩 6.2 SP1-CFP5는 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 에셋 공유, 이동, 게시 및 다운로드와 관련된 여러 UI 문제가 해결되었습니다.
* 참조된 에셋을 표시할 때 이동 대화 상자의 용량을 늘렸습니다.
* 게시 취소 및 버전 삭제와 같은 WCM 구성 요소 및 워크플로와 관련된 여러 문제가 해결되었습니다.
* 도구 모음 작업 및 Coral 구성 요소 표시와 관련된 작업 표시줄의 응답성이 개선되었습니다.

### 자산 {#assets-14}

* Brand Portal에 게시 기능의 성능이 개선되었습니다. NPR-17189, CQ-4204150용 핫픽스
* 링크 공유 옵션을 사용하여 에셋을 공유해도 다운로드할 기본 폴더 구조가 있는 zip 파일이 만들어지지 않습니다. NPR-17513, CQ-4209381용 핫픽스
* DAM에서 에셋을 선택하고 게시를 클릭해도 에셋 세부 사항 페이지에 Brand Portal에 게시 옵션이 표시되지 않습니다. NPR-17351, CQ-94905용 핫픽스
* DAM 워크플로 단계의 Session 또는 ResourceResolver에서 얻은 이진 스트림은 마지막 블록에서 닫아야 리소스 누수가 발생하지 않습니다. NPR-17385, CQ-4209452용 핫픽스
* DAM에서 Word 문서를 업로드하면 null 포인터 예외가 발생하고 워크플로 인스턴스가 실행 중 상태로 남아 있습니다. NPR-17160, CQ-4207358용 핫픽스
* 관리자가 아닌 사용자를 위해 메타데이터 편집기 페이지에서 만료된 에셋에 대해 공유, 이동, 게시 및 다운로드 버튼이 표시됩니다. NPR-16903, CQ-101440/CQ-104535용 핫픽스
* 공유, 이동, 게시 및 복사와 같은 작업은 Assets 콘솔에서 관리 사용자가 볼 수 있어야 합니다. NPR-16902, CQ-4207111용 핫픽스

### 사이트 {#sites-14}

* 클래식 UI나 Touch UI를 사용하여 페이지를 이동하는 동안 이동 대화 상자에 150개를 넘는 참조가 표시되지 않아서 사용자가 이러한 참조를 업데이트하고 페이지를 다시 게시할 수 없습니다. 이 문제는 siteadmin 노드: &#39;/libs/wcm/core/content/siteadmin&#39;에 구성할 수 있는 클래식 UI: &#39;maxRefNo&#39;의 속성을 도입하면서 해결되었습니다. 이 속성은 대량 이동 작업 전에 표시되는 최대 참조 수(기본값 150)를 지정하며 페이지에 더 많은 수의 참조가 있는 경우 movePage 대화 상자에 표시되지 않습니다. 이 구성은 노드에 구성을 적용하여 damadmin 및 miscadmin에도 작동합니다. 각각 `'/libs/wcm/core/content/damadmin'` 및 `'/libs/wcm/core/content/miscadmin'`. NPR-17222, CQ-85878용 핫픽스

* WCM 구성 요소로 작업하는 동안 공백이 포함된 하이퍼링크는 Touch UI 리치 텍스트 편집기에서 제거됩니다. NPR-17698, NPR-17570, CQ-4206768용 핫픽스
* 페이지 속성에서 게시 취소 요청 워크플로를 트리거하면 복제 권한이 없는 사용자에 대해 JavaScript 오류가 표시됩니다. NPR-17294, CQ-102064용 핫픽스
* HTL 이미지 구성 요소를 렌더링하거나 내보내면 URL이 숫자로 변경되고 파일 이름을 바꾸면 링크가 끊어집니다. NPR-17245, CQ-59616용 핫픽스
* 중첩 실행에서 실행을 삭제하면 하위 실행이 고립됩니다. NPR-17228, CQ-4202639용 핫픽스
* Oak 1.4.13이 적용된 AEM 6.2에서 버전 삭제를 실행하면 로그에 경고가 지속해서 반복 표시됩니다. NPR-17391, CQ-4206870용 핫픽스
* ContextHub 구성 요소에 대한 핫픽스 또는 업그레이드를 설치한 후, 콘텐츠 패키지는 /etc/segmentation/contexthub의 모든 세그먼트를 덮어쓰므로 모든 사용자 지정 ContextHub 세그먼트가 손실됩니다. NPR-17250, CQ-79958용 핫픽스
* 워크플로 사용자로 중첩된 그룹이 포함된 워크플로를 실행하는 동안 WorkflowStatusProvider(pageinfo.json)에서 워크플로 인스턴스를 잠급니다. NPR-17555, CQ-4202056용 핫픽스
* WCM 페이지 편집기 구성 요소를 사용하는 동안 작성 인스턴스의 Touch UI 편집 모드에서 페이지 끝에 많은 빈 공간이 있습니다. NPR-17510, CQ-4205441용 핫픽스
* HTL 이미지 구성 요소를 렌더링하거나 내보내면 URL이 숫자로 변경되므로 링크가 끊어집니다. NPR-17245, CQ-59616용 핫픽스

### UI {#ui}

* 에셋을 선택하고 개발자 도구를 클릭해도 작업 표시줄의 도구 모음 작업이 느린 연결로 항상 표시되지는 않으며 페이지를 다시 로드해야 합니다. NPR-17568, CQ-108365용 핫픽스
* 작업 표시줄을 2개의 컨테이너를 사용하도록 업데이트해야 합니다. coral-actionbar-container 대신 coral-actionbar-primary 및 coral-actionbar-secondary를 사용합니다. NPR-17591, GRANITE-15225용 핫픽스

### Mobile-on-demand {#mobile-on-demand-2}

* AEM Mobile 앱에 대한 &#39;읽기 전용&#39; 권한이 있는 사용자는 AEM Mobile 콘텐츠 관리 페이지에서 콘텐츠를 미리 볼 수 없습니다. NPR-17390, CQ-4209690용 핫픽스

### 보안 {#security-2}

* HTMLRendererServlet에 의해 생성된 출력의 XSS 취약성. NPR-17136
* AEM Web Syndication Feeds 페이지의 AEM 버전 공개를 방지하는 요청. NPR-16219

### 양식 {#forms-15}

#### Forms 추가 기능 패키지 {#forms-add-on-package-15}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

**적응형 양식**

* 첨부 파일이 있는 적응형 양식의 경우 양식이 두 번째로 제출될 때 afSubmissionInfo 태그에 대한 중복 항목이 제출된 XML에 생성됩니다. NPR-17364
* Google Chrome 브라우저를 사용하는 동안 양식에서 첨부 파일을 제거한 후 동일한 첨부 파일을 다시 첨부하려고 하면 오류가 발생합니다. NPR-17297
* XSD 기반 또는 양식 없는 모델 기반의 적응형 양식에 중첩된 반복 가능한 지연 로드 패널이 있는 경우 양식에 입력된 값이 DOR(Document of Record)에 유지되지 않습니다. NPR-17176
* 규칙 편집기의 오류 로그에 표시되는 오류는 try/catch 블록 JavaScript 코드의 catch 블록에 추가해야 합니다. NPR-16757
* 양식의 파일 첨부 파일을 클릭하면 브라우저 콘솔 오류가 발생하고 첨부 파일 미리보기가 표시되지 않습니다. NPR-17174

**서신 관리**

* UI에 인라인 텍스트 또는 빈 줄이 추가되는 경우에 대비해 서신 UI 만들기 기능이 중단됩니다. NPR-17748
* 편집을 위해 편지를 열면 브라우저가 깜박입니다. NPR-17576
* 계산된 데이터 사전 요소에서 원격 함수를 추가하는 동안 함수 개수가 원격 함수를 표시하는 탭의 길이보다 많으면 스크롤바가 탭에 나타나지 않습니다. NPR-17359
* API 메서드, import com.adobe.icc.services.api.LetterInstanceService가 작동하지 않습니다. NPR-17922, NPR-16008
* 편지를 편집하는 동안 텍스트 모듈에 추가된 변수가 데이터 바인딩 패널에 표시되지 않습니다. NPR-17940
* HTML 제출 작업에서 POST 메서드를 사용하는 경우 서신 관리 UI가 시작되지 않습니다. NPR-17595

**Forms Manager**

* AB 테스트를 위해 구성된 적응형 양식을 사용하여 AB 테스트 시작을 클릭해도 테스트가 시작되지 않고 브라우저 콘솔 오류가 발생합니다. NPR-17838

**Forms 서비스**

* OSGI 양식의 정적 코드 분석에 보고된 문제를 해결해야 합니다. NPR-13951

#### Forms JEE 설치 관리자 {#forms-jee-installer-15}

**출력 서비스**

* AEM Forms 6.2 출력 서비스를 사용하여 특정 양식을 데이터 XML과 병합하는 경우 LiveCycle ES4 SP1 서버에서 동일한 작업을 수행하는 데 걸리는 시간에 비해 20배 더 많은 시간이 소요됩니다. Windows 및 Linux 환경에서 수정되었습니다. NPR-17501

**LCM 설치**

* AEM Forms 6.2 GM 빌드를 설치하고 AEM 6.2 CFP를 적용한 후 LiveCycle 구성 관리자를 실행하면 버전 정보에 원치 않는 세미콜론이 표시되고 패치 설치 날짜는 업데이트되지 않습니다. NPR-14322

**프로세스 관리**

* TaskContext 변수가 AEM Forms 프로세스에 대해 채워지지 않습니다. CQ-4211857

#### AEM Forms JEE 번들 패키지 {#aem-forms-jee-bundles-package}

* JEE 관리 UI 콘솔 또는 OSGi 콘솔 사용에 대한 Forms 사용자의 기능은 동일해야 합니다. NPR-17670

### CFP5에 포함된 기능 팩 {#feature-packs-included-in-cfp}

**Forms JEE 패키지**

프로세스 관리 - HTML 작업 공간

* 작업 공간 단계를 지정하는 동안 첨부 파일 또는 메모가 둘 이상 있을 경우 작업 공간 첨부 파일 탭에 첨부 파일 또는 메모에 대한 카운터가 표시됩니다. NPR-17771
* 양식 워크플로에서 이메일 기능을 지원하기 위해 AEM JEE Forms의 Office 365를 지원하도록 요청합니다. NPR-13866

**Forms 추가 기능 패키지**

서신 관리

* 편지 미리보기 중에 텍스트 편집기에서 조각을 편집하는 동안 조각에 사용된 인라인 조건 대신 편집을 위해 처리된 텍스트를 표시해야 합니다. NPR-15748, NPR-17504

### CFP5에 포함된 OSGi 번들 {#osgi-bundles-included-in-cfp-3}

AEM 6.2 SP1-CFP5 간에 업데이트된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/cfp5_osgi_bundles.txt)

AEM 6.2 SP1-CFP5 간에 업데이트된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/content-package-cfp5.txt)

AEM 누적 수정 팩 6.2 SP1-CFP4는 AEM 6.2 SP1의 일반 공급 이후 릴리스된 주요 고객 수정 사항이 포함된 중요한 업데이트입니다.

이 누적 수정 팩의 주요 사항은 다음과 같습니다.

* Camera Raw 파일 렌디션, 타임라인 보기 및 이미지 방향에 대한 에셋의 수정 사항
* 향상된 기능

   * 사이트에 대한 WCM 실행
   * 프로젝트 워크플로
   * ContextHub 구성 요소

* Campaign, Mobile on-demand 및 번역 수정 사항
* 적응형 양식 규칙 편집기의 유용성 개선 사항
* 양식의 서신 관리를 위한 인라인 조건 편집기 개선
* JEE 기반의 AEM Forms에 대한 프로세스 관리 및 출력 서비스 수정 사항
* Forms Designer 관련 스크립트 편집기 수정

### 플랫폼 {#platform-12}

* 클라우드 서비스를 구성할 때 Search &amp; Promote 검색 양식에서는 `environment` 설정을 무시하고 작성자 인스턴스에서 이 설정을 사용할 수 없습니다. NPR-16594: CQ-4206076용 핫픽스
* /apps에 오버레이하여 **Assets OmniSearch** 결과에 열을 추가 또는 사용자 지정할 수 없습니다. NPR-16737: CQ-4206785용 핫픽스
* AEM 6.1 SP2에서 AEM 6.2 SP1로 업그레이드한 후 **진단 도구 **페이지가 작동하지 않습니다. NPR-17121, CQ-4196786용 핫픽스
* HTL: 포럼을 선택하는 동안 주제와 게시물을 만들면 `Sightly SightlyCompiledScript`에서 잘못된 `addSelectors` 속성을 `RequestDispatcherOption`에 추가합니다. NPR-17008: GRANITE-16384용 핫픽스

* `ReportImporter`에서 사용하는 `ManagedPollConfigs`에서 `CRON expressions`에 대한 지원을 추가했습니다. NPR-16608: CQ-4206066용 핫픽스 요청

* LDAP 사용자에 대한 아바타 이미지를 업로드하지 못했습니다. NPR-16561, Granite-17013용 핫픽스
* 사용자 관리 화면에 표시되는 결과 수가 카드 및 목록 보기에서 다릅니다. NPR-16241, GRANITE-16914용 핫픽스
* 전체 화면 모드로 Google Chrome 브라우저에서 보는 동안 워크플로 알림을 지연할 수 없습니다. NPR-17013: CQ-4207567용 핫픽스

### 자산 {#assets-15}

* 정의된 방향이 있는 이미지를 가져오는 동안 이미지 방향이 올바르게 적용되지 않습니다. NPR-16750: CQ-4204356용 핫픽스
* &#39;모두 표시&#39;가 기본적으로 설정되어 있어도 에셋 타임라인 보기에는 에셋이 표시되지 않습니다. NPR-16957: CQ-98780용 핫픽스
* Camera Raw 파일(ARW, CR2, NEF, DNG 및 EPS 포함)은 에셋에서 렌디션으로 추가할 때 선택하거나 삭제할 수 없습니다. 이러한 파일은 사용자가 클릭하면 자동으로 다운로드됩니다. NPR-16949: CQ-4206846용 핫픽스
* Assets UI에서 다른 pdf에 pdf를 만들면 crx 저장소에 표시되어도 DAM UI에 작성된 pdf가 표시되지 않습니다. NPR-16833: CQ-4206501용 핫픽스
* Touch UI를 사용하여 에셋을 직접 하위 노드로 업로드하면 문제가 발생합니다. 에셋이 이전에 선택한 에셋의 직접 하위로 업로드됩니다. NPR-16534: CQ-4204287용 핫픽스
* DAM UI에서 에셋에 대해 댓글을 달거나 댓글에 있는 사용자에게 태그를 지정하면 메일 알림이 생성되지 않습니다. NPR-16589: CQ-102318용 핫픽스

### 프로젝트 {#projects-3}

워크플로가 삭제되면 프로젝트 워크플로 콘솔에 페이지의 NullPointerException이 표시됩니다. NPR-17017: CQ-4194269용 핫픽스

### 사이트 {#sites-15}

* 작성자 인스턴스에서 `ContextHub`의 파일이 최소화되지 않습니다. NPR-17022: CQ-79456용 핫픽스
* WCM-Launch 실행 프로모션의 경우 페이지의 대형 트리로 구성된 실행을 프로모션하는 데 오랜 시간이 소요됩니다. NPR-16480: CQ-82731용 핫픽스
* `ClientContext` 세그먼트 조건 렌더러는 작업 중이 아니거나 완료되지 않은 규칙을 사용하여 세그먼트(또는 대상)를 만들 때 충돌합니다. NPR-16759: CQ-4205104용 핫픽스
* WCM Launch에서 Touch UI의 페이지 속성 내에서 작업이 시작되어도 Launch와 연관된 페이지는 게시 취소되지 않습니다. NPR-16560: CQ-4204681용 핫픽스
* 링크 재작성자는 콜론 &quot;:&quot;이 JCR 네임스페이스를 정의한다고 가정하여 콜론을 포함하는 href 값을 올바르지 않게 다시 기록합니다. NPR-16753: CQ-4203762용 핫픽스
* WCM-Design Importer에서 테스트 Importer 페이지를 열고 zip 파일을 업로드하려고 하면 이전에 업로드 및 삭제된 경우 문제가 발생합니다. NPR-16486: CQ-90962용 핫픽스
* Firefox Safari 및 Google Chrome 브라우저를 사용하여 **[!UICONTROL 전역 탐색]** 창으로 이동하면 다른 사용자 경험이 제공됩니다. Firefox 브라우저에는 **[!UICONTROL 도구]** 메뉴가 표시되지만 Google Chrome 브라우저에는 **[!UICONTROL 탐색]** 메뉴가 표시됩니다. NPR-16770, CQ-4200456용 핫픽스

### 캠페인 {#campaign}

* AEM Campaign 템플릿을 테스트하고 시드 주소를 수정하여 &#39;추가 데이터&#39;를 포함하는 동안 Adobe Campaign 드롭다운이 Touch UI 컨텍스트 허브에서 사라집니다. NPR-16771: CQ-105748용 핫픽스

### Mobile On-Demand {#mobile-on-demand-3}

* AEM 작성 환경에서 발행물을 사전 점검할 때 5초 이상 걸리는 사전 점검 작업이 있으면 AEMM - AEM PECS 통합 splunk 대시보드에 초당 높은 상태 요청이 있는 비정상적인 스파이크가 발생합니다. NPR-16908: CQ-4207055용 핫픽스
* AEM-6.2-SP1-CFP1-1.0 업데이트를 설치한 후 AEM Mobile 구성 관리에 실패합니다. NPR-16909: CQ-4204892용 핫픽스

### 번역 {#translation-7}

* 6.2 SP1 - CFP1을 설치한 후에는 번역 작업 미리보기가 작동하지 않습니다. NPR-16481, CQ-4204655용 핫픽스
* 번역 기능을 사용하여 만든 언어 사본이 로컬 국가 Live Copy 대신 루트 마스터를 가리킵니다. NPR-17257, CQ-4208287용 핫픽스

### 보안 {#security-3}

* 파일 바이너리를 AEM에 업로드할 때 MIME 유형 유효성 검사가 수행되지 않습니다. NPR-16617
* LDAP 사용자에 대한 아바타 이미지 업로드 시 문제가 발생합니다. NPR-16561

### 양식 {#forms-16}

#### Forms 추가 기능 패키지 {#forms-add-on-package-16}

**적응형 양식**

* 적응형 양식 편집기에서 head.jsp의 Target 설정 주석을 새 Context Hub 문으로 바꿔야 합니다. NPR-17173
* 적응형 양식 규칙 편집기에서 **[!UICONTROL 항목 선택]**&#x200B;은 이벤트를 &#39;null&#39;로 표시합니다. NPR-17139
* 제출된 양식은 앞으로 이동 시 화살표(>)를 사용하여 다시 제출됩니다. NPR-17080
* AJAX을 통해 적응형 양식을 제출하는 동안 오류가 발생할 경우 &#39;error&#39; 콜백 함수가 호출되지 않습니다. NPR-17034
* 런타임에 규칙 편집기에서 **[!UICONTROL 양식 저장]** 버튼을 클릭해도 양식이 저장되지 않습니다. NPR-16905
* 정적 텍스트는 적응형 양식의 탭 순서에서 제외해야 합니다. NPR-16749
* 십진수 필드의 계산된 값이 잘못 표시됩니다. NPR-16596
* 도움말 콘텐츠를 표시하는 아이콘은 적응형 양식의 탭 순서에 포함되어야 합니다. NPR-16484
* 적응형 양식의 미리 채우기에 대한 &#39;**[!UICONTROL 기본 자동 완성 서비스 구성]**&#39;에서 `dataRef=C:/Users/` 유형의 정규 표현식 사용을 지원합니다. NPR-16425

* 중첩된 지연 로드 시나리오가 있는 경우 모든 패널에 대한 유효성 검사가 올바르게 트리거되지 않습니다. NPR-15821

**서신 관리**

* 한 편지에 텍스트가 없는 빈 텍스트 모듈이 포함되어 있으면 편지 렌디션이 실패합니다. NPR-17054
* 텍스트 편집기에 붙여넣은 후 줄바꿈과 탭 공간이 콘텐츠에서 제거됩니다. NPR-17039
* 텍스트 모듈을 여러 편지에서 참조하는 경우 텍스트 모듈의 참조를 표시하는 데 많은 시간이 소요됩니다. NPR-17035
* 문서 조각에 대한 참조를 편집, 저장, 삭제 및 설정하는 데 많은 시간이 소요됩니다. NPR-17033
* 텍스트를 미리 볼 때 균등 배치된 텍스트가 다른 글꼴로 렌더링됩니다. NPR-16976
* 검색된 텍스트에 여러 항목이 있는 경우 검색 기능이 제대로 작동하지 않습니다. NPR-16920
* 텍스트 편집기 도구 모음이 간헐적으로 브라우저에 표시됩니다. NPR-16919
* 규칙 편집기에서 **[!UICONTROL 양식 저장]** 구성이 작동하지 않습니다. NPR-16905
* Internet Explorer를 사용하여 데이터 사전을 기반으로 텍스트 모듈을 만들 때 글꼴 드롭다운에서 글꼴 모음을 채우지 않습니다. NPR-16944
* 텍스트 조각을 만든 후 편지 글꼴이 편지 미리보기 시 변경됩니다. NPR-16830
* 문서 조각의 표현식 시작 또는 사이에 탭 공백이 있는 문자는 렌더링하거나 미리 볼 수 없습니다. NPR-16769

**Mobile Forms**

* PDF 렌더링에 대하여는 양식이 올바르게 표시되지만 Mobile Form 미리보기에는 겹치는 내용이 표시됩니다. NPR-17105

**Forms 포털**

* 제출된 양식에 대해 **[!UICONTROL 다운로드]** 링크를 클릭하면 PDF 양식 대신 HTML 페이지가 열립니다. NPR-17082

* `Upload Comments` crx 저장소에 저장된 XML에 파일의 첨부 파일이 있어도 제출되는 인스턴스의 UI에 해당 첨부 파일이 표시되지 않습니다. NPR-17075

**Reader 확장 서비스**

* AEM Forms OSGI 설치 시 특정 파일이 Reader 확장이 아닙니다. NPR-16625

#### Forms JEE 설치 관리자  {#forms-jee-installer-16}

**코어**

* 업그레이드 프로세스 중에 구성 관리자가 시간 초과로 실패합니다. NPR-16774([구성 요소 수준에서 작업 시간 제한 구성하기](install-cfp-aem-forms-jee.md#configuring-timeout-for-operations-at-component-level-npr) 참조).

**프로세스 관리 - HTML 작업 공간**

* 작업 시작의 시작점은 시작점 제출 시 제출된 데이터로 시작하지 않습니다. NPR-16917
* HTML 작업 공간에서 양식에 대한 **[!UICONTROL 반환]** 버튼을 클릭해도 양식이 닫히지 않고 해당 그룹 큐로 돌아갑니다.\
   NPR-16352

**프로세스 관리**

* 이전 작업의 표시 이름을 프로세스 인스턴스의 다음 작업 중 하나로 설정할 수 있도록 허용합니다. NPR-15382

**출력 서비스**

* 출력 서비스에서 `date-time format` 메타데이터에 추가 &#39;milli-sec&#39; 필드를 포함하도록 수정된 PDF를 처리하지 못합니다. NPR-16838

#### Forms 디자이너 {#forms-designer}

* AEM Designer 스크립트 편집기에서 `Calculate Event` 및 `Validate Event`의 양식 속성 기본값을 고려하지 않습니다. NPR-15921

### CFP4에 포함된 기능 팩 {#feature-packs-included-in-cfp-1}

**Forms 추가 기능 패키지**

* 서신 관리를 위한 인라인 조건 편집기의 개선 사항. NPR-10981

### CFP4에 포함된 OSGi 번들 {#osgi-bundles-included-in-cfp-4}

AEM 6.2 SP1과 CFP4 간에 업데이트된 OSGi 번들 목록

CFP3의 주요 특징:

* 다이제스트 인증이 있는 프록시를 사용하여 클래식 UI 및 AEM 검색 구성 요소에 대한 보다 효율적인 검색 기능 제공
* 에셋 업로드 및 에셋 메타데이터 표시 중 발생한 문제가 해결되었습니다.
* 제목에 특수 문자가 있을 경우 폴더를 만들고 페이지를 이동하는 동안 발생했던 문제가 수정되었습니다.
* 대상 동기화, 캠페인 게시 및 Touch UI에서 목표 지표 선택을 위한 타깃팅 수정
* 번역 작업의 동기화 문제 해결
* Forms 미리 채우기 서비스에 대한 보안 개선
* 양식 포털 초안 및 제출 구성 요소와 Barcoded Forms Service의 개선 사항
* 첨부 파일 위젯 또는 지연 로드된 조각을 포함하는 적응형 양식의 유용성 개선 사항.
* 향상된 검색 기능, 삭제된 에셋 로깅 및 데이터 사전 가져오기 등 서신 관리의 유용성 개선 사항.

### 플랫폼 {#platform-13}

* **ModelAdapterFactory**&#x200B;의 경쟁 조건이며 두 스레드에서 동일한 필드를 주입하려고 하면 모델을 구성하지 못할 수 있습니다. NPR-16443, SLING-6584용 핫픽스
* /apps 아래의 오버레이된 파일(JSP 또는 JavaScript 파일)과 /libs 아래의 핫픽스에 포함된 파일 간 충돌을 감지하는 패키지 관리자의 유효성 검사 옵션입니다. 그런 다음 /libs 아래에 있는 파일의 변경 사항을 포함하도록 영향을 받는 오버레이를 다시 사용할 수 있습니다. NPR-16216: CQ-81729용 핫픽스
* error.log에 로그인하면 가끔 게시자를 시작한 후 몇 초 후에 중지되며 다시 실행하려면 지워야 합니다. 로깅 프레임워크를 업데이트하고 Sling 로깅을 제공하도록 요청합니다. NPR-15913: Granite-15452용 핫픽스
* HTL JavaScript 사용 API 구현의 실패를 방지하기 위해 JavaScript &quot; `use"` API를 업데이트하도록 요청합니다. NPR-16461: SLING-6780용 핫픽스

### 사이트 {#sites-16}

* AEM 6.0에서 AEM 6.2로 업그레이드한 후 많은 쿼리로 인해 태그를 검색하는 동안 클래식 UI의 성능이 저하됩니다. 이 문제를 해결하려면 [태깅 콘솔에서 복제 상태 비활성화(클래식 UI)](release-notes-aem-6-2-cumulative-fix-pack.md#disable-replication-status-in-tagging-console-classic-ui-npr)에 설명된 단계를 따를 수 있습니다. NPR-15842: CQ-4201748용 핫픽스.

* Touch UI에서 페이지를 만드는 동안 &#39;이름&#39; 필드에 대한 입력 확인은 특수 문자 &#39;아포스트로피&#39;(클래식 UI에서와 동일)를 확인하지 않습니다. 따라서, 페이지를 이동할 수 없습니다. NPR-16404: CQ-4205321용 핫픽스.
* 리치 텍스트 편집기에서 두 행에 다른 스타일을 적용한 다음 병합하면 두 번째 행에 적용된 스타일이 제거됩니다. NPR-16389: CQ-4203835용 핫픽스.
* Touch UI 사이트 화면에서 하위 페이지가 없는 페이지에 페이지를 붙여넣으려고 하면 붙여넣기 버튼이 나타나지 않으므로 작동하지 않습니다. NPR-15894: CQ-4201696용 핫픽스.
* 콘텐츠 파인더 패널에서 페이지 탭을 스크롤하는 동안, 몇 개의 페이지 세트는 클래식 UI에 무제한 표시되는 반면 Touch UI는 반복되지 않는 몇 개의 제한된 페이지 집합을 표시합니다. NPR-16271: CQ-4202371용 핫픽스
* Touch UI에서 LiveCopy의 페이지 속성을 열고 변경 사항 없이 저장을 클릭하면 LiveCopy 탭이 기록되고 LiveSync 구성 노드가 만들어집니다. NPR-16327: CQ-108562용 핫픽스
* 양식 제한으로 `ConstraintMessage` 속성을 읽을 수 없습니다. NPR-16388: CQ-101330용 핫픽스
* `wcm/foundation/components/parsys` 구성 요소는 **[!UICONTROL &#39;구성 요소를 여기로 드래그하십시오]**&#39; 자리 표시자가 표시되지 않습니다. NPR: 16748: CQ-4205187용 핫픽스

### 자산 {#assets-16}

* 6.2 SP1 또는 Hotfix 12430을 설치한 후 pdf 래스터라이저 기능 작동이 중단되고 메모리 부족 문제가 발생합니다. NPR-15991
* 문자열 속성의 메타데이터 `documentNumber`가 날짜로 표시되지만 숫자여야 합니다. NPR-16134: GRANITE-16916용 핫픽스
* 타임라인 이벤트 풍선에서 텍스트가 잘립니다. NPR-16226: CQ-85226용 핫픽스
* 제목에 특수 문자가 있는 콘텐츠 계층 구조에 폴더를 만들면 특수 문자의 인코딩된 양식이 표시됩니다. NPR-15935: CQ-4202987용 핫픽스
* &#39;만들기&#39; 버튼을 사용할 때 표시되는 일관되지 않은 동작으로 인해 에셋을 탐색하는 동안 에셋을 업로드하거나 폴더를 만들 수 없습니다. NPR-16410: CQ-4204793용 핫픽스
* AEM 작성의 문서 보기에서 공유 HTML 리소스를 업로드하는 동안 예기치 않은 오류가 발생했습니다. NPR-16133: AEMM-4155970용 핫픽스

### 통합 {#integration-14}

* 다이제스트 인증을 사용하여 프록시 인증을 활성화하면 AEM 검색 구성 요소에 ConcurrentModificationException이 발생합니다. NPR-15309: CQ-4199191용 핫픽스
* AEM에서 Target A/B 테스트 활동을 만들 때 대상이 Target에 동기화되지 않고 &#39;대상 없음&#39;을 표시합니다. NPR-16229: CQ-4204210용 핫픽스
* SP1+NPR-11577 v1.2를 설치한 후 TouchUI에서 타깃팅하는 동안 목표 지표에 대해 &#39;분석 지표 사용&#39;을 선택하면 지표 드롭다운 목록이 로드되지 않습니다. NPR-16129: CQ-4204316용 핫픽스
* 타깃팅을 사용할 때 캠페인을 게시해도 브랜드 및 마스터를 포함한 전체 트리가 자동으로 게시되지 않습니다. NPR-15855: CQ-94630용 핫픽스

### 번역 {#translation-8}

* 번역 작업 동기화가 자동으로 트리거되지 않으며 번역 프로젝트를 시작하지 않으면 AEM에서 폴링을 수행할 수 없습니다. NPR-15163: CQ-90856용 핫픽스

### 양식 {#forms-17}

#### Forms 추가 기능 패키지 {#forms-add-on-package-17}

**적응형 양식**

* 첨부 파일과 함께 적응형 양식을 저장하는 동안 첨부 파일의 전체 경로가 첨부 파일의 이름 대신 생성된 XML의 `fileAttachment` 태그에 추가됩니다. NPR-16529
* XDP 기반 적응형 양식에서는 사전 작성된 XML에 `afData/afBoundData` 래퍼가 없어도 `afData/afBoundData` 래퍼가 제출된 XML에 있습니다. NPR-16118

* 숫자 필드의 지수 표기법: 적응형 양식을 사용하는 동안 총계에서 10자를 초과하는 소수 자릿수를 입력하면, 이 숫자가 제출된 XML에서 지수 표기법으로 바뀝니다. NPR-16106
* 첨부 파일 구성 요소와 지연 로드 조각이 모두 포함된 양식의 경우 제출된 데이터 xml에 첨부 파일 구성 요소에 대한 정보가 포함되지 않습니다. NPR-16022
* 반복 가능한 상위가 없는 지연 로드된 반복 가능 패널의 경우, 패널의 두 번째 인스턴스 내에서 반복 가능한 하위 항목이 반복되지 않습니다. NPR-15944
* 양식 편집기의 조각 내에 조각을 저장하려고 할 때 조각 모델 루트가 하위 조각 값을 채우지 않습니다. NPR-15943
* 한 항목만 포함하는 확인란을 만들고 항목 제목을 숨긴 확인란 제목을 표시하려고 하면 사전 만들기 작업에서 항목 텍스트가 비어 있는 경우 `ArrayIndexOutOfBoundException`이 표시됩니다. 사전이 만들어지지 않고 화면에 오류 응답이 생성되지 않습니다. NPR-15816
* 첨부 파일 위젯이 있는 적응형 양식의 경우 첨부된 파일을 미리 본 후 양식의 일부 부분이 비활성화됩니다.\
   NPR: 16611

* 여러 첨부 파일이 허용되는 파일 첨부 위젯의 경우, 첨부 파일이 있는 새 양식 인스턴스가 이전 첨부 파일이 있는 위젯에 제출되면 실제 콘텐츠 대신 추가된 첨부 파일을 열 때 오류 코드가 표시됩니다. NPR-16258
* `file://`, `http://` 및 `ftp://` 등의 프로토콜을 통해 권한 없는 액세스로부터 양식 미리 채우기 서비스를 보호합니다. [구성 관리자를 사용하여 미리 채우기 서비스 구성하기](https://helpx.adobe.com/aem-forms/6-2/prepopulate-adaptive-form-fields.html#main-pars_header_944235754)를 참조하십시오. NPR-15414

* 확인 단계에서 HTML 대신 PDF 형식으로 적응형 양식을 렌더링하도록 요청하고 모든 첨부 파일을 PDF에 추가하므로 인쇄물에 전체 양식이 표시됩니다. NPR-9011

**서신 관리**

* 미리보기/편집 모드로 편지에서 텍스트 조각을 사용하여 작업하는 동안 텍스트를 목록으로 변환하면 전체 편지 기능이 중단되고 JavaScript 오류가 생성됩니다. NPR-16460
* XSD를 업로드하고 루트 노드를 선택할 때마다 브라우저가 응답하지 않아 서신 관리 노드에서 데이터 사전을 만들기 위해 XSD 파일을 가져올 수 없습니다. 이 문제는 브라우저에 독립적이며 서버 로그에 표시되지 않습니다. NPR-16452
* Internet Explorer 브라우저를 사용하여 문자를 미리 보고 콘텐츠의 글꼴 크기를 편집하려고 하는 동안 글꼴 크기 드롭다운에서 중복 값이 8 ~ 72로 표시됩니다. NPR-16387
* 부동 필드가 XDP 조각의 입력 필드로 표시되는 경우 Internet Explorer 브라우저를 사용하는 동안 필드가 편지 미리보기에서 확장되지 않습니다. NPR-16367
* 미리보기에서 직접 편지를 제출하려 할 때 편지 이름에 대한 팝업이 숨겨져서 제대로 표시되지 않습니다. NPR-16353
* 문자를 편집하는 동안 추가된 라인 공백은 미리보기 창에 반영되지 않습니다. 텍스트 조각에 있는 목록의 경우 PDF 출력에 올바른 간격이 표시되지 않습니다. NPR-16267
* Internet Explorer 브라우저를 사용하여 텍스트 문서 조각에서 작업하는 동안 커서가 텍스트 들여쓰기를 허용하지 않으므로 텍스트에 들여쓰기를 제공하려고 시도해도 실패합니다. NPR-16128
* 기존 텍스트 문서 조각에 데이터 사전을 추가하거나 수정하는 데에는 많은 시간이 걸리고 사용자에게 항상 알림이 전송되지 않습니다. NPR-16102
* Internet Explorer 브라우저를 사용하여 스크롤 가능한 내용이 있는 문자를 미리 보는 동안 브라우저 스크롤바가 문자의 스크롤바와 겹치게 되며 오른쪽의 조각에 대해 전체 내용을 볼 수 없습니다. NPR-16068
* Google Chrome 브라우저를 사용하여 텍스트 문서 조각을 만들거나 편집하는 동안 색상 선택 드롭다운이 자동으로 표시되며 제거할 수 없습니다. 조각을 편집하려면 목록을 데이터 엔트리의 유형으로 선택해야 합니다. NPR-16067
* Letterinstance API를 사용하는 동안 `import com.adobe.icc.services.api.LetterInstanceService` 메서드가 작동하지 않습니다. NPR-16008
* Asset Composer 구성에서 날짜 표시 형식을 `locale=en_US; dateFormat=MMM dd,yyyy;`로 변경하면 제대로 작동하지 않고 날짜 형식이 정크 문자로 표시됩니다. NPR-16007
* 편지의 데이터 링크 유형은 다시 작성하는 동안 이전에 다르게 설정되었더라도 &#39;사용자&#39;로 표시됩니다. NPR-16619

**Forms 포털**

* 초안 및 제출 구성 요소에 대한 업그레이드 시나리오는 데이터베이스 샘플 구현 시 작동하지 않습니다. NPR: 16752

**BCF(Barcoded Forms Service)**

* BCF(Barcoded Forms Service)의 정적 코드 분석에서 문제를 보고합니다. NPR-13855

#### Forms JEE 설치 관리자  {#forms-jee-installer-17}

**프로세스 관리 - HTML 작업 공간**

* file://, &quot;http://&quot;, 및 ftp:// 등의 프로토콜을 통해 권한 없는 액세스로부터 양식 미리 채우기 서비스를 보호합니다. 자세한 내용은 [구성 관리자를 사용하여 미리 채우기 서비스 구성하기](https://helpx.adobe.com/aem-forms/6-2/prepopulate-adaptive-form-fields.html#main-pars_header_944235754)를 참조하십시오. NPR-15434

**사용자 관리 **

* SAML 로그인 화면에서 AEM 6.2 서버의 부적절한 버전(6.1.0)을 표시합니다. NPR-13825
* AEM Forms가 Single Sign On(Kerberos) 인증에 구성된 경우, 로그인 시도 중 사용자 인증이 실패하면 오류 코드 &#39;404&#39;가 반환됩니다. 사용자가 페이지를 새로 고친 후에만 로그인 사이트로 리디렉션됩니다. NPR-15015

#### Forms 디자이너 {#forms-designer-1}

* 사전 맞춤법 검사에서 양식 로케일을 프랑스어(캐나다)로 변경해도 AEM Forms Designer에서 작동하지 않습니다.\
   NPR-15896

### CFP3에 포함된 기능 팩 {#feature-packs-included-in-cfp-2}

**Forms 추가 기능 패키지**

* 서신 관리에서 에셋을 삭제하는 경우 error.log 파일에 경고 메시지가 기록되어야 합니다. NPR-13225
* 편지 제목이나 레이블만 검색하는 대신 텍스트 조각 콘텐츠에서 텍스트를 검색할 수 있도록 서신 관리에서 문자를 미리 보는 동안 검색 기능을 강화합니다. NPR-16103

### CFP3에 포함된 OSGi 번들 {#osgi-bundles-included-in-cfp-5}

AEM 6.2 SP1과 CFP3 간에 업데이트된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/osgi_bundle_list_for_aem-6.2sp1-cfp3.txt)
누적 수정 팩 2의 주요 특징:

* Sling 프레임워크 및 작업을 비롯한 AEM 플랫폼의 안정성 수정 및 성능 향상
* 에셋의 액세스, 이동, 검색, 업로드 및 게시에 대한 몇 가지 수정 사항으로 에셋 관리 개선
* 콘텐츠 조각, 앵커 플러그인, 슬라이드 쇼 및 Context Hub 구성 요소의 수정 사항이 있는 사이트 제작 및 관리 개선
* 텍스트 편집기, Omnisearch 및 변형 작성 프로세스를 비롯한 Touch UI의 몇 가지 수정 사항
* 향상된 번역 워크플로, Azure 포털용 새 번역 API를 사용하기 위한 Microsoft 커넥터 개선
* 프로젝트 및 캠페인의 수정 사항
* 적응형 양식, 서신 관리 및 양식 포털 기능 수정을 통해 작성 및 관리 개선
* Forms JEE 코어, XTG 및 HTML 작업 공간 구성 요소의 수정 사항

### 플랫폼 {#platform-14}

* Sling 프레임워크를 직접 참조하는 페이지가 편집되면 `SlingPostProcessor`가 트리거됩니다. NPR-15754: CQ-104153용 핫픽스

* 페이지 구성 요소로 이동하는 동안 `tagBasePath` 속성이 있는 태그의 값은 클래식 UI 대화 상자에서 가져오지 않습니다. NPR-15543: CQ-4199950용 핫픽스

* Sling 작업을 수행하는 동안 &#39;chunk_n_n-1&#39; 이라는 청크가 있으면 `SlingFileUpload handler.getLastChunk`에서 빈 청크가 있는 무한 루프가 발생합니다. NPR-15455: SLING-5701용 핫픽스

* 인터페이스가 또 다른 인터페이스를 확장하면 수퍼 인터페이스에서 주입 가능한 메서드가 올바르게 주입되지 않습니다. NPR-15202: SLING- 5710용 핫픽스
* `com.adobe.granite.infocollector.impl.FilesTraversal` 함수 호출을 사용할 때는 잠재적 null 포인터 예외가 발생하지 않습니다. NPR-15169, CQ-4197640용 핫픽스
* 일부 보조 노드에 대해 워크플로 상태가 일관되지 않으며 해당 노드에 대한 관찰 이벤트를 전달하는 동안 오류가 표시됩니다. NPR-15701: GRANITE-13786용 핫픽스
* 사용자가 CRXDE(예: /content/dam/)에서 노드를 선택한 다음 &#39;액세스 제어&#39; 탭을 선택하면 액세스 제어 목록이 있는지 확인하고 일부 요소를 드래그하여 놓으면 선택한 항목 이외의 요소가 이동됩니다. NPR-15696, GRANITE-16300용 핫픽스
* 가장을 시도할 때 드롭다운 목록에서 사용자를 선택하면 전체 사용자 팝업이 사라집니다. NPR-15774: CQ-4201738/GRANITE-11895용 핫픽스
* Omnisearch에서는 자동 작성된 제안을 포함하는 태그로 검색할 수 없습니다. NPR-15088: GRANITE-14426용 핫픽스.\
   참고: 이 수정 사항을 적용하려면 Oak CFP 1.4.11 이상이 필요합니다.

### 모바일 AEM 작성자 {#mobile-aem-author}

* AEM Mobile 및 ContentSync 패키지를 하이브리드 애플리케이션과 함께 사용하는 경우, AEM은 애플리케이션에서 요청한 패키지가 아닌 가장 오래된 패키지로 애플리케이션에서 수행하는 가져오기 요청(타임스탬프 포함)에 응답합니다. NPR-15749: CQ-104153용 핫픽스

### 사이트 {#sites-17}

* 사용자가 워크플로를 활성화한 후 페이지를 수정하는 경우, WCM 코어의 워크플로 받은 편지함에 대한 수정 상태가 변경되지 않습니다. NPR-15684: CQ-4196974용 핫픽스
* Touch UI용 리치 텍스트 편집기의 앵커 플러그인은 사용자가 앵커 아이콘을 클릭하고 이름을 추가하면 비호환 HTML5를 생성합니다. 앵커 요소의 HTML5 태그에 &#39;name&#39; 속성 대신 &#39;id&#39; 속성을 추가해야 합니다. NPR-15650: CQ-89782용 핫픽스
* 필드가 많은 메타데이터 스키마를 만들어 콘텐츠 조각 메타데이터에 적용하면 콘텐츠 조각 메타데이터 화면에서 스크롤바가 만들어지지 않아 필드를 편집할 수 없습니다. NPR-15478: CQ-4202622용 핫픽스
* `TagInput` 필드 구성 요소를 편집해도 대화 상자 필드에 대해 이전에 구성된 값이 표시되지 않습니다. NPR-15464: CQ-4200360용 핫픽스

* 콘텐츠 조각 편집기 UI에서 콘텐츠 조각의 다양한 변형을 만들 경우 사이드 패널에는 모든 변형을 탐색하는 스크롤바가 표시되지 않습니다. NPR-15445: CQ-4199444용 핫픽스
* 사용자가 직접 그룹에서 제거되면 상속된 그룹에 추가됩니다. NPR-15400: CQ-98758용 핫픽스
* WCM 작성: Touch UI 작성자는 이름에 쉼표가 있는 페이지의 편집을 허용하지 않습니다. NPR-15396: CQ-4199723용 핫픽스
* 작성을 위해 Touch UI를 사용하는 동안 `Granite.author.editableHelper.doSelectParent` 함수가 인수를 잘못된 순서로 전달하면 JavaScript 오류가 발생합니다. NPR-15349: CQ-4198594용 핫픽스
* ContextHub 세그먼트는 옵트아웃 쿠키가 있는 경우에도 경험을 표시합니다. NPR-15293: CQ-4198024용 핫픽스
* 클래식 UI의 슬라이드쇼 구성 요소는 슬라이드를 만들거나 이미지를 드래그하여 놓는 방식으로 새 슬라이드를 만들 수 없습니다. NPR-15281: CQ-4194164용 핫픽스
* 사용 권한에 관계없이 사이트 Admin Console에서 페이지 만들기, 사이트 만들기, 라이브 카피 만들기, 시작 만들기 및 카탈로그 만들기 메뉴 항목 등의 “만들기” 옵션이 표시됩니다. NPR-15278: CQ-94436용 핫픽스
* AEM 6.2 서비스 팩 1을 설치한 후, 페이지 시작에 대해 &#39;하위 페이지 포함&#39; 슬라이더가 작동하지 않습니다. NPR-15230: CQ-4198449용 핫픽스
* 블록에서 버전을 가져오고 처리하고 XPath 쿼리에 지정된 경로를 사용할 수 있도록 버전 삭제 기능의 개선을 요청합니다. NPR-15186: CQ-109205용 핫픽스
* Sites 구성 요소의 페이지 속성 썸네일 탭에 지우기 버튼이 없습니다. NPR-15143, CQ-4196997용 핫픽스
* 라이브 카피를 사용하는 사이트의 경우, 사이트 Admin Console의 열 창에서 “라이브 카피” 확인란을 선택하면 라이브 카피 상태가 올바로 표시되지 않고 HTML 마크업만 표시됩니다. NPR-15108: CQ-97086용 핫픽스
* 콘텐츠 조각을 편집할 때 게시물의 응답을 가져오기 전에 편집을 위해 완료(&#39;√&#39;)를 클릭하면 편집된 콘텐츠가 제대로 저장되지 않습니다. NPR-15014: CQ-4194095용 핫픽스
* 타임워프 모드 중에 편집 페이지를 닫고 사이트 관리자에서 다시 열려고 하면 페이지를 다시 여는 대신 상태가 &#39;500&#39;인 오류가 발생합니다. NPR-14965: CQ-109647용 핫픽스:
* DAM(Digital Asset Manager) UI에서 사용자 선택기의 승인 가능 대상 찾기 검색을 수행하면 &#39;메모리 부족&#39; 예외가 발생합니다. NPR: 15307: CQ-98542용 핫픽스

### 자산 {#assets-17}

* Omnisearch에서 에셋을 검색한 후, 에셋을 선택하고 &#39;속성 보기&#39;를 클릭하여 속성을 편집한 다음 &#39;저장&#39; 버튼을 사용하면 사용자가 빈 페이지로 리디렉션됩니다. NPR-15900: CQ-4202372용 핫픽스
* Assets 사용자 인터페이스가 이벤트에 응답하지 않습니다. 에셋을 선택하고 &#39;게시&#39; 또는 &#39;렌디션&#39;을 클릭해도 어떤 작업도 수행되지 않습니다. NPR-15828: CQ-4202247용 핫픽스
* 카드 보기에서 에셋을 게시할 때 페이지를 새로 고치지 않으면 게시된 상태를 반영하도록 카드가 업데이트되지 않습니다. NPR-15826: CQ-102732용 핫픽스
* Assets 핫픽스를 포함하는 누적 핫픽스. NPR-15225
* 앰퍼샌드(&#39;&amp;&#39;) 문자가 에셋 폴더 이름에 포함된 경우, 에셋으로 이동할 때 폴더 이름이 올바르게 표시되지 않습니다. NPR-15775: CQ-4201735용 핫픽스
* 에셋 파일 이름에 앰퍼샌드(&#39;&amp;&#39;) 문자를 사용하면 해당 속성에 액세스할 때 문제가 발생합니다. NPR-15770: CQ-4201737용 핫픽스
* Assets를 탐색하고 &#39;열 보기&#39; 표시 모드를 사용하는 동안, 사용자가 에셋을 선택하고 클릭한 후 페이지를 새로 고치면, 새로 고친 콘텐츠 대신 에셋 세부 사항이 표시됩니다. NPR-15768: CQ-4201727용 핫픽스
* PDS 처리는 PDF 서비스를 위한 라이브러리 힙과 함께 CPU 사용률을 100%로 높입니다. NPR-15606, GRANITE-12929용 핫픽스
* Firefox 브라우저를 사용하여 &#39;내 링크 공유&#39; UI에 액세스하면 공유 항목이 표시되지 않고 화면을 사용할 수 없습니다. NPR-15539: CQ-4200992용 핫픽스
* Digital Asset Manager를 사용하는 동안, 페이지가 이미지 집합에 연결된 경우 이미지를 새 폴더로 이동하면 페이지 연결이 끊기고 연결된 페이지에 일부 이미지가 누락됩니다. NPR-15538: CQ-111479용 핫픽스
* Dam 뷰어 구성 요소에서 &#39;nosamplecontent&#39; 실행 모드를 사용하면 Dynamic Media에 오류가 발생합니다. NPR-15449: CQ-4195425용 핫픽스
* 비디오 프로필을 만드는 동안 고품질 및 중간 품질의 비디오 인코딩 사전 설정을 모두 선택하면 변경 내용이 저장되지 않습니다. NPR-15447: CQ-4195482용 핫픽스
* 서버 오류 응답으로 인해 Brand Portal에 에셋을 업로드하지 못하는 경우에도 Brand Portal UI에서 상태가 &#39;게시됨&#39;으로 업데이트되므로 누락된 파일을 추적하기가 어렵습니다. NPR-15442: CQ-4197968용 핫픽스
* 에셋 폴더를 Brand Portal에 게시하면 게시 시간이 1시간 이상 걸리며 일부 파일을 게시할 수 없습니다. NPR-15441: CQ-4199493용 핫픽스
* 열 보기에서 에셋 파인더 콘솔을 사용할 때, 재시도는 성공해도 폴더 만들기에 한 번 실패합니다. NPR-15370: CQ-4199448용 핫픽스
* DAM UI에서 선택한 에셋 또는 폴더의 이름에 쉼표가 있는 경우 참조 탭을 사용할 수 없으며 &quot;여러 항목을 선택할 때 참조 목록을 사용할 수 없습니다.&quot;라는 메시지가 표시됩니다. NPR-15362: CQ-4199721용 핫픽스
* 폴더 아래에 에셋이 게시되었어도 폴더를 Brand Portal에 게시해서 폴더의 게시된 상태가 변경되지 않습니다. NPR-15292: CQ-4197667용 핫픽스
* Touch UI에서 Assets 콘솔로 이동하는 동안 특정 에셋을 활성화할 때 표시되는 예외 사항입니다. NPR-15217: CQ-108779용 핫픽스
* 프록시 서버를 통해 연결할 때 Youtube에 비디오를 게시합니다. NPR-15109: CQ-110332용 핫픽스
* 점 또는 마침표(.)가 포함된 이름의 에셋 사용하기 data-sly-resource에서는 동일한 에셋으로 확인되지 않으며 출력 경로가 점에서 끝납니다. NPR-15069: CQ-4195914용 핫픽스
* AEM 6.2를 서비스 팩 1로 업그레이드한 후 Scene7에 에셋을 동기화할 수 없습니다. dam:Scene7FileStatus 속성은 게시된 에셋에 대해서도 &#39; `UploadFailed`&#39; 상태를 표시합니다. NPR-15269: CQ-4197708용 핫픽스

### 사용자 인터페이스 {#user-interface-5}

* **[!UICONTROL Touch UI]**&#x200B;에서 인터넷 Chrome 브라우저 버전 56.0.2924.87을 사용하는 동안 type=&#39;datetime&#39;이 없는 날짜 필드에 저장된 날짜가 표시되지 않습니다. NPR-15383: GRANITE-16481용 핫픽스
* **[!UICONTROL Touch UI]**&#x200B;의 리치 텍스트 편집기는 렌더링하는 동안 HTML 테이블에서 스레드 및 캡션 요소를 제거합니다. NPR-15267: CRTE-41용 핫픽스
* autostart가 true이거나 `uploadFile()`을 수동으로 호출한 경우 `FileUpload Validator`에서 사례를 처리하지 않으며 이러한 사례에 대해 잘못된 유효성 검사 보고서를 생성합니다. NPR-15295: GRANITE-13499용 핫픽스

* Omnissearch는 위치 구성이 */libs/granite/omnisearch/content/metadata/* 아래에 있다고 간주하므로 /apps를 사용하는 고객이 열 데이터 소스를 추가할 수 없습니다. NPR-13188: GRANITE-16479용 핫픽스
* **[!UICONTROL Touch UI]**&#x200B;를 사용할 때 제품 변형이 제품과 동일한 수준에서 만들어지지 않습니다. 변형 작성 프로세스의 상태에 대해 사용자에게 알려주지 않습니다. NPR-15345: CQ-4198948용 핫픽스

**Scene7**

* Scene7 워크플로를 실행하면 열려 있는 파일이 닫히지 않습니다. 공유 풀링 구성으로 단일 HttpClient 인스턴스를 유지 관리하고 재사용할 수 있도록 하는 AEM-S7 서비스 개선 요청입니다. NPR-15357: CQ-109958용 핫픽스

### 번역 {#translation-9}

* 번역 프로젝트를 사용할 때, 영어 마스터에서 언어 사본을 업데이트하면 페이지 이름이 설정된 패턴을 따르는 경우, 이름과 소스 루트가 동일한 11개의 개별 시작을 생성하지만 시작 루트는 약간 다릅니다. NPR-15605: CQ-4200699용 핫픽스
* 언어 루트에서 이름에 하이픈 및 대시가 있는 경우 페이지에 대한 번역 프로젝트가 생성되지 않습니다. NPR-15171: CQ-96286용 핫픽스
* Microsoft Translator API를 사용할 수 있도록 Microsoft 커넥터를 업데이트하는 요청입니다. 이 API는 Microsoft에서 Azure 포털에서 사용할 수 있도록 지원합니다. NPR-15320: CQ-101010용 핫픽스

### 프로젝트 {#projects-4}

* 저장소에 20개 이상의 비활성 프로젝트가 있지만 프로젝트 화면에 20개의 비활성 프로젝트만 표시됩니다. NPR-15656: CQ-4200903용 핫픽스

### 캠페인 {#campaign-1}

* Campaign - 타깃팅 및 MAC - 테스트, Target 통합 구성 요소를 사용하는 동안 활동 게시를 취소하면 마스터 UI에서 활동 상태가 업데이트되지 않습니다. NPR-15401: CQ-4199839용 핫픽스
* AEM Commerce에서 제품을 이동하는 동안, 제품 이동 마법사에서 제품 이름, 제목, 참조된 페이지, 작성자 만들기 및 만든 날짜에 대해 미리 채워진 값을 누락합니다. NPR-15228: CQ-98617용 핫픽스

### 보안 {#security-4}

* CSRF 토큰 매개 변수가 GET 메서드를 사용하여 양식에 추가되었습니다. NPR-15229

### 양식 {#forms-18}

#### Forms 추가 기능 패키지 {#forms-add-on-package-18}

`**Adaptive Forms**`

* 입력 XML로 적응형 양식을 미리 채울 때 xml의 빈 값에 의해 기본값이 재정의됩니다. NPR-15721
* XML 스키마 기반 적응형 양식에 `afData/afBoundData` 래퍼가 포함되어 있지 않더라도, `afData/afBoundData` 래퍼가 제출된 XML에 표시됩니다. NPR-15541

* 아코디언 막대의 제목은 &#39;a&#39; 태그 대신 HTML &#39;h2&#39; 제목을 편집할 수 있어야 합니다. NPR-15475
* 화면 읽기 프로그램 사용자는 양식 패널의 아코디언 레이아웃에 액세스할 수 없습니다. JAWS 또는 NVDA와 같은 화면 읽기 프로그램 소프트웨어를 사용하여 키보드만으로 아코디언 탭으로 이동할 수 없습니다. NPR-15474

`**Correspondence Management**`

* 문서 조각에 대한 참조를 저장, 삭제 및 설정하는 데에는 상당한 시간이 소요됩니다. NPR-15939
* CCR UI에서 여러 개의 헤더 나누기가 포함된 텍스트의 에셋 관리에서 탭 정렬 집합입니다. NPR-15818
* Google Chrome에서 Tab 키를 사용하여 만든 맞춤 콘텐츠가 텍스트에 포함되어 있지만 텍스트 모듈의 썸네일은 정렬된 콘텐츠를 표시하지 않습니다. NPR-15819

`**Forms Portal**`

* XDP Forms에서는 미리 채우기 서비스가 작동하지 않습니다. NPR-15466
* 적응형 양식 초안 및 데이터베이스에 제출 문서를 저장할 때 데이터베이스 연결이 실패하면(예: 오랫동안 사용하지 않은 경우) 적응형 양식의 상태가 손상될 수 있습니다. NPR-15297

#### Forms JEE 설치 관리자  {#forms-jee-installer-18}

`**Core**`

* 최신 버전의 Java 1.8.0_121-b13으로 업그레이드한 후 AEM Forms에서 관리 사용자 인터페이스에 액세스할 수 없습니다. NPR-15330

`**XTG**`

* 출력 서비스를 사용하여 특정 양식을 데이터 xml과 병합하는 동안 동일한 작업에 대해 ES4 SP1 서버에서 걸리는 시간과 비교하여 응답 시간은 20배입니다. NPR-15283

#### AEM Forms 앱 {#aem-forms-app-1}

* 저장하지 않은 작업을 복구할 때 저장하지 않은 작업 복구에 표시되는 메시지를 명확하게 작성해야 사용자 오류를 줄일 수 있습니다. NPR-15377
* AEM Forms 앱은 사용자 정의 템플릿에서 만든 양식을 렌더링하지 않습니다. NPR-15892
* 사용자가 AEM Forms 앱에 로그인할 수 없습니다. NPR-15891

AEM 6.2 SP2-CFP1의 주요 특징:

* 사이트의 복제 기능 간소화:

   * 다양한 롤아웃, LiveCopy 및 잘못된 쓰기 문제에 대한 수정 사항

* 다음 작업 중 Touch UI 응답성을 개선합니다.

   * 에셋 검색
   * 크기 기반 정렬

* 스마트 컬렉션의 Tag management 향상
* 폴더에서의 CRUD 작업 중 더욱 긴밀해진 액세스 제어

### 플랫폼 {#previous}

* 복제 에이전트를 시작하는 동안 `ReplicationQueue#forceRetry` API 호출 제거를 요청합니다. 이러한 호출은 특히 복제 에이전트가 많을 때 인스턴스를 매우 느리게 만들기 때문입니다. NPR-14032: GRANITE-13095용 핫픽스
* 값 배열을 저장할 수 있는 필드를 지원하기 위해 `DurboImportConfigurationProviderService` OSGi 구성을 요청합니다. NPR-14570: CQ-108684용 핫픽스
* AEM 6.2로 마이그레이션한 후 페이지에서 Sightly 구성 요소를 사용하면 페이지의 속성 대화 상자가 작동하지 않습니다. NPR-14328: CQ-108355용 핫픽스
* 이전에 예약한 작업의 예약을 취소해도 */var/events/scheduled-jobs* 아래에서 해당하는 노드가 제거되지 않습니다. NPR-14253: SLING-5666용 핫픽스
* 관리자가 삭제된 사용자로 가장하려고 하면 사용자 인터페이스를 새로 고치지 못합니다. NPR-14247: CQ-107446용 핫픽스
* Sightly 구성 요소에서 잘못된 인코딩을 발생하게 만드는 XSS 보호 검사. NPR-14004: CQ-93821용 핫픽스
* 여러 문제를 해결하기 위해 Jackrabbit Filerabbit을 3.1.30으로 업그레이드하도록 요청합니다. NPR-13454
* Sling 배포 시 작성자에서 게시로 배포 패키지를 동기화할 때 캐시 오류가 발생합니다. NPR-13034: GRANITE-13970용 핫픽스

### 사이트 {#sites-18}

* VersionManagerImpl이 버전 내역에서 잘못된 버전을 삭제하는 문제 NPR-14372
* WCM Sightly Foundation parsys 구성 요소는 구성 요소 선언 태그 이름 `cq:htmlTag / cq:tagName`을 무시합니다. NPR-14225
* Touch UI에서 Sightly Parsys를 사용하여 JavaScript를 통해 삽입된 구성 요소를 렌더링하면 페이지를 새로 고친 후 사용자 정의 데코레이션이 무시됩니다. NPR-14122
* 링크와 같은 여러 개의 서식이 있는 텍스트 필드를 만들 때 Target 드롭다운 목록이 Touch UI 대화 상자에서 작동하지 않습니다. NPR-13911
* 대화 상자(Touch UI)에서 여러 RTE(Rich Text Editor) 속성이 있는 텍스트 필드를 편집할 때 포커스가 임의로 특정 RTE 속성으로 이동합니다. NPR-13703
* 기본적으로 비디오 구성 요소는 비디오 썸네일을 렌더링하지 않습니다. NPR-14976
* 템플릿 편집기의 라이브 사용량 탭에서 정보가 느리게 로드됩니다. NPR-14880: CQ-83417용 핫픽스
* AEM 6.2 인스턴스에 Hotfix-10936을 설치하면 iparsys 구성 요소가 비활성화됩니다. NPR-14330: CQ-106982용 핫픽스
* AEM 6.1 SP1로 마이그레이션한 후 다중 롤아웃 구성 요소 문제와 라이브 카피 문제. NPR-15256
* 페이지 롤아웃 작업은 여러 개의 롤아웃 구성에서도 첫 번째 수준 이상의 하위 항목을 만들지 못합니다. NPR-15055
* 편집기에서 PageProperties 대화 상자를 제출하면 LiveCopy 탭의 변경되지 않은 데이터가 다시 작성됩니다. NPR-14693
* 편집기에서 PageProperties 대화 상자를 제출하면 MSM 포스트 프로세서는 `msm:writeLiveCopyConfig` 매개 변수 대신 요청에서 일부 매개 변수를 기록합니다. NPR-14434
* 롤아웃 구성 요소, 라이브 카피 및 MSM의 기타 측면과 관련된 여러 문제입니다. NPR-12235

### 자산 {#assets-18}

* 압축 해제 워크플로에서 이미지 파일 이름에 특수 문자가 있는 이미지를 처리할 수 없습니다. NPR-15227: CQ-103887용 핫픽스
* 조건 표현식이 있는 반복이 포함된 에셋이 제대로 표시되지 않습니다. 사용자가 `*CDN3835RLCEN*` 편지 템플릿을 미리 볼 때 본문 대상 영역에 있는 에셋이 표시되지 않습니다. 선택적 에셋인 `*VIPReassement*` 에셋을 미리 선택하지 않은 경우, 사전에 선택한 다른 에셋이 편지에 표시됩니다. NPR-14844

* 스마트 컬렉션을 만드는 동안 스마트 컬렉션을 저장할 때 스타일 태그가 유지되지 않습니다. NPR-15081: CQ-4195494용 핫픽스
* 여러 사용자가 동시에 검색하는 동안 Touch UI에서 에셋 검색 쿼리가 느리게 실행됩니다. NPR-15019: CQ-4195405용 핫픽스
* `Long[]` 유형의 속성에 대해 추출된 메타데이터는 원래 에셋이 다른 위치로 다시 업로드되면 `String[]` 유형으로 변환됩니다. NPR-15016: CQ-4195005용 핫픽스

* 저장된 검색 또는 스마트 컬렉션을 삭제할 수 없습니다. NPR-14924: CQ-108494용 핫픽스
* 기본 메타데이터 스키마의 드롭다운 필드에서 TypeHint에 부울 값을 사용하는 동안 일괄(추가 모드)로 에셋의 메타데이터를 편집하면 오류가 발생합니다. NPR-14529: CQ-106876용 핫픽스
* 복제 권한이 없는 사용자는 에셋 폴더를 삭제할 수 없습니다. NPR-14321: CQ-88271용 핫픽스
* 채널 편집기에서 비디오에 대한 비디오 프로필을 편집하려고 하면 디자인 대화 상자가 열리지 않고 오류 로그에 Null 포인터 예외가 발생합니다. NPR-14144: CQ-81101용 핫픽스
* 에셋의 속성 페이지에 표시되는 시스템에서 생성한 &#39;Created&#39; 타임스탬프 속성이 잘못되었습니다. NPR-13992: CQ-95029용 핫픽스
* AEM Assets에서 읽기 액세스 권한이 없는 사용자에 대해 중복 에셋을 탐지할 수 있도록 요청. NPR-13851: CQ-102281용 핫픽스
* 속성 페이지에서 에셋의 메타데이터를 일괄적으로 편집할 수 없습니다. NPR-13721: CQ-100703용 핫픽스
* 중복 에셋이 업로드되면 클래식 UI에서 잘못된 오류 메시지가 표시됩니다. 업로드 실패 이유가 오류 메시지에 표시되지 않습니다. NPR-13691: CQ-99272용 핫픽스
* AEM Assets는 폴더에 많은 에셋이 포함되어 있는 경우 목록 보기에서 한 번에 50개 이상의 에셋을 크기 기준으로 정렬할 수 없습니다. CQ-100588
* 에셋/폴더 URI가 너무 긴 경우 여러 에셋을 선택하면 응답 코드 - 414(Request-URI Too Long) 오류가 발생합니다. NPR-13516: CQ-76076용 핫픽스
* 사용자가 열 구성 대화 상자에서 모든 선택 사항을 선택하면 에셋 보고서 페이지가 응답하지 않습니다. NPR-13187: CQ-95589용 핫픽스
* Safari 및 Internet Explorer에서 태그 선택기의 예기치 않은 동작입니다. NPR-13134
* 에셋 관리 검색 레일에서 저장된 검색을 편집하면 중첩된 스마트 선택 항목으로 저장할 수 있으므로 환경 안정성 문제가 발생합니다. NPR-13119: CQ-99460용 핫픽스
* 파일(또는 폴더)을 이동한 다음 이름을 바꾸면 &#39;cq:name&#39; 메타데이터에서 새 파일 이름(폴더 이름)을 반영하지 않습니다. NPR-13036: CQ-99141용 핫픽스
* 이름에 특수 문자가 포함된 에셋은 이메일을 통해 공유되는 다운로드 링크에서 다운로드할 수 없습니다. NPR-12872: CQ-95795용 핫픽스
* 많은 에셋이 있을 때 생성되는 기본 에셋 보고서 검색에서는 색인 및 CPU 사용 스파이크에 도달하지 않는 대량 순회를 만듭니다. NPR-12811: CQ-84409용 핫픽스
* 서로 다른 네트워크에서 액세스하는 AMS AEM Assets 작성자 인스턴스의 사용자는 폴더에 대한 삭제 권한 없이 청크 업로드를 사용하여 에셋을 업로드할 수 없습니다. NPR-12768: CQ-82715용 핫픽스
* 태그 기반 검색에서 에셋 검색 레일을 사용하여 에셋을 검색할 때 자동 완성 기능이 루트 경로로 한정되지 않으며 모든 네임스페이스의 태그를 표시합니다. NPR-12666
* StaticRenditions 구성 요소는 null 포인터 예외를 발생시킵니다. NPR-12665
* MissingMetadataNotificationJob을 비활성화하도록 요청하면 배지 알림 UI가 런타임 예외 &quot;입력 내용을 스캔할 수 없습니다.&quot;로 페이지가 중단됩니다. NPR-12500: CQ-93573용 핫픽스
* 태그 필드에 대한 &#39;편집 비활성화&#39; 옵션이 TouchUI의 에셋 속성 페이지에서 작동하지 않습니다. NPR-12429: CQ-88835용 핫픽스
* Companion App SMB 구현을 위한 AEM Assets 6.2의 API 수정 사항. NPR-11099
* Jquery 업데이트 이후 사용자는 콘텐츠 조각의 콘텐츠 연결 패널에서 에셋 컬렉션을 선택하고 선택을 확인할 수 없습니다. NPR-14847: CQ-4194209 지원
* 클라이언트 측에서 무한 정렬이 호출되더라도 현재 UI에 표시된 문서/배너/컬렉션만 정렬됩니다. NPR-14493: CQ-109926용 핫픽스
* AEM MOBILE-on-demand 서비스를 위한 omnisearch 기능 구현을 요청합니다. 모든 문서, 컬렉션 또는 배너에 대한 키워드 검색에서 일치하는 항목을 반환하지 않습니다. NPR-14093: CQ-101394용 핫픽스
* 대화 상자에서 Coral-select 구성 요소(*granite/ui/components/coral/foundation/form/select*)를 사용하는 경우, 선택한 값에 단일 항목이 포함되어 있으면 Internet Explorer(IE11 또는 Edge 브라우저)에서 값 초기화가 제대로 작동하지 않습니다. NPR-13395: CQ-101013용 핫픽스

### 프로젝트 {#projects-5}

* 번역 방법으로 &#39;human&#39;을 번역 공급자로 &#39;none&#39;을 사용하여 만든 번역 프로젝트를 내보낼 때 GUID 매핑 파일이 없으므로 translation_export_summary.xml 파일이 생성되지 않습니다. NPR-13137: CQ-91976용 핫픽스
* AEM 프로젝트에서 기한 속성이 설정된 프로젝트를 만들 때 서버 및 클라이언트 간의 시간대 차이로 인해 날짜 전환 시 시간을 잘못 설정합니다. NPR-13003: CQ-98288용 핫픽스
* 번역 프로젝트가 업데이트되면 번역 작업에서 &#39;사이트에 표시&#39; 옵션이 누락됩니다. NPR-12966: CQ-93740용 핫픽스
* 내보낸 사이트 페이지에 대한 번역 프로젝트를 만들 때 미리보기에서 올바르게 렌더링되지 않습니다. NPR-12964: CQ-84627용 핫픽스

### 워크플로우 {#workflow-3}

* 워크플로 콘솔의 보관 탭에 있는 페이로드 링크는 클릭 시 응답 코드 &#39;404&#39;가 있는 오류를 반환합니다. NPR-14993: CQ-4194977용 핫픽스
* AEM 기본 워크플로를 사용하는 경우 CQ 발송은 단일 구성원의 이메일 주소를 누락한 그룹에 이메일 알림을 보내지 못합니다. NPR-14804: CQ-91499용 핫픽스 요청
* Touch UI의 받은 편지함 및 알림 배지에 대한 성능이 개선되었습니다. NPR-14145: CQ-101125용 핫픽스
* 워크플로를 시작하는 동안 워크플로 받은 편지함 콘솔에서 페이로드를 미리 볼 수 없습니다. NPR-13226: CQ-100275용 핫픽스
* SAML 인증 핸들러를 사용하여 구성된 &#39;saml_request_path&#39; 쿠키는 추가 &#39;?&#39; 문자로 설정된 쿠키를 표시합니다. 또한 SAML 응답이 AEM에 다시 게시되면 AEM &#39;saml_request_path&#39; 쿠키에서 이미 인코딩된 문자로 인해 잘못된 값을 반환합니다. NPR-13517: GRANITE-11722 및 GRANITE-14414에 대한 사전 예방 핫픽스

### 솔루션 통합 {#solution-integration}

* AEM 6.2를 Search &amp; Promote과 통합한 후 사용자가 배너를 반환하는 용어를 검색하면 검색 기능이 응답하지 않습니다. NPR-14549: CQ-109631용 CFP

### 다이내믹 미디어 {#dynamic-media}

* 복제 중 AEM 활성화가 아카이브 작업으로 기록될 때 생성 및 취소된 수많은 AEM-Scene7 Sling 작업. NPR-12835: CQ-86115용 핫픽스

### 보안 {#security-5}

* WCMDebug 필터의 입력 유효성 검사 문제를 해결하기 위한 요청입니다. NPR-12444: CQ-94890용 핫픽스 요청
* 시작 만들기 마법사를 사용하는 동안 XSS 동작을 수정하기 위한 사전 요청.\
   NPR-13062: CQ-99577용 핫픽스 요청

#### Forms 추가 기능 패키지 {#forms-add-on-package-19}

`Adaptive Forms`

* 적응형 양식을 사용하여 반복 가능한 패널을 만들 때 런타임 시 패널 제목을 업데이트할 수 없습니다. NPR-15325
* 저장 또는 제출 시 라디오 버튼의 기본값이 설정되고 기본값이 아닌 값이 선택되어 있으면 이 값이 사전 채우기 중 표시되지 않습니다. NPR-15304
* Google Chrome은 드롭다운 목록을 동적으로 채우고 선택한 항목의 값을 제출하기 위한 옵션 이벤트 사용에 대한 잘못된 동작을 보여 줍니다. NPR-15198
* 적응형 양식을 사용하여 반복 가능한 패널을 만들 때 런타임 시 패널 제목을 업데이트할 수 없습니다. NPR-15181
* 적응형 양식에 편집 모드를 사용할 때 &#39;구성 요소의 핸들러가 잘못되었습니다.&#39; 및 &#39;guidelib가 정의되지 않음&#39;과 같은 JavaScript 오류가 발생합니다. NPR-15112
* 반복 패널 내의 지연 로드 조각이 예상대로 작동하지 않습니다. NPR-13916, NPR-14785

`Correspondence Management`

* `'Repeat with condition'` 표현식 세트가 있는 서신 관리 에셋이 제대로 표시되지 않습니다. NPR-14844
* 편지, 문서 조각 또는 기타 유형과 같은 서신 관리 에셋을 검색할 때, 다운로드 큐 아이콘이 도구 모음에서 누락됩니다. NPR-14745
* 목록 모듈을 만들 때, 에셋 관련 속성(예: 편집 가능, 필수)의 전환이 작동하지 않습니다. NPR-14689
* 데이터 사전을 선택하지 않고 조건 모듈이 만들어지는 경우 표현식 빌더 유틸리티의 데이터 요소 패널이 계속 로드됩니다. NPR-14688
* 편지 미리보기에서는 탭 공간을 사용하여 내용을 표 형식으로 정렬할 수 없습니다. NPR-14481
* 사용자 인터페이스에서 서신 관리 에셋을 일괄로 내보낼 때 AEM Forms 서버에서 불필요한 로그를 생성합니다. NPR-15226
* 편지를 미리 보면 좌우 정렬된 텍스트가 다른 글꼴로 표시됩니다. NPR-15468

`**Forms Portal**`

* Forms 포털에서 제출된 양식의 첨부 파일은 포털 제출 시 새 초안을 제출할 때 표시되지 않습니다. NPR-13515

`**Forms Manager**`

* *FormandDocuments* 디렉터리를 탐색할 때 사용자가 에셋을 복사하여 다른 폴더로 이동하는 경우 붙여넣기 버튼이 표시되지 않습니다. CQ-111327

#### Forms JEE 설치 관리자 {#forms-jee-installer-19}

`Rights Management`

* 사용자 로그인 관련 감사 이벤트가 잘못된 시간으로 기록됩니다. 감사 이벤트에 대한 올바른 시간을 추적할 수 없습니다. NPR-13107
* Adobe Acrobat Reader 및 Microsoft Office에서 확장된 인증으로 보호된 문서를 열지 못합니다. NPR-14482

`Process Management`

* HTML 작업 공간의 전달된 초안 작업이 초기 사용자에게 반환되면 초기 사용자의 큐에 작업이 나타나지 않습니다. NPR-15178

`Assembler Service`

* AEM Forms에서 두 개 이상의 서명을 사용하여 PDF/A-2b의 유효성을 검사하지 못했습니다. NPR-14101

`XTG`

* 프린터 바이패스 용지함을 사용하여 문서를 인쇄하는 동안 `GeneratePrintedOutput` 함수는 오른쪽 바이패스 용지함에서 종이를 가져올 수 없습니다. NPR-14079

#### Forms 디자이너 {#forms-designer-2}

* 사용자가 선택한 양식 로케일을 프랑스어(캐나다)로 사용하여 맞춤법 검사 유틸리티를 실행할 때 Forms Designer가 충돌합니다. NPR-13740
* 사용자가 양식 필드에 대해 이벤트 계산 또는 이벤트 유효성 검사를 선택하고 언어를 JavaScript로 변경한 다음 **[!UICONTROL 스크립트 편집기]** 창에 `this.`를 입력하면 Forms Designer가 충돌합니다. NPR-12974

### CFP1에 포함된 기능 팩 {#feature-packs-included-in-cfp-3}

`Mobile Forms`(Forms 추가 기능 패키지):

* XDP 파일에서 적응형 양식을 만들 때 액세스 가능성을 위한 탭 표시에서 설정된 패턴을 따르지 않습니다. NPR-12562

`Adaptive forms`(Forms 추가 기능 패키지):

* 적응형 양식에 대한 규칙 빌더는 역할 기반 액세스를 제공하지 않습니다. 작성자가 변경한 내용을 추적할 수 없습니다. NPR-12840

`Core` (Forms JEE 설치 관리자):

* Jboss+에 CORS(CoreCross Origin Resource Sharing) 기능을 서블릿 필터로 사용할 수 없습니다. NPR-13050

## 소프트웨어 배포를 통한 CFP용 지침 다운로드 {#download-instructions-for-cfp-via-package-share}

>[!NOTE]
>
>AEM Forms 고객의 경우 AEM 서비스 팩, 누적 서비스 팩 또는 기능 팩을 설치한 후 AEM Forms 추가 기능 패키지를 설치해야 합니다.

소프트웨어 배포에서 직접 CFP 패키지를 다운로드하거나 다음 단계를 수행할 수 있습니다.

1. [소프트웨어 배포](https://experience.adobe.com/downloads)를 엽니다. 소프트웨어 배포에 로그인하려면 Adobe ID가 필요합니다.
1. 헤더 메뉴에 제공된 **[!UICONTROL Adobe Experience Manager]**&#x200B;를 누릅니다.
1. 패키지 이름을 탭하고 **[!UICONTROL EULA 약관 동의]**&#x200B;를 선택한 후 **[!UICONTROL 다운로드]**&#x200B;를 탭합니다.

## CFP에 대한 설치 지침 {#installation-instructions-for-cfp}

이 섹션에서는 CFP를 설치하기 위한 요구 사항 및 단계를 안내합니다.

### 설치하기 전에 {#before-you-install}

>[!NOTE]
>
>Adobe에서 제공하는 선택적 기능 팩은 릴리스 버전 및 누적 수정 팩에 종속되어 있습니다. 기능 팩이 설치되어 있는 경우 [AEM 고객 지원팀](https://helpx.adobe.com/marketing-cloud/contact-support.html)에 문의하여 이 AEM 6.2용 누적 수정 팩과의 호환성을 확인하십시오.

>[!NOTE]
>
>패키지 설치를 시도하기 전에 모든 새 설치 패키지에서 유효성 검사를 실행하는 것이 좋습니다. 사전 유효성 검사는 설치 전에 발견된 모든 오류를 분석 및 보고하고, 그러한 오류, 오버레이, 권한에 대해 사전에 사용자에게 경고합니다.
>
>[https://docs.adobe.com/content/docs/en/aem/6-2/administer/content/package-manager.html#Package%20Validator](https://docs.adobe.com/content/docs/ko-KR/aem/6-2/administer/content/package-manager.html#Package%20Validator)에서 유효성 검사 옵션에 대한 문서에 액세스할 수 있습니다.

* AEM 6.2 서비스 팩 1은 CFP을 위한 필수 구성 요소입니다. 설치 지침은 [AEM 6.2 서비스 팩 1 릴리스 노트](https://docs.adobe.com/docs/en/aem/6-2/release-notes/sp1.html)를 참조하십시오.

* 누적 수정 팩 다운로드는 AEM 인스턴스에서 직접 액세스할 수 있는 [소프트웨어 배포](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html)에서 제공합니다.
* RDBMK 또는 MongoDB를 사용한 클러스터 배포를 위해 패키지 관리자를 사용하는 작성자 인스턴스에 CFP 패키지를 설치할 수 있습니다.

* 누적 수정 팩을 설치하기 전에 스냅샷을 작성하거나 AEM 인스턴스를 백업하십시오.
* CFP는 제거할 수 없습니다.

### 소프트웨어 배포를 통한 CFP 설치 {#install-the-cfp-via-package-share}

기존 AEM 6.2 SP1 인스턴스에 누적 수정 팩을 설치하려면 다음 단계를 수행하십시오.

1. [소프트웨어 배포](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq640/cumulativefixpack/aem-6.4.8-cfp-2.0.zip) 링크를 클릭하여 패키지를 다운로드합니다.

1. [패키지 관리자](http://localhost:4502/crx/packmgr/index.jsp)를 열고 **[!UICONTROL 패키지 업로드]**&#x200B;를 클릭하여 패키지를 업로드합니다.

1. 패키지 이름을 선택하고 **[!UICONTROL 설치]**&#x200B;를 클릭합니다.

### 자동 설치 {#automatic-installation}

CFP는 다음과 같은 방법으로 실행 중인 인스턴스에 자동으로 설치할 수 있습니다.

* 서버가 실행되는 동안 ../crx-quickstart/install에 패키지를 둡니다. 패키지가 자동으로 설치됩니다.
* [패키지 관리자에서 HTTP API](https://helpx.adobe.com/experience-manager/6-2/sites/administering/using/package-manager.html)를 사용하여 `cmd=install&recursive=true`를 사용하는지 확인합니다. 이 경우 중첩된 패키지가 설치됩니다.

### 설치 확인 {#validate-installation}

1. 제품 정보 페이지(/system/console/ productinfo )에서 설치된 제품 아래에 업데이트된 버전 문자열 &quot;Adobe Experience Manager, 버전 6.2.0.SP1-CFP20&quot;이 표시됩니다.
1. 모든 OSGI 번들은 OSGi 콘솔에서 ACTIVE이거나 FRAGMENT입니다(웹 콘솔 사용: /system/console/bundles).

>[!NOTE]
>
>패키지 설치가 완료되면 콘텐츠 패키지가 성공적으로 설치되었음을 나타내는 정보 메시지가 표시됩니다. (예: &quot;콘텐츠 패키지 AEM-6.2-Cumulative-Fix-Pack-SP1-CFP20이 성공적으로 설치되었습니다.&quot;)

>[!NOTE]
>
>AEM 6.2 SP1-CFP1 이후 Jackrabbit FileVault의 로그 수준이 메시지 대부분에 대해 INFO에서 DEBUG로 변경되었습니다. AEM 6.2 SP1-CFP1 이상에 설치된 콘텐츠 패키지에 대한 설치 로그를 가져오려면 `org.apache.jackrabbit.vault.packaging.impl`에 DEBUG 로그 레벨을 사용합니다.

### AEM Forms 설치 {#install-forms}

>[!NOTE]
>
>AEM Forms를 사용하지 않는 경우 이 섹션을 건너뜁니다.

#### AEM Forms 추가 기능 설치 {#install-aem-forms-add-on}

>[!NOTE]
>
>(**AEM Forms on JEE에만 해당**) AEM Forms에 CFP를 설치하는 절차는 [AEM Forms JEE에 CFP 설치하기](install-cfp-aem-forms-jee.md#install-cfp-on-aem-forms-jee)에 설명되어 있습니다.

1. AEM 6.2 SP1 CFP 패키지를 설치했는지 확인합니다.
1. 운영 체제에 대한 [AEM Forms 릴리스](aem-forms-releases.md)에 나열된 해당 양식 추가 기능 패키지를 다운로드합니다.
1. [AEM Forms 추가 기능 패키지 설치](https://helpx.adobe.com/experience-manager/6-2/forms/using/installing-configuring-aem-forms-osgi.html)에 설명된 대로 Forms 추가 기능 패키지를 설치합니다.

#### AEM Forms JEE 번들 패키지 설치 {#install-aem-forms-jee-bundles-package}

별도의 설치 관리자를 통해 AEM Forms JEE의 수정 사항이 전달됩니다. JEE의 AEM Forms에 CFP를 설치하는 방법에 대한 자세한 내용은 [AEM Forms JEE에 CFP 설치](install-cfp-aem-forms-jee.md)를 참조하십시오.

#### Forms 디자이너 설치 관리자 {#designer-installer}

1. 업데이트를 설치하려면 Designer 6.2.0_&lt;Language>_Cumulative_QF.msp 파일을 실행합니다.
1. 시작 화면에서 **업데이트**&#x200B;를 클릭합니다. 설치가 시작됩니다.
1. 설치가 완료되면 **완료**&#x200B;를 클릭합니다.

## DTM, Analytics, Target, Search &amp; Promote 연결에 대한 사용자 구성 가능한 시간 초과 매개 변수 {#user-configurable-timeout-parameters-for-dtm-analytics-target-search-promote-connections}

AEM 누적 수정 팩 6.2 SP1-CFP7 이상 릴리스를 사용하면 아래 세부 사항에 따라 위의 모든 연결에 대해 연결 시간 초과 기간을 구성할 수 있습니다.

| **연결** | **연결 시간 초과*** | **소켓 시간 제한**** |
|---|---|---|
| DTM | 30000ms | 30000ms |
| 분석 | 30000ms | 30000ms |
| 타겟 | 60000ms | 30000ms |
| Search&amp;Promote | 30000ms | 30000ms |

* **연결 시간 제한*** - 연결이 설정될 때까지의 시간 제한(밀리초)입니다. 시간 제한 값이 0이면 시간 제한을 무제한으로 해석됩니다.
* **소켓 시간 제한****- 데이터 대기 시간 또는 두 개의 연속 데이터 패킷 간 최대 비활성화 기간(밀리초)에 대한 제한 시간(밀리초)입니다.

>[!NOTE]
>
>AEM 누적 수정 팩 6.2 SP1-CFP6 및 이후 릴리스에서 Search&amp;Promote 통합에 사용된 OSGi 구성은 Apache HTTP 구성 요소 프록시 구성입니다. Day Commons HTTP Client 3.1의 프록시 구성은 이제 사용되지 않습니다.

## 태깅 콘솔에서 복제 상태 비활성화(클래식 UI)(NPR-15842) {#disable-replication-status-in-tagging-console-classic-ui-npr}

CFP3 이상을 사용하는 경우, 다음 지침에 따라 클래식 UI의 태깅 콘솔에서 복제 상태를 비활성화합니다.

* */apps*&#x200B;의 *&quot;/libs/cq/tagging/widgets/source/widgets/admin/TagAdmin.js&quot;* 오버레이

* #416 행 다음에 `replicationStateRequired`: &quot;false&quot;를 추가합니다.

   ```js
   415    baseParams: {
   416                    count: "false",
   417                    "replicationStateRequired": "false"
   418                },
   ```

## 최신 Java 8 업데이트 131에서 예외 발생(NPR-21355) {#latest-java-update-throws-an-exception-npr}

>[!NOTE]
>
>이러한 구성 설정은 문서 보안을 사용하는 AEM Forms 고객에게만 적용됩니다.

NPR-21355는 CFP12.1에 포함되어 있습니다. CFP12.1 이상을 설치하는 경우 다음 절차를 수행하여 JBoss 애플리케이션 서버에 NPR-21355를 구성합니다. Oracle WebLogic 또는 IBM WebSpehere 애플리케이션 서버에서 실행 중인 AEM Forms 서버에 CFP12.1을 설치하는 경우 추가 구성이 필요하지 않습니다:

1. 새 module.xml 파일을 백업, 삭제 및 생성합니다. 파일의 기본 위치는 [AEM_Forms_Installation_directory]/jboss/modules/system/layers/base/com/adobe/livecycle/main/입니다.

1. 새로 만든 module.xml 파일을 열어 편집합니다. 파일에 다음 코드를 추가합니다.

   ```xml
   <module xmlns="urn:jboss:module:1.1"
   name="com.adobe.livecycle">
   <resources>
   <resource-root path="cryptojcommon.jar"/>
   <resource-root path="cryptojce.jar"/>
   <resource-root path="jcmFIPS.jar"/>
   <resource-root path="certj.jar"/>
   <resource-root path="cglib.jar"/>
   </resources>
   <dependencies>
   <module name="javax.api"/>
   <module name="asm.asm"/>
   </dependencies>
   </module>
   ```

1. [AEM_Forms_Installation_directory]/jboss/modules/system/layers/base/com/adobe/livecycle/main/에 있는 jsafeFIPS.jar, jsafeJCEFIPS.jar 및 certjFIPS.jar 파일의 백업을 만들고 위의 디렉터리에서 파일을 삭제합니다.

   새 JAR 파일을 가져오려면 [Adobe 지원](https://helpx.adobe.com/marketing-cloud/contact-support.html)에 문의하십시오. [Adobe 지원](https://helpx.adobe.com/marketing-cloud/contact-support.html)([AEM_Forms_Installation_directory]/jboss/modules/system/layers/base/com/adobe/livecycle/main/)에서 가져온 JAR 파일을 배치합니다.

1. (Windows 전용) `[AEM_Forms_Installation_directory]/jboss/standalone.conf.bat` 또는 `domain.conf.bat` 구성 파일을 수정합니다.

   * 독립형 구성의 JBoss 서버인 경우, 편집할 standalone.conf.bat를 엽니다.
   * 클러스터 구성의 JBoss 서버인 경우 편집할 domain.conf.bat를 엽니다.

   끝에 다음 라인을 추가하고 파일을 저장합니다.

   JAVA_OPTS=%JAVA_OPTS%-Djnlp.com.rsa.cryptoj.fips140loader=true 설정

   JAVA_OPTS=%JAVA_OPTS%-Dcom.rsa.cryptoj.fips140initialmode=NON_FIPS140_MODE 설정

1. (Linux 기반 OS만 해당) [AEM_Forms_Installation_directory]/jboss/standalone.conf 또는 domain.conf 구성 파일을 수정합니다.

   * 독립형 구성의 JBoss 서버인 경우 편집할 standalone.conf를 엽니다.
   * 클러스터 구성의 JBoss 서버인 경우 편집할 domain.conf를 엽니다.

   끝에 다음 라인을 추가하고 파일을 저장합니다.

   JAVA_OPTS=&quot;$JAVA_OPTS-Djnlp.com.rsa.cryptoj.fips140loader=true&quot;

   JAVA_OPTS=&quot;$JAVA_OPTS -Dcom.rsa.cryptoj.fips140initialmode=NON_FIPS140_MODE&quot;

## NPR-19778에 필요한 구성 설정 {#configuration-settings-required-for-npr}

>[!NOTE]
>
>NPR-19778은 CFP14의 일부입니다.

사용자가 작업을 요청할 때 다른 사용자에 대한 공유 큐 개수는 기본적으로 새로 고쳐지지 않습니다. 이 문제를 해결하기 위해 새로운 속성을 도입했습니다. 아래 절차에 따라 AEM 인스턴스에서 이 속성을 구성하십시오.

1. 관리자 UI -> 서비스 -> 작업 공간 -> 전역 관리로 이동합니다.
1. 전역 설정을 내보냅니다.
1. 다운로드한 XML 파일에서 `<client_tasksPollingInterval>10</client_tasksPollingInterval>` 태그를 추가합니다. 여기서 10은 예제 값입니다(초). 그에 따라 수정할 수 있습니다.
1. 파일을 저장합니다.
1. 관리자 UI -> 서비스 -> 작업 공간 -> 전역 관리로 돌아갑니다.
1. 전역 설정 가져오기 섹션에서 xml 파일을 가져옵니다.
1. 이제 시스템에서 로그아웃한 다음 다시 로그인할 수 있습니다.
1. 이제 작업 공간의 다른 사용자에 대한 공유 큐 개수를 새로 고칩니다.
1. 폴링을 해제하려면 값을 0으로 변경하고 XML 파일을 다시 가져옵니다.

## UI 변경 사항 {#ui-changes}

* dc가 있는 이미지의 이미지 카드에 제목을 표시할 때의 동작 변경: title 속성을 문자열 [] ( multifield )로 설정합니다. 모든 제목이 CRX에 저장되지만 UI의 이미지 카드에 변경된 최신 제목만 표시됩니다. CQ-4217165용 핫픽스

## 알려진 문제 {#known-issues}

* CFP18에서 AEM 6.2SP1-CFP19 및 AEM 6.2SP1-CFP20을 업데이트하면 루트 리디렉션이 /sites.html/content 대신 클래식 UI 시작 페이지로 변경됩니다. sling을 수정해야 할 수 있습니다. target 속성을 /welcome.html에서 /index.html으로 변환하고 CRX 탐색기를 사용합니다. CFP17 이전 버전에서 업데이트할 때에는 이 문제가 발생하지 않습니다.

AEM 6.2 SP1-CFPx를 설치할 때 다음과 같은 일시적인 오류가 발생할 수 있습니다. 그러나 이러한 오류는 AEM 인스턴스에 영향을 주지 않고 CFP가 설치된 후 제거되기 때문에 해결이 필요하지 않습니다.

* AEM 6.2SP1-CFP20 인스턴스를 AEM 6.5로 업그레이드하는 경우 일부 별칭 URL이 다음과 같이 작동하지 않을 수 있습니다.

   * */projects.html*
   * */sites.html*

그러나 업그레이드 후 AEM 인스턴스를 다시 시작하면 해결됩니다.

* 웹 콘솔 구성 요소 세부 사항 페이지를 열면 HTTP 500 내부 서버 오류가 표시됩니다.
* 저장소 다시 시작으로 인해 다음과 같은 **구성 요소 인스턴스 만들기** 및 **서비스 팩토리에서 null 반환** 오류가 발생합니다.

   * com.day.cq.cq-personalization [com.day.cq.personalization.impl.DefaultProfileProvider(938)] 참조 profileManager에 연결하지 못해서 구성 요소 인스턴스를 만들 수 없음
   * org.apache.sling.commons.scheduler FrameworkEvent ERROR (org.osgi.framework.ServiceException: 서비스 팩토리에서 null을 반환함. (Component: com.day.cq.tagging.impl.TagGarbageCollector (1687)))

* Mongo 및 DB2의 CFP 설치 시 발견된 오류: **org.apache.sling.discovery.oak.TopologyWebConsolePlugin addDiscoveryLiteHistoryEntry: Exception: java.lang.NullPointerException**. CFP8을 통해 CFP를 설치한 후에는 이 오류가 발생하지 않습니다.
* (Adobe Granite Maintenance Scheduler 업데이트 작업) com.adobe.granite.maintenance.impl.TaskScheduler: window granite:weekly를 위한 WorkflowPurgeTask에 유지관리 작업이 없음
* `[sling-oak-observation-8]com.day.cq.dam.scene7.impl.Scene7DamChangeEventListener checking - isAsset`
* `[sling-oak-observation-8] com.day.cq.dam.scene7.impl.Scene7UploadServiceImpl synchronizeFolder failed for (null) failed`
* `[OsgiInstallerImpl] com.adobe.granite.offloading.impl.transporter.OffloadingAgentManager Cannot disable outbox replication agent.org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.adobe.cq.mobile.cq-mobile-core [com.adobe.cq.mobile.omnisearch.impl.MobileAppsOmniSearchHandler(3058)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.adobe.aemds.formsmanager.adobe-aemds-formsanddocuments-core [com.adobe.aem.formsndocuments.handlers.FormsAndDocumentOmniSearchHandler(2718)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored15.02.2017 08:28:06.511`
* `[OsgiInstallerImpl] com.adobe.aemds.formsmanager.adobe-aemds-formsanddocuments-core [com.adobe.aem.formsndocuments.handlers.ThemeOmniSearchHandler(2722)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.adobe.cq.screens.com.adobe.cq.screens.dcc [com.adobe.cq.screens.dcc.impl.ScreensOmniSearchHandler(332)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Cannot derive user name for bundle com.adobe.cq.screens.com.adobe.cq.screens.dcc [158] and sub service omnisearch-service)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.day.cq.cq-personalization [com.day.cq.personalization.impl.omnisearch.OfferOmniSearchHandler(947)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Cannot derive user name for bundle com.day.cq.cq-personalization [250] and sub service omnisearch-service)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.day.cq.cq-personalization [com.day.cq.personalization.impl.omnisearch.AudienceOmniSearchHandler(957)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Cannot derive user name for bundle com.day.cq.cq-personalization [250] and sub service omnisearch-service)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.day.cq.cq-personalization [com.day.cq.personalization.impl.omnisearch.ActivitiesOmnisearchHandler(958)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Cannot derive user name for bundle com.day.cq.cq-personalization [250] and sub service omnisearch-service)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.adobe.cq.commerce.cq-commerce-core [com.adobe.cq.commerce.impl.omnisearch.OrdersOmniSearchHandler(623)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Cannot derive user name for bundle com.adobe.cq.commerce.cq-commerce-core [225] and sub service omnisearch-service)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.adobe.cq.commerce.cq-commerce-core [com.adobe.cq.commerce.impl.omnisearch.ProductsOmniSearchHandler(625)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Cannot derive user name for bundle com.adobe.cq.commerce.cq-commerce-core [225] and sub service omnisearch-service)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.adobe.cq.commerce.cq-commerce-core [com.adobe.cq.commerce.impl.omnisearch.ProductCollectionsOmniSearchHandler(627)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Cannot derive user name for bundle com.adobe.cq.commerce.cq-commerce-core [225] and sub service omnisearch-service)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.adobe.cq.commerce.cq-commerce-core [com.adobe.cq.commerce.impl.omnisearch.CatalogsOmniSearchHandler(633)] The deactivate method has thrown an exception (org.apache.sling.api.resource.LoginException: Cannot derive user name for bundle com.adobe.cq.commerce.cq-commerce-core [225] and sub service omnisearch-service)org.apache.sling.api.resource.LoginException: Login Failure: all modules ignored`
* `[OsgiInstallerImpl] com.day.cq.dam.dam-webdav-support [com.adobe.cq.dam.webdav.impl.io.DamWebdavVersionLinkingJob(1697)] The deactivate method has thrown an exception (java.util.NoSuchElementException: No job found with name com.adobe.cq.dam.webdav.impl.io.DamWebdavVersionLinkingJob){code}`
* `[sling-default-5-discovery.connectors.common.runner.d6a26647-dd1c-4665-be2c-afdd19397e77096a1c19-18ce-4051-bbf1-166caed986f2] org.apache.sling.discovery.oak.pinger.OakViewChecker issueConnectorPings: connectorRegistry is null`
* `[sling-default-5-discovery.connectors.common.runner.d6a26647-dd1c-4665-be2c-afdd19397e77096a1c19-18ce-4051-bbf1-166caed986f2] org.apache.sling.discovery.oak.pinger.OakViewChecker announcementRegistry is null`
* 스마트 태그 기능 팩이 포함된 AEM 6.2 SP1에 CFPx를 설치하면 DAM 에셋 업데이트 워크플로에서 스마트 태그 에셋에 대해 이전에 추가한 워크플로 단계가 삭제됩니다.

]AEM 6.2 SP1의 알려진 문제[ 목록을 참조하십시오(https://docs.adobe.com/docs/en/aem/6-2/release-notes/sp1.html#Known Issues).

## Uber Jar {#uber-jar}

6.2 SP1-CFP20용 Uber Jar을 [Adobe Public Maven 저장소](https://repo.adobe.com/nexus/content/groups/public/com/adobe/aem/uber-jar/6.2.SP1-CFP19/)에서 사용할 수 있습니다.

Maven 프로젝트에서 Uber Jar을 사용하려면 프로젝트 POM에 다음 종속성을 포함하십시오.

```XML
<dependency>
    <groupId>com.adobe.aem</groupId>
    <artifactId>uber-jar</artifactId>
    <version>6.2.SP1-CFP20</version>
    <classifier>apis</classifier>
    <scope>provided</scope>
</dependency>
```

## OSGi 번들 및 콘텐츠 패키지가 포함됨 {#osgi-bundles-and-content-packages-included-5}

다음 텍스트 문서에는 CFP에 포함된 OSGi 번들 및 콘텐츠 패키지 목록이 있습니다.

* [AEM 6.2 SP1-CFP20에 포함된 OSGi 번들 목록](assets/do-not-localize/updated.txt)
* [AEM 6.2 SP1-CFP20에 포함된 콘텐츠 패키지 목록](assets/do-not-localize/content_package_comparison_result.txt)

>[!MORELIKETHIS]
>
>* [AEM 6.2 핫픽스 페이지](https://helpx.adobe.com/experience-manager/kb/aem62-available-hotfixes.html)
>* [AEM 6.2 SP1 릴리스 노트](https://docs.adobe.com/content/docs/ko-kr/aem/6-2/release-notes/sp1.html)
>* [AEM 6.2 릴리스 노트](https://docs.adobe.com/docs/ko/aem/6-2/release-notes.html)
>* [AEM 제품 페이지](http://www.adobe.com/solutions/web-experience-management.html)
>* [AEM 6.2 설명서](https://docs.adobe.com/content/docs/en/aem/6-2.html)
>* [Adobe 우선 순위 제품 업데이트](https://docs.adobe.com/content/help/ko-KR/release-notes/experience-cloud/current.html)

