---
title: AEM 6.3 누적 수정 팩
description: AEM 6.3 누적 수정 팩 릴리스 정보
exl-id: 04969587-a904-44cb-83e0-51707ac6a87f
source-git-commit: 53803f61394144ed81367a5c050814223fc6d565
workflow-type: ht
source-wordcount: '17347'
ht-degree: 100%

---

# AEM 6.3 누적 수정 팩 릴리스 정보 {#release-notes-aem-cumulative-fix-pack}

## 릴리스 정보 {#release-information}

| **제품** | Adobe Experience Manager |
|---|---|
| **버전** | 6.3 |
| **릴리스** | [소프트웨어 배포](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq630/cumulativefixpack/aem-6.3.3-cfp-8.0.zip)의 누적 수정 팩 6.3.3.8 |
| **전제 조건** | [AEM 6.3 서비스 팩 3(6.3.3.0)](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions) |
| **일반 가용성** | 2020년 3월 5일 |

### 누적 수정 팩 {#cumulative-fix-pack}

Adobe는 수정 사항을 릴리스하기 위해 단일 게재 모델을 도입했습니다. Adobe는 이제 개별 문제에 대한 핫픽스를 릴리스하지 않고 매달 CFP(누적 수정 팩)를 릴리스합니다(품질 검사 통과 여부에 따름). CFP는 여러 수정 사항을 집계한 콘텐츠 패키지로, 주로 버그 수정 사항이 포함되지만, 기능 팩이 포함될 수도 있습니다. 개별 핫픽스 릴리스와 비교해 다음과 같은 이점이 있습니다.

* 기본적으로 누적(예: CFP에 이전 CFP를 통해 게재된 수정 사항이 포함됨)
* 개선된 품질 보증
* 간단한 설치(사용자가 최신 서비스 팩을 제외하고, 종속성이 없는 단일 패키지로 CFP를 설치함)

CFP 및 기타 릴리스 유형에 대한 자세한 내용은 [유지 관리 릴리스 차량 정의](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)를 참조하십시오.

## 릴리스 정보 {#about-the-release}

AEM 누적 수정 팩 6.3.3.8은 2018년 9월, AEM 6.3 서비스 팩 3(6.3.3.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.3.8은 AEM 6.3 서비스 팩 3에 종속됩니다. 따라서 AEM 6.3 서비스 팩 3을 설치한 후 AEM 누적 수정 팩 6.3.3.x 패키지를 설치해야 합니다. 설치 지침은 [AEM 6.3 서비스 팩 3](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)의 릴리스 정보를 참조하십시오.

**AEM 누적 수정 팩**&#x200B;의 주요 사항은 다음과 같습니다.

* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.20으로 업데이트되었습니다.

>[!CAUTION]
>
>설치된 기능 팩 간의 호환성을 확인하지 않고 CFP를 적용하면 시스템 오류가 발생하거나 사용자 정의 구성이 손실될 수 있으며, 이를 해결하기 위해 백업에서 복원해야 할 수 있습니다.

>[!NOTE]
>
>6.3.3.0 이하 버전의 AEM 인스턴스의 경우, Adobe에서는 AEM 인스턴스에 많은 사용자가 있는 고객의 설치 폴더를 통해 SP/CFP를 배포할 것을 권장합니다.

>[!NOTE]
>
>MongoDB Enterprise 3.6은 AEM 버전 6.3.3.1부터 지원됩니다.

## 문제 목록 {#changes}

이 섹션에는 현재 CFP에 포함된 모든 문제와 핫픽스가 나와 있습니다.

또한 이 CFP에는 [이전 누적 수정 팩](#previous)에 제공된 핫픽스가 포함되어 있습니다.

### 자산 {#assets}

* 컬렉션에 자산을 추가하는 동안 [컬렉션에 추가] 페이지의 카드 보기에 모든 사용 가능한 컬렉션이 표시되지 않습니다(NPR-32537).

### Sites {#sites}

* Parsys와 그 안의 구성 요소를 선택하고 키보드 단축키를 사용하여 선택한 항목을 삭제하면 이 작업을 통해 구성 요소와 상위 Parsys가 모두 삭제됩니다(NPR-32071).
* 페이지의 속성이 저장되면 잘못된 노드가 생성됩니다(NPR-31774).

### 통합 {#integrations}

* ReportSuitesServlet이 SSRF에 취약합니다(NPR-32162).

### 캠페인 타겟팅 {#campaign-targeting}

* 작성자 인스턴스에서 변경된 구성 요소의 콘텐츠가 활성화되면 구성 요소가 다시 시작될 때까지 게시 인스턴스에 표시되지 않습니다. **com.day.cq.personalization.impl.TargetedContentManagerImpl**(NPR-32489 및 NPR-32232).
* 게시할 때 Context Hub 성능이 충돌합니다(NPR-31170).

### Brand Portal {#brand-portal}

* Adobe Developer는 Brand Portal용 Adobe Experience Manager 6.3과 통합되지 않습니다(NPR-32056).

### Forms {#forms}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

#### Forms 추가 기능 패키지 {#forms-add-on-package}

>[!NOTE]
>
>AEM Forms 추가 기능 패키지는 양식 기능을 AEM 서비스 팩 및 누적 수정 팩과 맞추는 데 도움이 됩니다. 따라서 반드시 AEM 서비스 팩, 누적 수정 팩 또는 기능 팩을 설치한 후 AEM Forms 추가 기능 패키지를 설치해야 합니다.

* Designer: 태그 지정 옵션이 활성화된 경우 생성된 PDF 출력에서 하위 양식 테두리가 사라집니다(NPR-32324 및 NPR-32545).
* Designer: 표에 병합된 셀이 있는 경우 출력 서비스를 사용하여 XDP 양식에서 변환된 출력 PDF 파일에 접근성 테스트를 수행하면 오류가 발생합니다(NPR-32068).
* 문서 보안: `DisableGlobalOfflineSynchronizationData` 옵션이 `True`로 설정되어 보호된 PDF 파일을 오프라인으로 열 수 없습니다(NPR-32080).

**6.3.0-0047에서 해결된 문제**

* (JEE만 해당) Apache `Log4j2`에 대해 심각한 보안 취약성(CVE-2021-44228 및 CVE-2021-45046)이 보고되었습니다.

## 이전 누적 수정 팩에 포함된 핫픽스 및 기능 팩 {#previous}

### 누적 수정 팩 6.3.3.7 {#cumulative-fix-pack-1}

AEM 누적 수정 팩 6.3.3.7은 2018년 9월, AEM 6.3 서비스 팩 3(6.3.3.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.3.7은 AEM 6.3 서비스 팩 3에 종속됩니다. 따라서 AEM 6.3 서비스 팩 3을 설치한 후 AEM 누적 수정 팩 6.3.3.x 패키지를 설치해야 합니다. 설치 지침은 [AEM 6.3 서비스 팩 3](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)의 릴리스 정보를 참조하십시오.

### 자산 {#assets-1}

* 콘텐츠 전용 드롭다운에서 필터 옵션을 선택하고 이동 옵션을 선택하기 전에 선택한 자산(Touch UI의 열 보기에서)도 이동됩니다(NPR-30693).
* `${extension}` 변수가 워크플로 처리 시 작성자 인스턴스에 렌더링되지 않습니다(NPR-31694).
* Dynamic Media 하이브리드 모드에 대해 구성된 만료(클라이언트 캐시 TTL(Time To Live)) 값이 Dynamic Media 게재 환경(NPR-31114)에 복제되지 않습니다.
* 기본 필터를 사용한 후에도 Dynamic Media - Scene7 배포 시 실행 중인 작성자 인스턴스의 게시 인스턴스에 자산이 복제됩니다(NPR-30856).

### Sites {#sites-1}

* 기본 페이지의 페이지 속성이 로드되지 않고 NullPointerException이 반환됩니다. 이 문제는 `cq:blueprin`t 속성 추가 시 해결됩니다(NPR-30901).
* 롤아웃 구성이 루트 노드의 blueprintConfig에서 제대로 검색되지 않습니다. 비활성화가 블루프린트와 라이브 카피 모두에 대해 트리거됩니다. 블루프린트에 대한 비활성화만 트리거합니다(NPR-30866).
* 사용자가 페이지를 롤아웃하면 롤아웃 구성 대화 상자에 중복 Live Copy 경로가 표시됩니다(NPR-30438).
* 기본 제공되는 스캐폴딩 RTE(리치 텍스트 편집기)가 예기치 않게 인라인 글꼴 크기를 요소에 적용합니다(NPR-31283, NPR-30922).
* Adobe Campaign에서 기본 제공되는 디자인 Importer 구성 요소가 포함된 캠페인을 동기화할 수 없습니다(NPR-30890).
* 리치 텍스트 편집기(RTE)가 임베드된 테이블을 목록 항목으로 삽입할 수 없습니다(NPR-30878).
* 사용자는 왼쪽 레일 필드에 초점을 맞추고 키보드 단축키를 사용하여 콘텐츠를 붙여넣습니다. 이러한 작업에서 왼쪽 레일 필드에서 복사한 콘텐츠 대신 페이지 편집기 클립보드의 콘텐츠를 붙여넣습니다(NPR-31173).
* 사용자가 콘텐츠 조각을 편집하면 이미 삭제된 콘텐츠 조각의 변형이 복원됩니다(NPR-31272).
* AEM Site에서 언어 사본을 만들지 않습니다(NPR-30690).
* 페이지 편집기 작업에는 라이브 사본을 롤아웃하는 컨트롤이 없습니다(NPR-30613).

### 커뮤니티 {#communities}

* 활동 및 알림 제목이 일치하지 않습니다(NPR-30940).
* Analytics 보고서는 AEM 작성자 환경에 채워지지 않습니다. 대신 빈 페이지가 표시됩니다(NPR-30905).
* 페이지 매김이 Communities 블로그에서 제대로 작동하지 않습니다(NPR-30827).

### Foundation {#foundation}

* Jetty 기반 HTTP 서비스에 대한 버퍼 크기 구성의 업데이트가 저장되지 않습니다(NPR-30925).

### Forms {#forms-1}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-1}

>[!NOTE]
>
>AEM Forms 추가 기능 패키지는 양식 기능을 AEM 서비스 팩 및 누적 수정 팩과 맞추는 데 도움이 됩니다. 따라서 반드시 AEM 서비스 팩, 누적 수정 팩 또는 기능 팩을 설치한 후 AEM Forms 추가 기능 패키지를 설치해야 합니다.

#### 적응형 양식 {#adaptive-forms}

* 스크립트를 사용하여 계산된 부동 값이 양식 세트의 일부인 양식에 올바르게 표시되지 않습니다(NPR-30802).

#### HTML5 양식 {#html-forms}

* XDP 양식의 HTML5 미리보기를 생성하면 하위 양식의 인스턴스를 추가하는 동안 깜박임이 표시됩니다(NPR-30908).

### Forms JEE 설치 관리자 {#forms-jee-installer}

#### Acrobat 서비스 {#document-services}

* HTML을 PDF로 변환 시 발생하는 문제를 해결하기 위해 패치를 적용하면 OutputService에 올바르지 않은 응답이 표시됩니다(NPR-31504).

#### PDFG 서비스 {#pdfg-service}

* JMX 콘솔의 최대 재사용 횟수는 HTML2PDF 서비스에 대해 표시되지 않습니다(NPR-30305).

#### Foundation JEE {#foundation-jee}

* JMX 콘솔의 최대 재사용 횟수는 HTML2PDF 서비스에 대해 표시되지 않습니다(NPR-30136).

### 누적 수정 팩 6.3.3.6 {#cumulative-fix-pack-2}

AEM 누적 수정 팩 6.3.3.6은 2018년 9월, AEM 6.3 서비스 팩 3(6.3.3.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.3.6은 AEM 6.3 서비스 팩 3에 종속됩니다. 따라서 AEM 6.3 서비스 팩 3을 설치한 후 AEM 누적 수정 팩 6.3.3.x 패키지를 설치해야 합니다. 설치 지침은 [AEM 6.3 서비스 팩 3](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)의 릴리스 정보를 참조하십시오.

### 자산 {#assets-2}

* Dynamic Video별 비디오 집계는 결과 세트에 있는 상위 100개 항목만 반환합니다. NPR-30441: CQ-4213561용 핫픽스
* Data power를 통한 Adobe 스마트 태그 연결 문제. NPR-30026: CQ-4269457용 핫픽스
* 이름에 백분율 기호(%)가 있는 폴더로 아카이브 압축을 풀면 Assets 인터페이스를 사용하여 열 수 없습니다. NPR-29989: CQ-4270467용 핫픽스
* 대용량 PDF 파일의 하위 자산을 처리하면 OOME(OutOfMemoryError) 예외가 발생합니다. NPR-29851: CQ-4269574용 핫픽스

### Sites {#sites-2}

* AEM 및 캠페인 통합 중에 ContextHub 오류가 발생합니다. NPR-30624: CQ-4250790용 핫픽스
* AEM 서버가 다시 시작되는 경우 자산에 저장된 &#39;onTime&#39; 또는 &#39;offTime&#39; 메타데이터 속성이 호출되지 않습니다. NPR-30412: CQ-4272784용 핫픽스
* CSV 내보내기를 생성하는 동안 목록 보기에 대한 사용자 정의 열을 추가하면 보고서가 손상됩니다. NPR-30208: CQ-4273344용 핫픽스
* /etc/reports/의 OOTB 보고서가 올바르게 작동하지 않으며, 이전 데이터 그래프가 표시되지 않습니다. NPR-30016: CQ-4220180용 핫픽스
* resourceType 요청 매개변수의 값은 큰따옴표에 캡슐화된 HTML 태그 속성값에 복사됩니다. NPR-29832: CQ-4255365용 핫픽스

### 커뮤니티 {#communities-1}

* AEM Communities 관리 콘솔에 중복 콘텐츠 문제가 있습니다. NPR-30667: CQ-4276829용 핫픽스

### 번역 {#translation}

* 번역 문제 - 일부 구성 요소만 기계 번역을 사용하여 번역됩니다. NPR-30079: CQ-4273764용 핫픽스
* 번역 프레임워크를 사용할 때 여러 번역 작업에 페이지를 추가하면 오류가 트리거됩니다. NPR-29746: CQ-4270953용 핫픽스

### Forms {#forms-2}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-2}

>[!NOTE]
>
>AEM Forms 추가 기능 패키지는 양식 기능을 AEM 서비스 팩 및 누적 수정 팩과 맞추는 데 도움이 됩니다. 따라서 반드시 AEM 서비스 팩, 누적 수정 팩 또는 기능 팩을 설치한 후 AEM Forms 추가 기능 패키지를 설치해야 합니다.

#### HTML5 양식 {#html-forms-1}

* 검색 모드에서 비시각적 데스크탑 액세스를 사용하여 HTML5 양식을 읽을 때 Chrome 브라우저는 양식 디자인에서 각 SVG(규모 가변적인 벡터 그래픽) 앞에 있는 “그래픽”을 읽습니다. NPR-30451: CQ-4274732용 핫픽스

#### Forms - 백엔드 통합 {#forms-backend-integration}

* FDM(Form Data Model)을 생성하는 동안 데이터베이스 연결에 대한 서비스/데이터 소스를 확인할 수 없습니다. NPR-30108: CQ-4273359용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-1}

#### Forms - Acrobat 서비스 {#forms-document-services}

* HTML에서 PDF 서비스로 로드 테스트를 수행하면 오류가 발생하고 실패하며, 파일 유형 설정이 AEM Forms 서버에서 제거됩니다. NPR-30111, NPR-30086: CQ-4271495용 핫픽스

### 누적 수정 팩 6.3.3.5 {#cumulative-fix-pack-3}

AEM 누적 수정 팩 6.3.3.5은 2018년 9월, AEM 6.3 서비스 팩 3(6.3.3.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.3.5는 AEM 6.3 서비스 팩 3에 종속됩니다. 따라서 AEM 6.3 서비스 팩 3을 설치한 후 AEM 누적 수정 팩 6.3.3.x 패키지를 설치해야 합니다. 설치 지침은 [AEM 6.3 서비스 팩 3](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)의 릴리스 정보를 참조하십시오.

**AEM 누적 수정 팩**&#x200B;의 주요 사항은 다음과 같습니다.

* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.17으로 업데이트되었습니다.

### 자산 {#assets-3}

* S3 다중 부분 지원에 대한 DAM DMGateway 인터페이스가 업데이트되었습니다. NPR-29740: Q-4226303용 핫픽스
* 자산 세부 정보 페이지에서 비디오 자산에 대한 이미지 렌디션을 삭제할 수 없습니다. NPR-29417: CQ-4268675용 핫픽스
* 소유자가 개인 폴더 내에 개인 폴더를 만들 수 없습니다. NPR-29397: CQ-4229830용 핫픽스
* 2GB 이상의 Adobe Illustrator 아트워크 파일을 업로드하면 Java™ 힙 공간 오류가 생성됩니다. NPR-29265: CQ-4226217용 핫픽스
* DAM CQ MIME 유형 서비스가 m3u8의 텍스트를 적용하면 자산을 사용할 수 없게 됩니다. NPR-29259: CQ-4264052용 핫픽스
* Edge에서 컬렉션을 만들려고 할 때 만들기 옵션이 작동하지 않습니다. NPR-29248: CQ-4265699 및 CQ-4265438용 핫픽스
* 자산 링크를 공유하면 폴더의 일부 자산에 대해 빈 회색 카드를 표시합니다. NPR-29831: CQ-4270187용 핫픽스
* 자산에 추가된 새 태그가 저장되지 않고 속성에서 사라집니다. CQ-4271931, CQ-4270476용 핫픽스

### Sites {#sites-3}

* CoralUI가 Multifield에서 사용되는 경우 fileReferenceParameter는 multifield 수준이 아닌 구성 요소 수준에 저장됩니다. NPR-29535: CQ-4266129용 핫픽스
* AEM 6.3.3.3에서 최신 및 현재 페이지 버전 비교를 시도하는 중 문제가 발생했습니다. NPR-29532: CQ-4269639용 핫픽스
* 검색에 지정된 경로와 관련 없이 경로 필드가 루트 경로에서 열립니다. NPR-29398: CQ-4268897용 핫픽스
* (경험 조각)
FacebookApplication#setUpApp은 이제 사용되지 않는 API를 사용하므로, 더는 작동하지 않습니다. NPR-29213: CQ-4266630용 핫픽스
* 인스턴스에서 축소가 사용되면 WCM 페이지에 구성 요소를 추가할 때 오류 경고가 생성됩니다. NPR-29476: CQ-4266197용 핫픽스
* 빈 속성 및 여러 속성이 롤아웃 중에 블루프린트에서 전파되지 않습니다. 블루프린트로 재설정된 Live Copy가 구성 요소에 대해 작동하지 않습니다. NPR-29252: CQ-4264928, CQ-4264926, CQ-4267722용 핫픽스
* 소스 편집 모드에 있는 동안 전체 화면에서 리치 텍스트 편집기를 최소화하면 콘텐츠가 손실됩니다. NPR-28838: CQ-4260584용 핫픽스

### 커뮤니티 {#communities-2}

* 중재자 권한이 없는 방문자 및 멤버는 URL을 붙여넣어 승인되지 않은 게시물 및 보류 중인 게시물을 볼 수 있습니다. NPR-29726: CQ-4271124용 핫픽스
* 커뮤니티에 대한 사용자 로그인에서 최대 40~50초의 높은 응답 시간이 관찰됩니다. NPR-29679: CQ-4269444용 핫픽스
* 키가 교환된 사용자 이름 및 이메일로 생성된 것으로 보이므로 다른 사용자 이름 및 이메일로 로그인한 경우에는 암호를 재설정할 수 없습니다. NPR-29281: CQ-4268694용 핫픽스

### 경험 조각 {#experience-fragments}

* 스마트 이미지를 사용하는 경우 경험 조각을 대상으로 내보낼 수 없습니다. CQ-4269606용 핫픽스

### 복제 {#replication}

* 복제 에이전트 구성 요소는 중요한 정보를 권한이 없는 사용자에게 공개하는 취약성이 있습니다. NPR-29613: Granite-25070용 핫픽스
* 사용자가 제공한 데이터는 `cq/replication/components/agent` 구성 요소에서 출력에 이스케이프되지 않으므로, 저장된 XSS(크로스 사이트 스크립팅)에 취약성이 발생합니다. NPR-29452: CQ-4266263용 핫픽스

### Forms {#forms-3}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-3}

* AEM Forms 추가 기능 패키지에는 새로운 수정 사항이 없습니다.

### Forms JEE 설치 관리자 {#forms-jee-installer-2}

* AEM Forms JEE 설치 관리자에는 새 수정 사항이 없습니다.

### 6.3.3.5에 포함된 OSGi 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in}

AEM 6.3.3.5에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/6_5-bundle-list.txt)

AEM 6.3.3.5에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/content_packages6335.txt)

### 누적 수정 팩 6.3.3.4 {#cumulative-fix-pack-4}

AEM 누적 수정 팩 6.3.3.4은 2018년 9월, AEM 6.3 서비스 팩 3(6.3.3.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.3.4는 AEM 6.3 서비스 팩 3에 종속됩니다. 따라서 AEM 6.3 서비스 팩 3을 설치한 후 AEM 누적 수정 팩 6.3.3.x 패키지를 설치해야 합니다. 설치 지침은 [AEM 6.3 서비스 팩 3](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)의 릴리스 정보를 참조하십시오.

**AEM 누적 수정 팩**&#x200B;의 주요 사항은 다음과 같습니다.

* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.16으로 업데이트되었습니다.
* Brand Portal 복제 에이전트에 소켓 제한 시간 및 연결 제한 시간이 추가되었습니다.

### 자산 {#assets-4}

* 동일한 이름의 아카이브를 다시 업로드하는 경우 새로 처리된 자산에 대해 표현물이 생성되지 않습니다. NPR-28643: CQ-4262286용 핫픽스
* 워크플로 CommandLineProcess가 작은 따옴표가 있는 파일 이름에서 오류가 발생합니다. NPR-28805: CQ-4262287용 핫픽스
* 컬렉션 페이지와 필터를 사용할 때 컬렉션 페이지의 값이 서로 다릅니다. NPR-28642: CQ-4261405용 핫픽스
* CommitFailedException은 큰 zip 아카이브 자산 업로드를 사용하여 트리거합니다. NPR-28528: CQ-4260903용 핫픽스
* 특수 문자가 포함된 폴더를 편집할 때 폴더 메타데이터가 저장되지 않습니다. NPR-28211: CQ-4260401용 핫픽스
* 자산 세부 정보 페이지에서 비디오 자산의 이미지 렌디션을 삭제할 수 없습니다. NPR-29149: CQ-4266073용 핫픽스
* DMComponent를 사용한 DMS7 데스크탑 비디오 게재는 게시 모드에서 비디오 재생에 점진적 다운로드를 사용하며 스트리밍되지 않습니다. NPR-28754: CQ-4263732용 핫픽스
* /etc/dam/video/dynamicmedia에 대한 액세스를 제한하면 이미지 관리자에 대한 기능을 비활성화하므로 이미지 사전 설정을 작성/편집할 수 없습니다. NPR-28662: CQ-4263022용 핫픽스
* DMS7로 인코딩된 비디오 파일이 포함된 링크를 공유하면 폴더가 비어 있게 됩니다. NPR-28851: CQ-4206743용 핫픽스
* AEM에서 Brand Portal로의 복제가 오랫동안 중지됩니다. NPR-28913: CQ-4254932용 핫픽스

### 커뮤니티 {#communities-3}

* Outlook 보낸 편지함 및 받은 편지함 폴더에 첨부 파일이 있는 메시지를 열 수 없습니다. NPR-28559: CQ-4217072용 핫픽스

### Sites {#sites-4}

* 6.3에 대한 SuggestionHandler의 XSS(크로스 사이트 스크립팅)입니다. NPR-28692: CQ-4253821용 핫픽스
* 각 LiveCopy에 모든 분기를 포함하지 않고 심층 롤아웃이 종료됩니다. NPR-29175: CQ-4239472용 핫픽스
* (MSM) oak-색인을 사용하여 LiveCopyIndex를 구현합니다. NPR-29198: CQ-4222472용 핫픽스
* 파일에는 `coral.js` 취약한 버전의 라이브러리가 포함되어 있습니다 `handlebars.js`. NPR-26973: CQ-4255377용 핫픽스
* 중첩된 레이아웃 컨테이너 및 텍스트 구성 요소와 함께 Target 구성 요소를 사용하는 경우 텍스트를 편집하거나 컨테이너를 클릭하면 “null currentPos 속성을 읽을 수 없습니다”라는 JavaScript 오류가 발생합니다. NPR-29077: CQ-4246594용 핫픽스
* (Touch UI) 다른 태그로 이미 태그가 지정된 페이지로 태그를 대량 업데이트할 수 없습니다. NPR-28729: CQ-4262922용 핫픽스
* 카드 보기에서 변형을 열면 500 오류가 발생합니다. NPR-28611: CQ-4263571용 핫픽스
* 기본에서 이동된 구조를 롤아웃하면 잘못된 `cq:moveTarget`으로 이동됩니다. NPR-28968: CQ-4265280용 핫픽스

### 통합 {#integration}

* (클라우드 서비스 구성) 루트 수준에 표시되는 “다음에서 상속” 확인란을 제거해야 합니다. NPR-28771: CQ-4259676용 핫픽스
* com.day.cq.personalization.impl.TeaserResourceEventHandler가 무한 루프로 이동하고 게시 인스턴스의 노드에 대한 업데이트가 발생합니다. NPR-28561: CQ-4263096용 핫픽스
* Bright edge 자격 증명을 사용할 수 없고 연결 오류가 발생합니다. NPR-29167: CQ-4265872용 핫픽스
* &#39;Resource&#39; 클래스에 대한 import 문이 누락되어 OfferproxyTandtProvider.java에서 컴파일 문제가 발생합니다. import 문이 누락되었습니다. org.apache.sling.api.resource.Resource를 가져옵니다. NPR-28772

### 상거래 {#commerce}

* 전자 상거래 컬렉션 내부의 자산에 대해 정렬 옵션이 작동하지 않습니다. NPR-28755: CQ-4213622용 핫픽스

### Jetty {#jetty}

* 6.3.3 상단에 CFP2 설치 후 모든 302 리디렉션에 대해 error.log에 Jetty 예외가 발생합니다. NPR-28606: CQ-4262844용 백포트

### UI - Foundation {#ui-foundation}

* 태그를 클릭하면 글로벌 mouse-up 이벤트가 제거되고 대화 상자가 끌어오기 가능한 모드에서 중단됩니다. NPR-28641: CUI-7294용 핫픽스

### WCM - MSM {#wcm-msm}

* PageManager 이동을 위한 PushOnModify 롤아웃은 두 세션에서 여러 번 커밋되므로 경합 상태가 발생합니다. NPR-28880: CQ-4266191용 핫픽스

### 취약성 {#vulnerability}

* CSRF 보호 프레임워크가 AEM Foundation Forms에서 작동하지 않습니다. NPR-28612: GRANITE-22231용 핫픽스

### Forms {#forms-4}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

AEM Forms의 주요 사항은 다음과 같습니다.

* 정책 세트 보기 페이지에서 페이지당 항목 수를 선택하는 옵션이 활성화됩니다.
* 모든 브라우저에 대한 공유 대기열 기능이 추가되었습니다.

### Forms 추가 기능 패키지 {#forms-add-on-package-4}

#### Forms - 워크플로 {#forms-workflow}

* 공유 대기열 응답 작업이 HTML5 작업 영역에서 플래시 요소를 엽니다. NPR-29161: CQ-4266498용 핫픽스
* 버튼에 모음 기호 문자가 포함된 경우 작업 영역에서 제출할 수 없습니다. NPR-29014: CQ-4263172용 핫픽스

#### Forms - 문서 보안 {#forms-document-security}

* 정책 세트 보기 페이지에서 페이지당 항목 수를 선택하는 옵션을 활성화합니다. NPR-29243: CQ-4268567 및 CQ-4265132용 핫픽스

#### Forms - Acrobat 서비스 {#forms-document-services-1}

* OSGi Forms 어셈블러가 Acrobat 파일에서 작동하지 않습니다. NPR-29049: CQ-4254426용 핫픽스

#### HTML5 양식 {#html-forms-2}

* XDP를 Designer에서 PDF로 미리 보거나 HTML과 동일한 PDF로 미리 보는 동안 다른 동작이 발생합니다. NPR-28602: CQ-4260239용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-3}

* AEM Forms JEE 설치 관리자에는 새 수정 사항이 없습니다.

### 6.3.3.4에 포함된 OSGi 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-1}

AEM 6.3.3.4에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/list_of_osgi_bundlesincludedinaem633.4)

AEM 6.3.3.4에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/list_of_content_packagesincludedinaem633.4)

### 누적 수정 팩 6.3.3.3 {#cumulative-fix-pack-5}

AEM 누적 수정 팩 6.3.3.3은 2018년 9월, AEM 6.3 서비스 팩 3(6.3.3.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.3.3은 AEM 6.3 서비스 팩 3에 종속됩니다. 따라서 AEM 6.3 서비스 팩 3을 설치한 후 AEM 누적 수정 팩 6.3.3.x 패키지를 설치해야 합니다. 설치 지침은 [AEM 6.3 서비스 팩 3](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)의 릴리스 정보를 참조하십시오.

**AEM 누적 수정 팩**&#x200B;의 주요 사항은 다음과 같습니다.

* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.16으로 업데이트되었습니다.
* 정책 세트 목록 페이지 매김이 페이지당 레코드를 50개로 제한하도록 변경되었습니다.
* rep: 캐시가 게시 인스턴스의 AEM Communities 사용자 동기화 리스너에 있는 Ignorable 노드에 추가되었습니다.
* 목록 및 카드 보기 버튼에 대한 Aria 레이블이 추가되었습니다.
* 검색이 수행될 때 쉼표에 대한 이스케이프 문자가 포함되었습니다.
* 콘텐츠 정책에 대한 합성 리소스를 지원하도록 설정되었습니다.

#### 자산 {#assets-5}

* `.jp2`, `.max`, `.oft`, `.msg` 유형의 여러 파일을 다운로드할 수 없습니다. NPR-28002: CQ-4210856용 핫픽스
* ImageServer 게시 설정은 하이브리드 게재에 복제되지 않습니다. NPR-28329: CQ-4253030용 핫픽스

#### 커뮤니티 {#communities-4}

* 게시할 때 AEM Communities 지원 구성 요소에 대한 키보드 탐색이 활성화됩니다. NPR-27739: CQ-4253856용 핫픽스
* 콘텐츠 재생을 트리거하기 위해 키보드 탐색을 사용하도록 설정했습니다. NPR-27738: CQ-4254026용 핫픽스
* 목록 및 카드 보기 버튼에 대한 Aria 레이블이 추가되었습니다. NPR-27736: CQ-4254027용 핫픽스
* (백포트) rep: 캐시가 게시 인스턴스의 AEM Communities 사용자 동기화 리스너에 있는 Ignorable 노드에 추가되었습니다. NPR-27841: CQ-4247234용 핫픽스
* 특수 문자에는 검색 상자에 이스케이프 문자(\)가 접두사로 추가됩니다. NPR-27839: CQ-4259757용 핫픽스
* 빠른 검색에서 `(`, `+` 및 `?` 등의 문자를 검색하는 중 오류가 발생합니다. NPR-28212: CQ-4260969용 핫픽스
* API를 사용한 사용자 생성 콘텐츠에서 댓글을 삭제할 수 없습니다. NPR-28075: CQ-4260534용 핫픽스
* 새 댓글이 게시되면 다음 페이지에 게시된 댓글이 노란색으로 강조 표시됩니다. NPR-28148: CQ-4259681용 핫픽스
* Outlook 보낸 편지함 및 받은 편지함 폴더에 첨부 파일이 있는 메시지를 열 수 없습니다. NPR-28559: CQ-4217072용 핫픽스

#### Sites {#sites-5}

* AEM 6.3에서 버전 삭제를 실행하면 로그에 경고가 지속해서 반복 표시됩니다. NPR-27750: CQ-4206870용 핫픽스
* 스타일 플러그인은 리치 텍스트 편집기 전체 화면 모드에서 지원되지 않습니다. NPR-27622: CQ-4258674용 핫픽스
* 콘텐츠 프레임이 editor.js에 로드된 후에는 `loaderPromises` 목록이 지워지지 않습니다. NPR-27768: CQ-4205337용 핫픽스
* 상위 구성 요소에 설정하지 않고 중첩된 Parsys에 템플릿 정책을 설정할 수 없습니다. NPR-27987: CQ-4246095용 핫픽스
* 구성 요소 브라우저는 사용자 입력을 삭제하지 않으므로 JavaScript 오류가 발생할 수 있습니다. NPR-27986: CQ-4247590용 핫픽스
* 사용자가 콘텐츠 조각을 편집하려고 하면 페이지가 공백으로 표시됩니다. NPR-27669
* 사용자가 주석을 클릭하면 주석 강조 표시가 사라집니다. BPR-27196: CQ-4254423용 핫픽스

#### 통합 {#integration-1}

* ResourceResolver는 Target 구성 요소에 대해 여러 도메인을 확인하지 않습니다. NPR-28265: CQ-107847용 핫픽스
* 작업이 표시되므로 LiveCopy 상속 취소가 대상 컨테이너에서 제대로 작동합니다. NPR-28129: CQ-4259813용 핫픽스

#### 복제 {#replication-1}

* DispatcherFlushRules가 6.3.3.1에서 복제를 중단합니다. NPR-28150: CQ-4261401용 핫픽스

#### 캠페인 - 타겟팅 {#campaign-targeting-1}

* TargetedContentManager에서 NullPointerException이 발생합니다. CQ-4263485용 핫픽스

#### 소셜 - SCORM {#social-scorm}

* 플레이어에서 SCORM(Shareable Content Object Reference Model) 클라우드에 대한 참조를 제거합니다. CQ-4260779용 핫픽스

#### DAM - 일반 {#dam-general}

* 링크 공유 이메일을 통해 다운로드하면 빈/손상된 zip이 반환됩니다. CQ-4259686용 핫픽스

#### `MAC` - Test&amp;Target 통합 {#mac-test-target-integration}

* Target 구성 요소 구성 옵션은 기본 대상자를 제외한 대상자에 사용할 수 없습니다. CQ-4261370용 핫픽스

#### 번역 {#translation-1}

* MS® Translator를 API v3.0으로 업그레이드하면 AEM 6.3에서 MS® Translator 서비스를 지원합니다. NPR-28365: CQ-4259096용 핫픽스

### Forms {#forms-5}

### Forms 추가 기능 패키지 {#forms-add-on-package-5}

#### Forms - 워크플로 {#forms-workflow-1}

* HTML5 작업 공간에서 PDF 양식을 렌더링할 수 없습니다. NPR-28059: CQ-4260373용 핫픽스

#### Forms - Acrobat 서비스 {#forms-document-services-2}

* Admin Console의 정책 세트 보기에 나열된 처음 1000개 이외의 정책 세트를 볼 수 없습니다. NPR-28060, NPR-26047: CQ-4249865용 핫픽스
* `java.lang.IllegalArgumentException message:No enum constant com.adobe.internal.pdfm.docbuilder.signature.PathValidationFailureReason.SIGNED_IN_FUTURE`라는 이름의 예외가 발생하여 단기 프로세스가 완료되지 않습니다. NPR-28652

#### Forms - 적응형 양식 {#forms-adaptive-forms}

* 드롭다운 목록에서 항목을 추가 또는 제거하면 확인란 항목 선택 시 업데이트되지 않습니다. NPR-28224: CQ-4252834용 핫픽스

### Forms - JEE 설치 관리자 {#forms-jee-installer-4}

* AEM Forms JEE 설치 관리자에는 새 수정 사항이 없습니다.

### 6.3.3.3에 포함된 OSGi 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-2}

AEM 6.3.3.3에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/6333_bundle_list.txt)

AEM 6.3.3.3에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/content_package_list_6333.txt)

### 누적 수정 팩 6.3.3.2 {#cumulative-fix-pack-6}

AEM 누적 수정 팩 6.3.3.2은 2018년 9월, AEM 6.3 서비스 팩 3(6.3.3.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.3.2는 AEM 6.3 서비스 팩 3에 종속됩니다. 따라서 AEM 6.3 서비스 팩 3을 설치한 후 AEM 누적 수정 팩 6.3.3.x 패키지를 설치해야 합니다. 설치 지침은 AEM 6.3 서비스 팩 3의 릴리스 정보를 참조하십시오.

AEM 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.15으로 업데이트되었습니다.
* 자산 폴더의 규칙 탭 및 탭 적용에 대한 지원이 폴더 메타데이터 스키마에 추가되었습니다.
* 게시할 때 그룹 목록 페이지에 대한 페이지 매김 지원을 사용하도록 설정되었습니다.
* 알림 unreadCount를 임의 수로 구성하도록 설정되었습니다. 기본값은 20입니다.
* 외부 링크 확인의 수정 사항입니다.

#### 자산 {#assets-6}

* 동적 드롭다운 목록에서 계단식 드롭다운이 지원되지 않습니다. NPR-27044; CQ-4252564용 핫픽스
* ExpiryNotification 기능을 사용하도록 쿼리가 개선되었습니다. NPR-26999: CQ-4251188용 핫픽스
* 규칙이 메타데이터 스키마에서 폴더 메타데이터 스키마로 이전됩니다. NPR-27771: CQ-4257737, CQ-4257735, CQ-4259822용 백포트
* 자산 참조 조정으로 Sling ResourceCollections의 일부인 자산에 대한 참조를 업데이트하지 못했습니다. NPR-26759: CQ-4252605용 핫픽스
* 링크 공유 이메일을 통해 다운로드하면 비어 있거나 손상된 zip 파일이 반환됩니다. NPR-27997: CQ-4259686용 핫픽스
* 하이브리드 비디오 인코딩이 완료되지 않고 썸네일이 생성되지 않습니다. NPR-27122: CQ-4255080용 핫픽스

#### Sites {#sites-6}

* 상위 페이지를 일시 중단하면 누락된 페이지에서 cq:LiveRelationship mixin 유형이 제거됩니다. NPR-26996: CQ-4254113용 핫픽스
* (외부 링크 확인) 내부 링크는 개별 페이지에서 끊어진 것으로 표시되지만, 외부 링크에 대해 작동하지 않습니다. NPR-27481: CQ-4257780용 핫픽스
* 다른 페이지 속성을 편집할 때 클라우드 서비스 구성 상속이 끊어집니다. NPR-27311: CQ-4256785용 핫픽스
* Foundation Forms와 함께 핵심 구성 요소 양식을 사용할 때 Null 포인터 예외를 발생시킵니다. NPR-27333: CQ-4249176용 핫픽스
* 리치 텍스트 편집기가 빈 alt 태그를 제거합니다. NPR-26938: CQ-4253267용 핫픽스
* (클래식 UI) 선택에 성능 문제가 있습니다. 드롭다운이 여러 개 있는 경우 리스너가 변경됩니다. NPR-27115: CQ-4237215용 핫픽스
* 리치 텍스트 편집기를 여러 필드와 결합하면 확인되지 않은 TypeError: fieldAPI.getName이 foundation.js에서 함수가 아님 오류가 발생합니다. NPR-27146: CQ-4253155, CQ-4259967용 핫픽스
* Safari 브라우저에서 라디오 버튼을 클릭할 때에도 포커스/커서가 리치 텍스트 편집기에 남아 있습니다. NPR-27144: CQ-4249635용 핫픽스
* 사용자가 콘텐츠 조각을 편집하려고 하면 페이지가 공백으로 표시됩니다. NPR-27669
* 경험 조각에 대한 버전을 작성할 수 없습니다. NPR-27689: CQ-4259009용 핫픽스

#### 통합 {#integration-2}

* com.day.cq.personalization.impl.BrandsRetriever가 사용 가능한 브랜드를 수집하도록 전체 트리를 안내합니다. NPR-27060: CQ-4255790용 핫픽스
* `cq:actions`는 타겟팅된 구성 요소에 대해 고려되지 않습니다. NPR-27616: CQ-4257497용 핫픽스

#### 슬링 {#sling}

* data-sly-use가 동일한 이름의 클래스와 함께 사용되는 경우 컴파일할 수 없는 코드가 생성됩니다. NPR-27282: Sling-7581용 핫픽스

#### 상거래 {#commerce-1}

* Apache Felix Http Jetty 4.0.6으로 업데이트하십시오. NPR-26472: Granite-22916용 핫픽스

#### DAM - DM 클라이언트 {#dam-dm-client}

* Dynamic Media 구성 요소에 중단점을 지정하면 이미지가 표시되지 않습니다. CQ-4256168용 핫픽스

#### DAM - DMServices {#dam-dmservices}

* 관련 비디오가 포함된 MixedMediaSet가 제대로 동기화되지 않습니다. CQ-4251650용 핫픽스
* 비디오가 혼합 미디어 집합용 뷰어 사전 설정 편집기에서 재생되지 않습니다. CQ-4251442용 핫픽스

#### DAM - 일반 {#dam-general-1}

* SP3 패치를 적용하면 콘텐츠 조각 모델에 대한 링크가 누락됩니다. CQ-4259029용 핫픽스

#### DAM - UI {#dam-ui}

* SP3 설치 후 폴더 메타데이터 스키마 UI가 중단됩니다. CQ-4257737용 핫픽스

#### 커뮤니티 {#communities-5}

* 게시할 때 그룹 목록에 대한 페이지 매김을 추가합니다. NPR-26953: CQ-4246525용 핫픽스
* 읽지 않은 횟수 알림은 21 이상으로 설정할 수 없습니다. NPR-27496: CQ-4252829용 핫픽스
* 사용자 구독 수가 1,000개로 제한됩니다. NPR-27615: CQ-4254689용 핫픽스
* 포럼에서 이미지(예: .pdf) 이외의 첨부 파일을 업로드할 때 오류가 관찰되었습니다. NPR-27375: CQ-4257753용 핫픽스
* 행 클릭 시 답글에 대한 링크가 작동하지 않습니다. NPR-24556: CQ-4256138용 핫픽스
* UGC 삭제 시 UGC에 대한 관계가 삭제되지 않습니다. NPR-27631: CQ-4258706용 핫픽스
* 커뮤니티가 DSRP(데이터베이스 저장소 리소스 제공자)를 사용하여 설정된 경우 키워드 검색 시 주소값으로 검색할 수 없습니다. NPR-27652: CQ-4253261용 핫픽스
* 삭제 확인 후 이미지에서 휴지통 아이콘을 클릭하면 첨부 파일이 영구적으로 제거됩니다. NPR-27340: CQ-4255150용 핫픽스
* 포럼 게시물과 답글은 두 번째 페이지 상단에 추가되고, 새로 고치면 게시물이 첫 번째 페이지 상단의 올바른 위치로 이동됩니다. NPR-27341: CQ-4247338용 핫픽스
* 지원 Scorm 리소스 완료 상태 레이블이 UI에 빈 상태로 표시됩니다. NPR-27152: CQ-4249994용 핫픽스
* **권한이 있는 멤버 허용**&#x200B;을 활성화하는 경우 권한이 있는 멤버가 커뮤니티 멤버인 사용자만 작성할 수 있어야 합니다. NPR-27901: CQ-4251235용 핫픽스

#### 지속성 {#sustenance}

* 패키지 관리자 활동 로그는 별도의 로그 파일에 추출해야 합니다. NPR-27323: Granite-14866용 핫픽스

#### 번역 {#translation-2}

* 번역 미리보기가 we.retail 샘플 콘텐츠에서 작동하지 않습니다. NPR-27170: CQ-4241179용 핫픽스

* 사전 대응형 platform.login 수정 사항입니다. NPR-26961
* 페이지 속성의 저장 후 닫기가 Tomcat에서 AEM WAR의 해당 페이지로 돌아가지 않습니다. NPR-27567: Granite-23671용 핫픽스

* sourceEdit 기능이 저장되면 입력한 텍스트가 손실됩니다. CQ-4259273용 핫픽스

### Forms {#forms-6}

### Forms 추가 기능 패키지 {#forms-add-on-package-6}

#### Forms - 문서 보안 {#forms-document-security-1}

* JEE 클라이언트 SDK에 동시성 문제가 발생합니다. NPR-27572: CQ-4247156용 핫픽스

#### Forms - Acrobat 서비스 {#forms-document-services-3}

* WebSphere®에서 SOAP를 기반으로 한 양식 데이터 모델을 만들 수 없습니다. NPR-27692: CQ-4253702용 핫픽스

#### Forms - 적응형 양식 {#forms-adaptive-forms-1}

* AEM Forms에 XML 삽입 취약성이 있습니다. NPR-27863: CQ-4257315용 핫픽스
* AEM Sites 페이지에 잘못된 양식이 구성되고 “양식이 페이지의 전체 폭을 가림” 확인란이 선택된 경우 AEM Forms 컨테이너 구성 요소가 표시되지 않습니다. NPR-25972: CQ-4239287, CQ-4249133용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-5}

#### Foundation JEE {#foundation-jee-1}

* WebSphere®에서 SOAP를 기반으로 한 양식 데이터 모델을 만들 수 없습니다. NPR-27692: CQ-4253702용 핫픽스

#### OSGi 번들 및 콘텐츠 패키지가 포함됨 {#osgi-bundles-and-content-packages-included}

AEM 6.3.3.2에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/63332bundle_list.txt)

AEM 6.3.3.2에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/6332content_package.txt)

### 누적 수정 팩 6.3.3.1 {#cumulative-fix-pack-7}

AEM 누적 수정 팩 6.3.3.1은 2018년 9월, AEM 6.3 서비스 팩 3(6.3.3.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.3.1은 AEM 6.3 서비스 팩 3에 종속됩니다. 따라서 AEM 6.3 서비스 팩 3을 설치한 후 AEM 누적 수정 팩 6.3.3.x 패키지를 설치해야 합니다. 설치 지침은 [AEM 6.3 서비스 팩 3](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)의 릴리스 정보를 참조하십시오.

**AEM 누적 수정 팩**&#x200B;의 주요 사항은 다음과 같습니다.

* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.14으로 업데이트되었습니다.
* 설명 및 검색의 성능이 향상되었습니다.
* 기본값에 대한 FormData 처리 문제가 해결되었습니다.
* 양식 빌더가 최신 Handlebars 버전으로 업그레이드되었습니다.
* 대화 상자 모드에 RTE 편집 구성에 대한 구성 서블릿이 추가되었습니다.
* 복합 필드에 대한 지원이 추가되었습니다.
* 편집 대화 상자에 대한 콘텐츠 정책으로 리치 텍스트 편집기의 도구 모음 항목이 활성화/비활성화되었습니다.

#### 자산 {#assets-7}

* IDS 분리를 활성화한 상태에서 DAM 자산 업데이트 워크플로가 참조를 더는 연결하지 않습니다. NPR-26135: CQ-4250933용 핫픽스
* 보관 해제 단계에서 생성된 아카이브를 %로 이름이 지정된 폴더로 압축을 풀면 열리지 않습니다. NPR-26275: CQ-4251482용 핫픽스
* 작은따옴표 문자로 인해 메타데이터가 업데이트되지 않습니다. NPR-26808: CQ-4254305용 핫픽스
* (Omnisearch) 컬렉션 내에서 검색할 때 성능 문제가 발생합니다. NPR-26714: CQ-4253408용 핫픽스
* 텍스트 내에 “OR” 문자가 있는 전체 텍스트 검색에서 GQLConverter를 사용하면 잘못 처리됩니다. NPR-26564: CQ-4247362용 핫픽스
* 다중 테넌트에서 자산 링크를 공유하면 잘못된 URL을 형성하는 테넌트 ID가 앞에 추가됩니다. NPR-26482: CQ-4253540용 핫픽스
* Dynamic Media 클라우드 구성 UI에서 “회사 루트 폴더 경로”를 비활성화합니다. NPR-26361: CQ-4249505용 핫픽스
* .mos RAW 파일을 수집하는 데 너무 오래 걸립니다. NPR-26296: CQ-4250661용 핫픽스
* 자산 링크 공유에서는 숫자 사용자 ID를 사용하는 내부 사용자를 둘 이상 추가할 수 없습니다. NPR-26206: CQ-4251466용 핫픽스
* deflate64 알고리즘으로 압축된 zip 파일이 손상됩니다. NPR-26793: CQ-4253995용 핫픽스
* 썸네일 생성 프로세스가 복잡한 PDF 파일에 대해 올바르게 작동하지 않아 썸네일에서 이미지 일부가 누락됩니다. NPR-26057: CQ-4250944용 핫픽스
* 썸네일 생성 시 힙 메모리 사용 문제가 발생합니다. NPR-25545: CQ-4246960용 핫픽스
* 자산에 관계를 많이 만들면 오류가 발생합니다. NPR-26309: CQ-4250708용 핫픽스
* **렌디션 삭제** 옵션이 작동하지 않으며 “삭제할 대상이 없습니다” 오류가 발생합니다. NPR-26007: CQ-4213414용 핫픽스
* 다중값 필드에 대한 기본값을 삭제할 수 없습니다. NPR-25116: CQ-4247856용 핫픽스
* (DM 하이브리드) 카탈로그 복제가 Dynamic Media를 사용한 AEM 6.3.2에 대해 중단됩니다. NPR-26406: CQ-4251306용 핫픽스

#### Sites {#sites-7}

* Sites 수정 사항에 대한 사전 대응 백포트입니다. NPR-26963
* 제목 및 이름의 대/소문자 유형에 차이가 있으면 태그가 두 번 생성됩니다. NPR-26877: CQ-4254134용 핫픽스
* 정책에 따라 편집 대화 상자의 리치 텍스트 편집기 기능이 제어되지 않습니다. NPR-27059, NPR-26750: CQ-4241130용 핫픽스
* 클라이언트 컨텍스트 segment.js 캐싱과 비캐싱 질문입니다. NPR-26622: CQ-4253486용 핫픽스
* 하위 규칙에 대해 세그먼트 규칙(/etc/segmentation)을 활성화하면 게시가 중단됩니다. NPR-26601: CQ-4253588용 핫픽스
* “특수 문자”를 추가하면 리치 텍스트 편집기 대화 상자가 맨 위로 스크롤됩니다. NPR-26435: CQ-4249869용 핫픽스
* (Touch UI) 전체 화면에서 부동 대화 상자로 전환하는 동안 도구 모음을 여러 리치 텍스트 편집기에서 사용할 수 없습니다. NPR-25652: CQ-4206008용 핫픽스
* 다중 페이지 시작을 홍보하면 각 페이지에 대한 여러 버전이 작성됩니다. NPR-26810: CQ-4254663용 핫픽스
* 구조화된 콘텐츠 조각 모델 태그 필드는 태그 이동 작업을 반영하지 않습니다. NPR-26801: CQ-4251805용 핫픽스
* (Touch UI) 블루프린트에서 페이지 이름을 바꾼 후에는 페이지 편집기에서 하위 페이지 게시 취소가 작동하지 않습니다. NPR-26774: CQ-4254175용 핫픽스
* 게시되지 않은 페이지가 참조에서 작동하지 않습니다. NPR-26749: CQ-4254372용 핫픽스
* Live Copy로 변형을 작성하려면 사용자가 페이지를 새로 고쳐서 반영해야 합니다. NPR-26663: CQ-4254328용 핫픽스
* (클래식 UI) 페이지 속성으로 돌아간 썸네일 이미지는 더 이상 상속을 사용하지 않고 사이트 관리자 및 사이드 킥에서 표시되지 않으며 공백으로 표시됩니다. NPR-26562: CQ-4252346용 핫픽스
* 페이지 버전이 생성되고 비교가 트리거되면 /content/versionhistory의 노드가 블루프린트의 라이브 카피 목록에 나열됩니다. NPR-26506: CQ-4243957용 핫픽스
* 경험 조각 관리 편집기의 URL은 오버레이를 허용하지 않습니다. NPR-26318: CQ-4252156용 핫픽스

#### 플랫폼 {#platform}

* 테스트 이벤트가 있는 ReplicationEventListener에서 세션 누출이 발생했습니다. NPR-25937: CQ-4251090용 핫픽스
* 복제에서 OAuth에 만료된 토큰을 사용하여 여러 오류가 발생합니다. NPR-25894: GRANITE-22388용 핫픽스

#### 통합 {#integration-3}

* AEM에 임베드된 TSDK는 호환되지 않는 템플릿 사용으로 인해 Handlebars 4로의 업그레이드가 중단됩니다. NPR-26699: CQ-4248974용 핫픽스
* 새 자산으로 페이지를 게시하면 알림 없이 게시 인스턴스에서 하위 페이지가 비활성화됩니다. NPR-24869: CQ-4247832용 핫픽스
* 복제에서 OAauth에 만료된 토큰을 사용합니다. NPR-25984: Granite-22388용 핫픽스

#### 복제 {#replication-2}

* HTTP 전송 시 열려 있는 세션이 누출될 수 있습니다. Granite-17434용 핫픽스
* 여러 복제 에이전트가 동시에 액세스하면 액세스 토큰 노드에 액세스하는 도중 로그에 예외가 발생합니다. NPR-26964: GRANITE-23276, Granite-23155용 핫픽스

#### ContextHub {#contexthub}

* 파일에는 `coral.js` 취약한 버전의 라이브러리가 포함되어 있습니다 `handlebars.js`. CQ-4255377용 핫픽스

#### DAM - DM 클라이언트 {#dam-dm-client-1}

* 이미지 자산의 사본을 삭제하면 원본 이미지 자산을 사용할 수 없게 됩니다. CQ-4251648용 핫픽스
* S7 서버에서 추가 이미지 콘텐츠가 중복 다운로드됩니다. CQ-4248770용 핫픽스

#### Granite {#granite}

* AEM OAuth 공급자가 대/소문자를 구분하지 않는 검색을 수행하지 않습니다. NPR-26133: GRANITE-22650용 핫픽스
* 패키지 유효성 검사기는 CFP/SP에 포함된 패키지의 유효성을 검사하지 않습니다. NPR-26775: Granite-22825용 핫픽스

#### 커뮤니티 {#communities-6}

* 검색 결과에 구분 기호 문제가 있습니다. NPR-27051: CQ-4248939용 핫픽스
* Adobe 저장소 리소스 제공자에서 드롭다운 값을 댈러스에서 버지니아로 변경합니다. NPR-26936: CQ-4254434용 핫픽스
* SocialTagManager에서 현지화된 제목 검색을 지원합니다. NPR-26932: CQ-4250276용 핫픽스
* 포럼 게시물을 작성하는 도중 첨부 파일 이미지에 썸네일이 표시되지 않습니다. NPR-26380: CQ-4253105용 핫픽스
* Word 플러그인에서 붙여넣기를 수행하면 두 개 이상의 이미지가 로드되지 않습니다. NPR-26728: CQ-4253638용 핫픽스
* 관리 페이지에서 콘텐츠를 필터링할 수 없습니다. NPR-26697: CQ-4213766용 핫픽스
* (보안 취약성) 잘못된 JWT 구성으로 인해 계정이 도용되었습니다. NPR-26440: CQ-4253314용 핫픽스
* Adobe 저장소 리소스 제공자의 데이터를 검색하는 속도가 느립니다. NPR-26237: NPR-24152용 핫픽스
* 비공개 메시지 작성 페이지가 비정상적이고 느립니다. NPR-26120: CQ-4250923용 핫픽스
* “모두 읽은 상태로 표시” 알림이 페이지를 새로 고치지 않고 처음 10개의 메시지만 읽지 않음으로 렌더링합니다. NPR-27036: CQ-4254058용 핫픽스
* 커뮤니티 댓글 섹션 페이지 매김 클릭 및 페이지 로드 동작입니다. NPR-27030: CQ-4251228용 핫픽스
* (포럼 검색) 뒤로 버튼 사용 시 페이지를 건너뛰고 다시 forum.html로 전송합니다. NPR-26949: CQ-4254804용 핫픽스
* 읽지 않은 알림이 21 이상으로 늘어나지 않습니다. NPR-26947: CQ-4251251용 핫픽스
* (SearchScheduledPosts 작업) ConfigMgr에 활성화/비활성화 스위치를 추가합니다. NPR-26924: CQ-4250463용 핫픽스
* 할당 페이지에서 스크롤할 때 Tomcat 컨텍스트(/aempublish) 경로가 삭제됩니다. NPR-26919: CQ-4254345용 핫픽스
* 그룹 및 멤버 생성 중 NullPointerException이 발생합니다. NPR-26778: CQ-4248095용 핫픽스
* 중재자 고정 해제 및 포함 해제된 콘텐츠가 MySQL SRP(단일 책임 원칙)와 호환되지 않습니다. NPR-26767: CQ-4251520용 핫픽스
* 특정 문자에서 검색 기능 문제가 발생합니다. NPR-26726: CQ-4247744용 핫픽스
* 관리 UI 및 지원 리소스에 딥 링크를 사용합니다. NPR-26705: CQ-4251381용 핫픽스
* 포럼 구성 요소를 검색하는 동안 문제가 발생합니다. NPR-26577: CQ-4251303용 핫픽스
* 커뮤니티 메시징에서 이름과 성을 함께 검색하면 예상 결과가 반환되지 않습니다. NPR-26377: CQ-4253150용 핫픽스
* 답글 제거 시 페이지 매김이 업데이트되지 않습니다. NPR-26327
* 게시물 삭제가 수행되지만, 콘솔에 오류가 발생하고 게시물이 UI에 계속 표시됩니다. NPR-26292: CQ-4252803용 핫픽스
* 페이지 매김이 동적으로 업데이트되지 않고 댓글 목록이 점점 더 길어집니다. NPR-26145: CQ-4251586용 핫픽스
* 사용자 수천 명이 포함된 그룹에 그룹 설정이 로드되지 않습니다. NPR-25642: CQ-4238426용 핫픽스
* 컨텍스트 경로에 대해 카탈로그 리소스 플레이어가 실패했습니다. NPR-25640: CQ-4238426용 핫픽스
* (포럼 검색) - 게시물이 많은 스레드에 대한 페이지 매김된 링크가 알림에서 작동하지 않습니다. CQ-4254202용 핫픽스
* Firefox에서는 관리 콘솔에 5개의 항목만 표시됩니다. CQ-4254128용 핫픽스
* 사이트 생성 중에 그룹이 표시되지 않습니다. NPR-27148: CQ-4251788용 핫픽스
* 역할 설정에 그룹 및 멤버를 추가하고 블로그 기능에 권한이 있는 멤버를 허용하는 중 Null 포인터 예외가 발생합니다. NPR-21732, NPR-27176: CQ-4255909용 핫픽스
* 역할 설정에서 사이트를 편집하고 멤버를 추가하면 null 포인터 예외가 발생합니다. NPR-27132: CQ-4255909용 핫픽스

#### 사용자 인터페이스 {#user-interface}

* 사전 대응형 플랫폼 로그인 수정 사항입니다. NPR-26961
* (Multifield) 합성 항목에 사용자 정의 이름을 사용할 수 있습니다. NPR-26493: Granite-20568용 핫픽스
* 페이지를 붙여넣은 후 새로 고칠 때까지 열 보기가 업데이트되지 않습니다. NPR-26030: CQ-4236346용 핫픽스
* 사전 대응형 granite.ui.commons 수정 사항입니다. NPR-26960
* 사전 대응형 granite.ui.content 수정 사항입니다. NPR-26959
* 사전 대응형 CQ/experience 로그 수정 사항입니다. NPR-26943
* 사전 대응형 Foundation UI 백포트입니다. NPR-26942
* (IE11) 음수값을 입력할 때 “NaN”이 숫자 필드에 표시됩니다. NPR-26701: CQ-100826용 핫픽스
* (Coral. Multifield) 중첩된 multi-fields에서 잘못된 템플릿을 사용하여 항목을 작성합니다. NPR-25649: CUI-6743용 핫픽스
* Granite coralui2 및 coralui3 clientlibs를 업데이트하여 빌드에서 Handlebars를 제거합니다. NPR-25606: Granite-22116용 핫픽스

### Forms {#forms-7}

### Forms 추가 기능 패키지 {#forms-add-on-package-7}

#### Forms - 문서 보안 {#forms-document-security-2}

* 서버 로그에 비활성 상태의 키에 대한 주체 키 롤오버 예외가 발생했습니다. NPR-26748: CQ-4253705용 핫픽스
* 문서 보안의 워터마크 설정을 작성하거나 편집할 수 없습니다. NPR-26267, NPR-26129: CQ-4250234용 핫픽스

#### Forms - Acrobat 서비스 {#forms-document-services-4}

* PDF/A 유효성 검사가 “PDF/A 확인”에서 유효한 것으로 표시되지 않습니다. NPR-25934: CQ-4248558용 핫픽스

#### Forms - 인터랙티브 커뮤니케이션 {#forms-interactive-communication}

* 편집 가능한 모듈을 편집하고 저장한 후 PDF 미리보기를 열거나 닫으면 편지의 PDF 및 HTML 미리보기가 계속 표시됩니다. 두 미리보기가 동일한 창에서 작동합니다. NPR-26770: CQ-4253217용 핫픽스

#### Forms - 워크플로 {#forms-workflow-2}

* 작업 영역이 간헐적으로 중단되고 시작 지점을 반복적으로 표시합니다. NPR-26461: CQ-4253439용 핫픽스
* 작업 이름에 중괄호가 사용되는 경우 로그에서 ESAPI 예외가 발생합니다. CQ-4256627용 핫픽스
* 시작 지점과 연결된 미리 채워지지 않은 적응형 양식 또는 양식 세트가 열려 있으면 Null 포인터 예외가 발생합니다. CQ-4256124용 핫픽스
* 전역 설정을 사용하여 이메일을 보낼 수 없습니다. NPR-26163: CQ-111110용 핫픽스
* axis.jar 파일을 적용한 후 작업 영역을 열 수 없습니다. NPR-26131: CQ-4251126용 핫픽스
* 새로 고침 버튼이 서버의 최신 데이터를 적응형 양식에 동기화하지 못했습니다. CQ-4255670용 핫픽스
* 관리자 UI에서 검색 템플릿을 설정한 다음 이 설정을 사용하여 AEM Forms 작업 영역에서 작업을 검색하는 경우 예외가 발생합니다. CQ-4255649용 핫픽스
* 이름에 괄호 기호를 사용한 애플리케이션의 프로세스 추적 세부 사항은 HTML 작업 영역에 표시되지 않습니다. CQ-4242101용 핫픽스
* HTML 작업 영역의 환경 설정 화면에서 변경 사항을 저장하면 예외가 발생합니다. CQ-4241485용 핫픽스
* 대량 승인이 최신 JEE 설정에서 해제됩니다. CQ-4241486용 핫픽스
* 최신 6.4 JEE 서버에서 작업/시작 지점의 초안이 실패합니다. CQ-4241484용 핫픽스
* 세션을 초기화하려면 Date.toString() 대신 Date().getTime().toString 매개변수를 설정합니다. CQ-4241483용 핫픽스
* /lc/ws를 여는 동안 HTML 매개변수에서 취약한 문자 예외가 관찰되었습니다. CQ-4241481용 핫픽스

#### 취약성 {#vulnerability-1}

* Forms Manager의 메모 탭에 저장된 XSS(크로스 사이트 스크립팅)에 취약성이 발견되었습니다. NPR-27157: CQ-4255556용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-6}

#### Foundation JEE {#foundation-jee-2}

* Enterprise Security API에 대한 코드 검토입니다. CQ-4255638용 핫픽스
* esapi.properties를 WAS9의 classloader 리소스로 로드하지 못했습니다. CQ-4255631용 핫픽스
* 도메인 구성 중에 인증 추가를 클릭하면 오류가 발생합니다. CQ-4255634용 핫픽스
* Forms JEE가 PKCS#11 상호 인증을 지원합니다. NPR-21372
* 코어의 정적 코드 분석에 보고된 문제가 수정되었습니다. CQ-104446용 핫픽스
* LCM을 실행하는 동안 adobe.livecycle.weblogic.ear 및 adobe.livecycle.websphere.ear를 배포하지 못했습니다. CQ-4255629, CQ-4255630용 핫픽스
* 애플리케이션 관리에 잘못된 오류 메시지가 있습니다. NPR-23289: CQ-4233163, CQ-4255636용 핫픽스
* 도메인 구성 중에 인증 추가를 클릭하면 오류가 발생합니다. CQ-4255634용 핫픽스

#### Forms - JEE 커넥터 {#forms-jee-connector}

* 커넥터의 정적 코드 분석에 보고된 문제가 수정되었습니다. NPR-22260

#### PDFG 서비스 {#pdfg-service-1}

* LiveCycle에서 AEM 6.2 Forms로 업그레이드하면 로그에 org.jgroups.Message 오류가 발생합니다. NPR-26795: CQ-4220415용 핫픽스
* AEM Forms - 스타일을 마이그레이션하는 동안 오류가 발생합니다. CQ-4251969용 핫픽스
* PDFG의 정적 코드 분석 보고서에 보고된 문제가 수정되었습니다. NPR-23251: CQ-4213930용 핫픽스

#### 6.3.3.1에 포함된 OSGi 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-3}

AEM 6.3.3.1에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/63sp3cfp1bundlelist.txt)

AEM 6.3.3.1에 포함된 콘텐츠 패키지 목록

### 누적 수정 팩 6.3.2.2 {#cumulative-fix-pack-8}

AEM 누적 수정 팩 6.3.2.2는 2018년 4월, AEM 6.3 서비스 팩 2(6.3.2.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩 6.3.2.2는 AEM 6.3 서비스 팩 2에 종속됩니다. 따라서 AEM 6.3 서비스 팩 2를 설치한 후 AEM 누적 수정 팩 6.3.2.x 패키지를 설치해야 합니다. 설치 지침은 [AEM 6.3 서비스 팩 2](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)의 릴리스 정보를 참조하십시오.

**AEM 누적 수정 팩**&#x200B;의 주요 사항은 다음과 같습니다.

* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.11으로 업데이트되었습니다.
* Brand Portal에서 하위 자산 및 다중 페이지 자산 뷰어가 활성화되었습니다.
* 다른 유형의 첨부 파일에 사용할 수 있는 모든 MIME 유형을 지원하도록 필드 유형의 길이가 255로 변경되었습니다.
* 이미지가 업로드 기준을 위반하는 경우 서버에서 구성된 오류 메시지입니다.
* 일별 CQ 메일 서비스에 STARTTLS 지원이 추가되었습니다.
* cq-wcm-content 및 com.adobe.cq.launches.it.serverside의 최신 버전으로 업데이트합니다.
* com.adobe.granite.ui.coralui3-rte를 릴리스된 최신 버전으로 업데이트합니다.
* expressionResolver가 null일 경우 렌더링 조건이 올바른 결과를 반환합니다.
* Coral.ColumnView: shift+클릭에 대한 지원이 추가되었습니다.

### 자산 {#assets-8}

* 자산 폴더 CUG(폐쇄된 사용자 그룹) 필드가 &#39;모든 사람&#39; 그룹을 반환하지 않습니다. NPR-23163: CQ-4239377용 핫픽스
* 저장된 스마트 컬렉션 검색 결과를 검색하면 일부 결과가 반환되지 않습니다. NPR-23243: CQ-4240355용 핫픽스
* (ExpiryNotificationJobImpl) 기존 쿼리의 최적화입니다. NPR-23330: CQ-4205249용 핫픽스
* (메타데이터 프로필) 생성 시 설정된 표준 태그값은 저장 후에 사용할 수 없습니다. NPR-23370: CQ-4235458용 핫픽스
* (Touch UI) JS 오류로 인해 여러 자산을 이동할 수 없습니다. NPR-23395: CQ-4241279용 핫픽스
* 표시된 정보는 다운로드 크기와 일치하지 않습니다. NPR-23418: CQ-4242774용 핫픽스
* 파일 확장자 LSR 및 SKETCH에 대해 추출된 MIME 유형이 올바르지 않아서 잘못된 파일이 다운로드될 수 있습니다. NPR-23644: CQ-4243260용 핫픽스
* (Firefox/Chrome) 자산 공유 페이지에서 자산을 다운로드할 수 없습니다. NPR-23963: CQ-4244391용 핫픽스
* 자산 관리 검색 패싯이 미리보기 후에 검색 패널에서 사라집니다. NPR-23964: CQ-4244410용 핫픽스
* 검색 양식 게시를 취소하면 기본 검색 양식이 완전히 제거됩니다. NPR-23291: CQ-4241382용 핫픽스
* (Brand Portal) 디렉터리 설명에서의 검색은 복제 시 필터링됩니다. NPR-23292: CQ-4241385용 핫픽스
* Brand Portal에 게시 UI 작업을 사용할 수 없습니다. NPR-23293: CQ-4241161용 핫픽스
* Brand Portal에 게시/게시 취소 버튼은 콘텐츠 조각에 사용할 수 없습니다. NPR-23318: CQ-4245086용 핫픽스
* (Brand Portal) 자산이 게시될 때 하위 자산 만들기를 활성화합니다. NPR-23331: CQ-4242018용 핫픽스
* Dynamic Media 요청에서 프록시/HTTP 일반 클라이언트를 사용하지 않습니다. NPR-10727: CQ-45695, CQ-88800용 핫픽스
* DMS7(Dynamic Media S7)의 단일 렌디션 MP4 비디오 자산에 주석을 추가할 수 없습니다. NPR-22046: CQ-4215912용 핫픽스
* EmbedXMP 데이터가 Tiff 피라미드 생성 프로세스에 대해 항상 “활성”으로 설정됩니다. NPR-22903: CQ-4234498용 핫픽스
* 큰 이미지 사전 설정 수에 동적 렌디션 표시/선택 문제가 발생합니다. NPR-23151: CQ-4217511용 핫픽스
* Dynamic Media 인코딩 비디오 - 수정/시작 관리자 다시 업로드 시 문제가 발생합니다. NPR-23237: CQ-4240260용 핫픽스
* Dynamic Media S7에서 HTTP 전달자에 대한 프록시 처리 수정 사항입니다. NPR-24001: CQ-244140용 핫픽스

### Sites {#sites-8}

* QueryBuilder 불일치로 인해 6.2와 6.3의 xPath 변환이 서로 다릅니다. NPR-23245: CQ-4240396용 핫픽스
* 대화 상자 확장 시 페이지 속성의 썸네일 탭이 작동하지 않습니다. NPR-22844: CQ-4241474용 핫픽스
* Parsys가 에뮬레이터 디바이스 프레임 폭을 나누고 여기에 추가된 구성 요소를 자릅니다. NPR-22926: CQ-4238224용 핫픽스
* 여러 시작을 실행할 때 시작이 작성자에서 홍보되지만, 변경 사항은 복제 권한이 없으므로 게시 서버에 복제되지 않습니다. NPR-22934: CQ-4234746용 핫픽스
* 다른 세션의 다른 사용자가 첫 번째 세션에서 사용자가 잠근 페이지를 수정할 수 있습니다. NPR-23057: CQ-4199017용 핫픽스
* 목록 보기에서 재정렬 가능 옵션을 수정했습니다. NPR-23065: CQ-4239321용 핫픽스
* (페이지 편집기) 이미지 구성 요소의 이미지가 대화 상자를 다시 열 때 사라집니다. NPR-23156: CQ-4239978용 핫픽스
* 템플릿 편집기에 최대 20개의 템플릿/폴더만 표시되고, 페이지 맨 아래로 스크롤할 때 다른 템플릿/폴더가 로드되지 않습니다. NPR-23185: CQ-4238483용 핫픽스
* (클래식 UI) 페이지를 이동하거나 이름을 변경하는 중에 오류가 발생합니다. NPR-23213: CQ-4240971용 핫픽스
* ContextHub 세그먼트를 편집/생성할 수 없습니다. NPR-23218: CQ-4226948용 핫픽스
* (리치 텍스트 편집기) - 바꾸기 작업이 단어의 형식을 변경합니다. NPR-23271: CQ-4239677용 핫픽스
* XF 변형에 대한 블루프린트 탭에서 롤아웃 버튼이 누락되었습니다. NPR-23320: CQ-4240404용 핫픽스
* 사용 중단으로 인해 CUG를 클래식 UI에서 편집할 수 없습니다. NPR-24122: 4241823용 핫픽스
* 원치 않는 콘텐츠 홍보로부터 보호하기 위한 사전 대응형 수정 사항입니다. NPR-24387: 4244993용 핫픽스
* 약 80개의 조각이 자산의 폴더에 추가되면 타임라인 콘솔에서 워크플로가 트리거될 때 오류가 발생합니다. NPR-23393; CQ-4211216용 핫픽스
* 콘텐츠 파인더의 리치 텍스트 편집기 대화 상자로 이미지를 끌어다 놓을 수 없습니다. NPR-23403: CQ-4242094용 핫픽스
* AEM 6.0에서 AEM 6.2로 구성 요소를 마이그레이션하는 중 &#39;올바르지 않은 재귀 선택기 값&#39; 오류가 발생합니다. NPR-23532: CQ-4241258용 핫픽스
* (리치 텍스트 편집기) 도구 설명에 읽을 수 있는 플러그인 이름 대신 플러그인의 변수 이름이 표시됩니다. NPR-23550: CQ-4243269용 핫픽스
* 모바일/태블릿 버전에서 필수 선택 드롭다운이 있는 대화 상자를 저장할 수 없습니다. NPR-23904: CQ-4243096용 핫픽스
* 6.3.2.1 설치 후 스타일 시스템 옵션이 모든 페이지에 표시됩니다. NPR-23972: CQ-4244394용 핫픽스
* 사용 중단으로 인해 CUG를 클래식 UI에서 편집할 수 없습니다. NPR-24122: 4241823용 핫픽스
* 원치 않는 콘텐츠 홍보로부터 보호하기 위한 사전 대응형 수정 사항입니다. NPR-24387: 4244993용 핫픽스
* 자산을 이동했을 때 자산 참조가 업데이트되지 않습니다. NPR-23208: CQ-4239879용 핫픽스

### 플랫폼 {#platform-1}

* 검색 패싯에서 태그 설명을 사용하는 경우 저장하면 스마트 컬렉션에 결과가 표시되지 않습니다. NPR-23401: Granite-21278용 핫픽스
* 보안 수정 사항을 포함하는 clientlib의 jQuery 1.12.4 패치입니다. NPR-24128: Granite-20058용 핫픽스
* 번들이 다시 시작되면 국제화 번역이 업데이트됩니다. NPR-23193: Sling-7190용 핫픽스
* ReplicationEventListener에서 리소스 확인자가 닫히지 않았습니다. NPR-23240: CQ-4241350용 핫픽스
* “Day CQ Mail Service”에서 STARTTLS를 지원합니다. NPR-23941: CQ-4240397용 핫픽스
* JCR 규격 태그 이름이 태그 제목에 따라 자동으로 채워집니다. NPR-24173: CQ-4199411용 핫픽스

### 통합 {#integration-4}

* (Target) XML과 같은 API 유형을 사용할 때 캠페인이 활성화되지 않습니다. NPR-23199: CQ-4240936용 핫픽스****
* 구성 참조 복제가 중간 폴더 구조로 인해 실패합니다. NPR-23485: CQ-4242751용 핫픽스

### 취약성 {#vulnerability-2}

* Salesforce 통합은 SSRF(Server Side Request Forgery)에 취약합니다. NPR-24289: CQ-424527용 핫픽스
* 관리자 UI 프로젝트의 XSS(크로스 사이트 스크립팅)가 연결됩니다. NPR-23272: CQ-4241795용 핫픽스

### WCM - Foundation 구성 요소 {#wcm-foundation-components}

* Foundation 테이블은 저장된 크로스 사이트 스크립팅에 취약합니다. NPR-23214: CQ-4240760용 핫픽스

### 번역 {#translation-3}

* 언어 사본 작성 중에 Live Copy 속성이 삭제되지 않습니다. NPR-23123: CQ-4230641용 핫픽스

### 사용자 인터페이스 {#user-interface-1}

* DatePicker가 숨김 필드에 의해 수동으로 설정된 외부 유형 힌트를 지원하지 않습니다. 이 유형 힌트를 변경하면 변환 오류가 발생합니다. NPR-23371: Granite-21194용 핫픽스
* Coral.ColumnView: shift+클릭을 추가로 지원합니다. NPR-23404: Granite-13338용 핫픽스
* 값이 비어 있는 항목을 선택하면 선택 RT가 유효성을 검사하지 않습니다. NPR-23405: Granite-21283용 핫픽스
* (OMEGA) “기능”을 영어로만 보고합니다. NPR-23990: Granite-21231용 핫픽스
* Coral.Autocomplete API를 수정했습니다. NPR-23516

### Granite {#granite-1}

* Apache HTTP 클라이언트 추적 연결 및 높은 힙 사용률로 인해 AEM 서버가 충돌합니다. NPR-23906: Granite-21056용 핫픽스

### 상거래 {#commerce-2}

* Campaign json 출력에 서블릿 컨텍스트 루트가 포함되지 않습니다. NPR-23733: CQ-4243827용 핫픽스

### 커뮤니티 {#communities-7}

* Communities에서 검색하면 단어가 검색되지 않습니다. NPR-23256: CQ-4240717용 핫픽스
* 커뮤니티 관리자 역할 문제에 대해 그룹을 지정할 수 없습니다. NPR-23317: CQ-4241233용 핫픽스: CQ-4221399
* 유사한 자산 이름으로 리소스를 만드는 데 문제가 있습니다. NPR-23319: CQ-4240700용 핫픽스
* (ContextPath) 커뮤니티 그룹 멤버 목록에서 그룹 멤버를 검색하는 동안 Jetty 구성 및 오류로 인해 주요 메시지 기능이 중단됩니다. NPR-23336: CQ-4241519, CQ-4242080용 핫픽스
* 이미지를 커뮤니티 포럼에 업로드하면 ASRP(Adobe 저장소 리소스 제공자)에 나타나지 않습니다. NPR-23397: CQ-4242497용 핫픽스
* 삭제된 아이디어가 활동에 활성 링크로 표시됩니다. NPR-23406
* 컨텍스트 루트로 실행 중인 AEM에서 imsmanifest.xml을 로드할 수 없습니다. NPR-23483: CQ-4242193용 핫픽스
* 이전 버전의 Handlebars에 보안 취약점이 있습니다. NPR-23518: CQ-4243055용 핫픽스
* 터널 서비스가 작동하지 않습니다. NPR-23543: CQ-4242217용 핫픽스
* Dispatcher 및 sling dynamic을 통해 액세스할 때 커뮤니티 구성 요소에 이를 사용하도록 하는 설정이 포함되는 문제가 발생합니다. NPR-23586: CQ-4242360, CQ-4241522용 핫픽스
* 검색을 통해 많은 결과를 생성하는 검색어를 검색한 다음 새 검색어를 입력할 때 페이징이 재설정되지 않습니다. NPR-23739: CQ-4222593용 핫픽스
* 포럼 구성 요소에서 검색을 수행하는 동안 문제가 발생합니다. NPR-23838: CQ-4243770용 핫픽스
* (Communities 관리 플래그 지정) 플래그가 지정된 메시지의 벌크 허용이 작동하지 않습니다. NPR-23845: CQ-4243962용 핫픽스
* 기본 정렬 순서를 선택했지만 정렬 버튼 텍스트에 기본 선택된 값이 표시되지 않습니다. NPR-23881: CQ-4243375용 핫픽스
* 메시지 오류로 인해 웹 및 메일 알림이 그룹으로 트리거되지 않습니다. NPR-23934: CQ-4242880용 핫픽스
* 플래그 사용자 및 이유에 대한 세부 사항이 DSRP 구성을 사용하여 표시되지 않습니다. NPR-23973: CQ-4243205용 핫픽스
* 플래그가 지정되지 않은 사용자의 플래그 이유가 계속 표시됩니다. NPR-23974: CQ-4243822용 핫픽스
* 이름이 같은 두 개의 파일을 양식 게시에 두 번 첨부하면 서버 오류가 발생합니다. NPR-24166: CQ-4244367용 핫픽스
* DSRP(Database Storage Resource Developer)를 사용하여 15자 이상의 MIME 유형으로 첨부 파일을 저장할 수 없습니다. NPR-24174
* 업로드 기준을 위반하는 이미지를 게시 텍스트로 끌어다 놓으면 서버 오류가 발생하고 일반 오류 메시지가 사용자에게 표시됩니다. NPR-24243
* 여러 AEM Communities 서버측 문제에 대한 수정 사항입니다. NPR-23971: CQ-4243144, CQ-4242145, CQ-4243365, CQ-4244098용 핫픽스
* 여러 Adobe Social 문제에 대한 수정 사항입니다. NPR-24242: CQ-4245054, CQ-4245120, CQ-4245296용 핫픽스

### 캠페인 {#campaign}

* Campaign json 출력에 서블릿 컨텍스트 루트가 포함되지 않습니다. NPR-23733: CQ-4243827용 핫픽스

### MSM {#msm}

* 페이지를 롤아웃할 때 Live Copy에 기본에서 상속된 설정/해제 시간 속성이 표시되지 않습니다. NPR-23873: CQ-4243431용 핫픽스
* LiveCopy 작업이 삭제된 구성 요소의 하위 노드를 무시하지 않습니다. NPR-23058: CQ-4211662용 핫픽스

### 오프로드 {#offloading}

* 처리 후 또는 정기적으로 작업자 인스턴스에서 자산을 정리하기 위한 메커니즘을 요청합니다. NPR-23638: Granite-21337용 핫픽스

## Forms {#forms-8}

### Forms 추가 기능 패키지 {#forms-add-on-package-8}

#### 적응형 양식 {#adaptive-forms-1}

* `ReCaptchaConfigService`를 내부 패키지로 이동합니다. CQ-4217459용 핫픽스
* 숫자 필드에 최소값이 적용되지 않습니다. NPR-23967: CQ-4244830용 핫픽스
* Adobe Sign과 적응형 양식 통합에서 다중 분할된 데이터베이스를 지원합니다. NPR-23383

#### 백엔드 통합 {#backend-integration}

* (FDM) (WebService) WSDL 파서에서 WSDL의 확장 구성을 지원합니다. NPR-23640
* Forms 추가 기능 클라이언트 SDK에 SDLInvokerParams를 포함합니다. NPR-23157

### Forms JEE 설치 관리자 {#forms-jee-installer-7}

#### 프로세스 관리 {#process-management}

* 새 axis.jar 파일을 적용한 후 작업 영역을 열 수 없습니다. NPR-23316
* LiveCycle이 PMAdmin의 XSS에 취약합니다. NPR-23267
* AEM 6.1 Forms로 업그레이드한 후 HTML 작업 공간이 특정 사용자의 작업 목록에 액세스할 때 중지됩니다. NPR-23943

#### 코어 {#core}

* Forms JEE가 PKCS#11 상호 인증을 지원합니다. NPR-21372

#### PDFG 서비스 {#pdfg-service-2}

* TIFF 파일(약 50킬로바이트 크기)을 동시에 처리하는 동안 종이 캡처 서비스가 충돌합니다. NPR-23556

#### Forms Designer {#forms-designer}

* AEM Forms 서버 출력 - 주석에 대한 대체 설명이 없습니다. NPR-22207
* Designer 및 출력 서비스를 통해 생성된 XML 양식에 PDF/UA 지원을 추가합니다. NPR-23132

### 6.3.2.2에 포함된 OSGi 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-4}

AEM 6.3.2.2에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/6_3_2_2_bundle-list.txt)

AEM 6.3.2.2에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/6_3_2_2_content_packagelist.txt)

### 누적 수정 팩 6.3.2.1 {#cumulative-fix-pack-9}

AEM 누적 수정 팩 6.3.2.1는 2018년 4월, AEM 6.3 서비스 팩 2(6.3.2.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

**AEM 누적 수정 팩**&#x200B;의 주요 사항은 다음과 같습니다.

* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.10으로 업데이트되었습니다.
* 클래식 UI에서 Parsys 구성 요소의 렌더링이 개선되었습니다.
* 문자 세트 수정 사항을 포함하도록 Sling 모델 번들이 업데이트되었습니다.
* 모든 자산 유형에 대해 Brand Portal에 게시 비동기를 작성합니다.
* 0.1.15에서 0.1.16으로 coralui-component-richtexteditor.git가 업데이트되었습니다.
* 드롭다운 구성 요소의 표시/숨기기 기능이 수정되었습니다.
* 코어 이미지 구성 요소에 대한 이미지 뒤집기를 사용하도록 설정되었습니다.
* 섹션 속성을 활성화하기 위해 Felix http 번들을 업데이트했습니다.

* 메모리 사용 문제로 인해 Sling 모델에서 cache=true가 제거되었습니다.

### 자산 {#assets-9}

* 자산 폴더 설정에서 제목 또는 썸네일 그림을 변경할 때 폴더의 원래 그룹 및 권한이 무시됩니다. NPR-22171: CQ-4216080용 핫픽스
* UI에 “Brand Portal에 게시하지 못했습니다”라는 잘못된 오류가 표시되지만, 작업이 복제 대기열에 추가되고 자산이 Brand Portal에 게시됩니다. NPR-22179: CQ-4205273용 핫픽스
* (Touch UI) 열 보기의 자산에 대한 기본 업로드 위치입니다. NPR-22465: CQ-4237057용 핫픽스
* `/conf/global`에서 `/conf/mytenant`로 자산 스키마를 복사하려고 하면 AEM에 StackOverflow 오류가 발생합니다. NPR-22489: CQ-4235875용 핫픽스
* 폴더 이름 끝에 있는 후행 공백으로 인해 ZIP 아카이브를 압축 해제하지 못했습니다. NPR-22522: CQ-4238036용 핫픽스
* 자산 제목 열을 사용한 정렬이 검색 결과에 대해 작동하지 않습니다. NPR-22908: CQ-4239076용 핫픽스
* YouTube 비디오에 태그 이름 자체가 아닌 전체 경로로 태그가 지정됩니다. NPR-22976: CQ-4238669용 핫픽스
* 재정렬 가능한 폴더에 있는 폴더를 다시 정렬하면 정렬이 유지되지 않습니다. NPR-23125: CQ-4231761용 핫픽스
* HTTP 504: 공유 링크를 사용하여 컬렉션을 공유하려고 하면 게이트웨이 시간 초과 오류가 발생합니다. NPR-21928: CQ-4234507용 핫픽스
* PDF 자산과 연관된 키워드가 여러 개 있는 경우 PDF 키워드 메타데이터가 제대로 추출되지 않고 잘못 수정됩니다. 이 문제를 해결하기 위해 PDF 자산에 대한 제목 필드 메타데이터 속성이 제거되었습니다. 그러나 메타데이터 스키마를 편집하여 제목 필드에 대한 여러 값 텍스트 필드를 추가할 수 있습니다. NPR-21972: 4215741용 핫픽스****
* 두 개의 팝업이 표시되는 사이에 선택된 폴더가 변경되면 잘못된 자산이 삭제됩니다. NPR-21980: CQ-4233675용 핫픽스
* (DAM) 컬렉션 마법사에 추가하는 중 여러 XSS(크로스 사이트 스크립팅) 취약성이 발생했습니다. NPR-22432: CQ-4327086용 핫픽스
* Safari의 자산에서 Digital Rights Management를 사용할 때 자산 다운로드가 실패합니다. 사용자가 면책조항이 있으며 긴 파일 이름을 사용하는 자산을 다운로드할 수 없습니다. NPR-22747: CQ-4236460 및 CQ-4235274용 핫픽스
* 자산을 Brand Portal에 게시하는 동안 공개 공유를 기본 옵션으로 설정합니다. NPR-21931: CQ-4218816용 핫픽스

### Sites {#sites-9}

* 워크플로 받은 편지함의 새 항목에 페이지 제목 대신 페이지 경로가 표시됩니다. NPR-21634: CQ-4230672용 핫픽스
* 편집 가능한 구조 구성 요소는 편집 시 응답형 격자에 필요한 CSS 클래스 이름을 잃게 됩니다. NPR-21741: CQ-4232374용 핫픽스
* (TouchUI) HTL 구성 요소는 여러 XSS(크로스 사이트 스크립팅) 취약성이 있습니다. NPR-21899: CQ-4232511용 핫픽스
* 콘텐츠 조각 혼합된 미디어 이미지 리소스 유형을 변경할 수 없습니다. NPR-21907: CQ-4233401용 핫픽스
* Touch UI 대화 상자에 대한 RTE 전체 화면이 RTE 플러그인을 숨깁니다. NPR-22034: CQ-4235457용 핫픽스
* (Touch UI) 리치 텍스트 편집기가 &lt;a> 태그에서 ID 이외의 모든 속성을 제거합니다. NPR-22044: CQ-4234133용 핫픽스
* 장기 실행 쿼리(6개 이상)로 인한 여러 누적 Parsys가 AEM을 느리게 만듭니다. NPR-22134: CQ-4233904용 핫픽스
* 이름에 콜론이 있는 노드에 대한 사용 권한을 변경할 수 없습니다. NPR-22136: CQ-4236221용 핫픽스
* (클래식 UI) 리치 텍스트 편집기 출력 html에 “list-position-style:inside;“를 &lt;ul> 태그에 대한 인라인 스타일로 추가합니다. NPR-22145: CRTE-114용 핫픽스
* 텍스트가 비어 있는 경우 TreeNode가 이름 속성으로 폴백됩니다. NPR-22146: CQ-4234724/CQ-4236300용 핫픽스
* RSS 피드 문제, AEM 6.3에 대한 포트 -1. NPR-22176: CQ-4233339용 핫픽스
* (클래식 UI) 텍스트 붙여넣기 단축키(Ctrl+V)가 OOTB 텍스트(리치 텍스트) 구성 요소에 대해 작동하지 않습니다. NPR-22224: CQ-4236224용 핫픽스
* 텍스트 입력 시 태그 필드의 필터링이 예상대로 작동하지 않습니다. NPR-22236: CQ-4236655용 핫픽스
* (페이지 편집기) 이미지 맵 구성 요소에 텍스트 데이터를 붙여넣을 때 텍스트 데이터를 이미지 맵 구성 요소에 붙여넣으면 텍스트 구성 요소도 붙여넣게 됩니다. NPR-22264: CQ-4236230용 핫픽스
* 대화 상자 FileUpload 필드가 필수이므로 대화 상자 제출 시 문제가 발생합니다. NPR-22464: CQ-4222192용 핫픽스
* 이동된 페이지 또는 해당 레퍼러를 활성화할 수 없는 경우 복제 권한 없이 이동하면 활성화 워크플로에 대한 요청이 시작됩니다. NPR-22467: CQ-4211765용 핫픽스
* 대상자가 큰(2000 이상) 페이지를 로드할 때 성능 문제가 발생합니다. NPR-22478: CQ-4209567용 핫픽스
* ContextHub 저장이 초기화 중에 덮어쓰기 기본 지속성 레이어를 겹쳐 쓰는 경우 지속성 문제가 발생합니다. NPR-22479: CQ-4218399용 핫픽스
* 첫 번째 콘텐츠 루트에서 “하위 페이지 포함”을 선택하지 않고 여러 페이지로 시작하면 하위 페이지가 게시되지 않습니다. NPR-22482: CQ-4237818용 핫픽스
* (Touch UI) 클래식 UI 콘솔을 통해 시작 페이지를 삭제하면 모든 페이지가 편집할 수 없게 됩니다. NPR-22491: CQ-4225074용 핫픽스
* 대화 상자의 추가 공간으로 인해 이미지 구성 요소 관련 문제가 발생합니다. NPR-22528: CQ-4238183용 핫픽스
* 인라인 모드를 사용해 구성 요소를 여는 동안 이전에 로드된 플러그인이 다시 표시되지 않습니다. NPR-22591: CQ-4236850용 핫픽스
* 중첩 실행에서 실행을 삭제하면 하위 실행이 고립됩니다. NPR-22621: CQ-4202639용 핫픽스
* (클래식 UI 사이드 킥) 페이지가 워크플로 잠금 단계에 있는 경우 워크플로 탭이 비활성화됩니다. NPR-22722: CQ-4237557용 핫픽스
* 페이지의 이미지 구성 요소에 추가된 이미지를 뒤집으면 변경 사항이 저장되지 않고 원본 이미지가 페이지에 표시됩니다. 렌더링 지원이 [https://github.com/adobe/aem-core-wcm-components/pull/141](https://github.com/adobe/aem-core-wcm-components/pull/141)을 통해 이미지 코어 구성 요소에 추가되었습니다. NPR-22801: CQ-4221539용 핫픽스
* 사용자가 앵커 메뉴에서 기존 앵커를 삭제하려고 하면 리치 텍스트 편집기 구성 요소 창이 닫히고 변경 사항이 저장되지 않은 상태로 유지됩니다. NPR-22802: CQ-4238167용 핫픽스
* Omnisearch 필터가 Sites 콘솔에 모든 작업을 표시하지 않습니다. NPR-22804: CQ-4239007용 핫픽스
* OS 클립보드 및 내부 AEM 클립보드를 사용할 때 Touch UI에서 복사/붙여넣기와 관련된 문제가 발생합니다. NPR-22807: CQ-4220383용 핫픽스
* Lucene 검색에서 반환된 발췌 강조 표시에 불일치가 발생합니다. NPR-22879: CQ-4238513용 핫픽스
* 게시 인스턴스를 끄고 페이지를 활성화하면 황색으로 바뀌는 대신 녹색 상태가 표시됩니다. NPR-22927: CQ-4236310용 핫픽스
* (StyleSystem) 팝업에서 스타일을 선택하는 동안 화면 위치가 이동합니다. NPR-23183: CQ-4238867용 핫픽스
* (게시 관리) 다음 달로 이동하려면 여러 번 클릭해야 합니다. NPR-23508: CQ-4242732용 핫픽스

### 플랫폼 {#platform-2}

* Sling 내보내기 서블릿이 일본어 문자를 올바르게 내보내지 않습니다. NPR-22153: CQ-4228920용 핫픽스
* 시작하는 동안 스케줄러가 교착 상태가 됩니다. NPR-22440: Sling-7004용 핫픽스
* 두 개의 게시 인스턴스 간에 그룹을 동기화할 수 없습니다. NPR-21943: Granite-19564용 핫픽스
* org.apache.sling.i18n 공유 세션/리소스 확인자에 성능 문제가 발생합니다. NPR-23390: Sling-7543용 핫픽스

### 통합 {#integration-5}

* com.day.cq.analytics.sitecatalyst의 ResourceResolver가 닫히지 않았습니다. NPR-22323: CQ-4236515용 핫픽스
* 쿼리를 장기 실행하는 동안 TargetContentImpl이 AEM을 느리게 만듭니다. NPR-22361: CQ-4236907용 핫픽스
* Target 엔진(mbox.js, at.js)은 mangled URL을 사용하지 않습니다. 콜론이 포함된 URL을 사용하므로 특정 배포에서 실패할 수 있습니다. NPR-22366: CQ-4237854용 핫픽스
* 사용자 정의 at.js 또는 mbox.js를 제공할 때 포함된 스크립트가 HTML 태그 대신 텍스트로 페이지에 작성됩니다. NPR-22441: CQ-4203691용 핫픽스
* 대상 모드에서 작성자가 상속을 취소하지 않고도 블루프린트에서 상속된 구성 요소를 수정할 수 있습니다. NPR-22751: CQ-4237907용 핫픽스
* PersonalizationDataSource가 `jcr:content` 노드 누락으로 인해 Null 포인터 예외를 발생시킵니다. NPR-22850: CQ-4222122용 핫픽스
* 영어 이외의 언어를 사용할 때 AEM 타겟팅이 실패합니다. NPR-22917: CQ-4218213용 핫픽스
* 타겟팅 콘텐츠가 포함된 페이지를 게시하면 관련 리소스가 누락됩니다. NPR-23064: CQ-4227119용 핫픽스
* 클라우드 구성에서 클라이언트 라이브러리로 AT.js를 사용하여 테스트할 때 볼 수 있는 mbox 호출에서 정적 매개변수의 테스트 값을 볼 수 없습니다. NPR-21930: CQ-4234520용 핫픽스

### WCM-Foundation 구성 요소 {#wcm-foundation-components-1}

* 상속 활성화/비활성화 확인란을 선택 취소하면 iParsys가 위치 이동을 생성합니다. NPR-21905: CQ-4230951용 핫픽스
* 양식 드롭다운 구성 요소의 기능 표시/숨기기 기능이 예상대로 작동하지 않습니다. NPR-22327: CQ-4222853용 핫픽스
* 보안 강화를 위해 CAPTCHA 구성 요소는 더 이상 사용되지 않습니다. CAPTCHA 구성 요소를 사용하는 경우 6.3.2.1 이후 릴리스를 설치하면 “Captcha 구성 요소가 삭제되었으므로 더 이상 사용해서는 안 됩니다”라는 메시지가 표시됩니다. 보안 강화를 위해 reCAPTCHA를 포함하도록 AEM 구성 요소를 사용자 정의할 수 있습니다. NPR-22151: CQ-4220052용 핫픽스

### WCM - 페이지 편집기 {#wcm-page-editor}

* 올바르지 않은 선택기를 사용할 때 XSS(크로스 사이트 스크립팅)이 반영됩니다. CQ-4270397용 핫픽스

### 번역 {#translation-4}

* 미리보기 기능을 사용하여 문제를 조사합니다. NPR-22114: CQ-4223753용 핫픽스

### 사용자 인터페이스 {#user-interface-2}

* &#39;min&#39; 및 &#39;max&#39; 날짜 범위가 설정된 경우 Coral 달력의 월 선택기와 관련된 문제가 발생합니다. NPR-22716: CUI-7187용 핫픽스
* (클래식 UI) 연관된 양식 데이터 모델 서비스가 빈 필드로 설정된 경우에도 구성 요소에 기본값이 표시됩니다. NPR-22272: GRANITE-19744용 핫픽스

### Granite {#granite-2}

* 메모리 누출로 인해 자산 공유 AEM 게시자 인스턴스에 안정성 문제가 발생합니다. NPR-22205, NPR-23178: Sling-5668, Sling-7292 및 Sling-7470용 핫픽스.
* 세션 속성 이름에 불안정한 서비스 ID를 사용해서는 안 됩니다. NPR-22821: Granite-21059용 핫픽스
* http 관리 대상 세션이 무효화된 경우 해당 세션에 다른 세션 속성이 없으면 컨테이너 세션도 무효화됩니다. NPR-23059: FELIX-5819용 핫픽스
* LogbackManager 시작 시 일부 OSGi 구성이 누락될 수 있습니다. NPR-23060: Granite-19791용 핫픽스

### 상거래 {#commerce-3}

* 경험 조각 메뉴의 워크플로 작성을 활성화합니다. NPR-22347: CQ-4221661용 핫픽스
* WeRetail에서 경험 조각 오류가 재현될 수 있습니다. NPR-21958: CQ-4220061용 핫픽스
* 삭제된 경험 조각이 포함된 페이지를 활성화하면 NullPointerException이 발생합니다. NPR-23179: CQ-4239939용 핫픽스

### 프로젝트 {#projects}

* (다국어 프로젝트) 프로젝트에 19개를 초과하는 언어에 대한 번역 작업이 나열되지 않습니다. NPR-22498: CQ-4229978용 핫픽스

### 워크플로 {#workflow}

* (클래식 UI) 워크플로 시작 관리자를 활성화하거나 비활성화하면 잘못된 동작이 발생합니다. NPR-22907: CQ-4239153용 핫픽스

## Forms {#forms-9}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

AEM Forms의 주요 사항은 다음과 같습니다.

* HTML5 입력 유형을 추가로 지원합니다.
* 기본 SOAP 헤더 인증이 해결되었습니다.
* 하이퍼링크의 제목 속성에 대한 지원이 추가되었습니다.
* Forms Designer의 액세스 가능성 트리에서 PDF/UA 식별자를 활성화했습니다.
* Workbench 사용자에 대해 인증서 인증을 사용하도록 설정했습니다.
* PDF/A-2a 또는 PDF/A-3a를 준수하는 PDF 파일을 생성하도록 지원을 추가했습니다.

### Forms 추가 기능 패키지 {#forms-add-on-package-9}

#### Forms-관리자 UI {#forms-admin-ui}

* ECM 커넥터 구성 페이지에서 암호 필드 검사 중 암호가 일반 텍스트로 표시됩니다. NPR-22508: CQ-4236065용 핫픽스

#### Forms 서비스 {#forms-service}

* SSL을 사용하도록 설정하면 제출 및 중단 이벤트가 Form Analytics에서 작동하지 않습니다. NPR-22637, CQ-4237973용 핫픽스

#### 사용자 관리 {#user-management}

* 잘못된 cglib-nodep 버전으로 인해 LDAP를 동기화할 수 없습니다. NPR-22493: CQ-4234099용 핫픽스

#### 적응형 양식 {#adaptive-forms-2}

* 규칙 편집기의 사용자 정의 함수에서 함수 호출 후 ;을 추가합니다. 사용자 정의 함수가 true를 반환해도 유효성 검사가 실패합니다. NPR-22481: CQ-4235499용 핫픽스
* 선택된 날짜 패턴과 관계없이, 최소 및 최대 유효성 검사 메시지를 표시할 때 날짜 선택기 구성 요소가 패턴을 따르지 않습니다. NPR-22444: CQ-4236269용 핫픽스
* 제출 요청에 보내는 날짜 형식이 날짜 선택기 구성 요소에 제공된 패턴에 맞아야 합니다. NPR-22384
* 적응형 양식 텍스트 상자에 지정된 최대 문자 수가 Android™ 6.0 Samsung 디바이스에 적용되지 않습니다. NPR-22363, NPR-22364: CQ-4235205용 핫픽스
* (Microsoft® Edge) (IE11) 다중 라인 필드가 있는 적응형 양식 텍스트 필드 구성 요소에 공백이 아닌 `Null`이 기본값으로 표시됩니다. NPR-22284: CQ-69107용 핫픽스
* 적응형 양식의 SOAP UTF-8 입력 인코딩이 잘못된 페이지의 오류를 반환합니다. NPR-20105: CQ-4222669용 핫픽스
* AEM Sites 페이지에서 잘못된 양식이 구성되면 AEM Forms 컨테이너 구성 요소를 편집할 수 없습니다. CQ-4237456용 핫픽스
* 개발 테스트를 JEE 서버에서 실행할 때 테스트가 실패합니다. CQ-4222082용 핫픽스
* Calvin 프레임워크의 축소 문제로 인해 JEE 서버에서 AF 테스트가 실패합니다. CQ-4217220용 핫픽스

#### Forms 관리자 {#forms-manager}

* (Firefox) DOR(기록 문서)의 옵션이 속성 페이지에서 사전 선택되지 않았으므로 적응형 양식의 XML 스키마 속성을 업데이트할 수 없습니다. NPR-22298: CQ-4237402용 핫픽스
* 페이지를 게시한 후 수정된 양식은 다시 게시되지 않습니다. NPR-23013: CQ-4236566용 핫픽스

#### 백엔드 통합 {#backend-integration-1}

* SOAP 서비스에 대한 OOTB 기본 인증이 FDM 통합의 기본 인증에 대해 작동하지 않습니다. NPR-23238: CQ-4241308용 핫픽스

#### 서신 관리 {#correspondence-management}

* OOTB XDPs를 편지 내에서 사용하고 미리보기를 수행하면 콘텐츠가 꼬리말과 겹쳐서 표시됩니다. CQ-4212414용 핫픽스

#### 어셈블러 서비스 {#assembler-service}

* Acrobat DC와 AEM 간의 불일치는 PDF/A-1b 규정 준수 검사 오류에 대해 보고합니다. NPR-22051, NPR-22050: CQ-4226128, CQ-4227671용 핫픽스

### Forms JEE 설치 관리자 {#forms-jee-installer-8}

#### Workbench {#workbench}

* Workbench 사용자에 대해 인증서 인증을 사용하도록 설정했습니다. NPR-20644: CQ-4214486용 핫픽스
* Workbench를 사용한 서버 로그 다운로드는 한 서버에 대해서만 작동하며, 다른 서버에서는 작동하지 않습니다. NPR-21079: CQ-4229842용 핫픽스

#### 프로세스 관리 {#process-management-1}

* (HTML 작업 공간) 스크롤 막대에 화면 크기 문제가 발생합니다. NPR-23288
* (HTML 작업 공간) 프로세스 Startpoint가 영숫자 순서로 정렬되지 않습니다. NPR-22841 CQ-4238944용 핫픽스
* (HTML 작업 영역) 작업 영역의 양식을 닫을 때 데이터 준비가 트리거됩니다. NPR-21127: CQ-4224574용 핫픽스
* (HTML 작업 공간) 긴 설명이 있는 메모가 필요한 프로세스를 호출할 때 메모 확장 버튼이 작동하지 않습니다. CQ-4241488용 핫픽스

#### 코어 {#core-1}

* 스케줄러를 시작하는 중 시작 시 오류가 발생합니다. NPR-22990
* 브라우저에서 HTML 양식에 입력된 자격 증명을 저장할 수 없습니다. NPR-21762: CQ-4206543용 핫픽스
* 코어의 정적 코드 분석에 보고된 문제를 해결해야 합니다. CQ-104446용 핫픽스

#### PDFG 서비스 {#pdfg-service-3}

* PDF Generator가 지정된 책갈피 수준으로 PDF 문서를 생성하지 못했습니다. NPR-22921, NPR-22285: CQ-4230562용 핫픽스
* PDF/A-2a 또는 PDF/A-3a를 준수하는 PDF 파일을 생성하도록 지원을 추가했습니다. NPR-23021: CQ-4214172용 핫픽스

#### Forms Designer {#forms-designer-1}

* Designer에서 PDF로 저장할 때 PDF/UA 식별자가 누락되었습니다. NPR-23137
* Designer에서 PDF로 저장할 때 경로 오브젝트(예: 테두리, 밑줄 및 하이퍼링크)에 태그가 지정되지 않습니다. NPR-23136
* Designer에서 PDF로 저장할 때 이미지 오브젝트에 테두리 상자가 없습니다. NPR-23134
* Designer에 정의된 인라인 하이퍼링크는 Designer에서 PDF로 저장할 때 태그가 지정되지 않거나 대체 텍스트가 없습니다. NPR-23133
* AEM 6.3 Forms Designer를 사용하여 XML 데이터 패키지를 열면 XML 소스에서 XHTML 형식이 제거됩니다. NPR-21178: LC-3917046용 핫픽스

#### LCM 설치 {#install-lcm}

* 설치 관리자 및 LCM에서 Jsafe Jars를 Cryptoj 6.1.3.1로 업데이트합니다. NPR-21370

#### 서명 서비스 {#signatures-service}

* HSM을 통해 PDF 문서를 디지털 서명하는 도중에 예외가 발생했습니다. NPR-21154: CQ-4226978용 핫픽스

### 6.3.2.1에 포함된 OSGi 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-5}

AEM 6.3.2.1에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/bundle-list_002_.txt)

AEM 6.3.2.1에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/content_package_comparison.txt)

AEM 누적 수정 팩 6.3.1.2는 2017년 10월, AEM 6.3 서비스 팩 1(6.3.1.0)의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩의 주요 사항은 다음과 같습니다.

* AEM Assets에서 CUG 기능 구현을 지원하도록 UI가 수정되었습니다.
* 더 나은 환경을 위해 라이선스 확인 페이지의 UI 문제가 수정되었습니다.
* AEM Forms 앱에서 OSGi 워크플로 작업 지원을 사용하도록 설정했습니다.

### 자산 {#assets-10}

* AEM Assets에서 CUG 기능 구현을 지원하도록 UI가 수정되었습니다. NPR-19485
* Touch UI를 사용하여 자산을 직접 하위 노드로 업로드하면 문제가 발생합니다. 자산이 이전에 선택한 자산의 직접 하위로 업로드됩니다. NPR-19736
* 저장된 검색/스마트 컬렉션을 로드할 때 날짜 범위 설명 및 범위 설명이 작동하지 않습니다. NPR-19844: CQ-4220808용 핫픽스
* 여러 자산(4개 이상)이 Brand Portal에 게시되는 경우 AEM 인스턴스 속도가 느려집니다. NPR-20009: CQ-4213426용 핫픽스
* 라이선스 확인 페이지에서 공백이 있는 자산을 다운로드할 수 없습니다. NPR-20067: CQ-4216557용 핫픽스
* 여러 알파 레이어가 있는 PSB 파일을 업로드할 때 처리 문제가 발생합니다. NPR-20250: CQ-4220869용 핫픽스
* 사용자가 파일 이름이 길고 및 면책조항이 정의된 자산을 다운로드할 수 없습니다. NPR-20254
* ProductAssetsUploader가 Java™ TEMP 폴더에 Java™ 캐시의 임시 파일을 둡니다. NPR-20256: CQ-4221801용 핫픽스
* 라이선스 문제로 인해 버전 비교 코드를 Adobe 자체 코드로 대체합니다. NPR-20272: CQ-4223758용 핫픽스
* 문자열 속성의 메타데이터 documentNumber가 날짜로 표시되지만, 숫자여야 합니다. NPR-20291: CQ-4223991용 핫픽스
* 손상된 PDF의 텍스트 추출이 중단되었습니다. NPR-20416: CTG-4150375용 핫픽스
* UTF-8 이외의 호환 이름을 사용하는 자산을 포함하는 압축 파일이 올바르게 다운로드되지 않습니다. NPR-20420: CQ-4219961용 핫픽스
* OmniSearch에 문자가 너무 많으면 AEM 서버가 충돌할 수 있습니다. NPR-20434: CQ-4223602용 핫픽스
* DAM Asset API 메타데이터 결함으로 xmp-write-back API를 중단합니다. NPR-20607: CQ-4220455용 핫픽스
* 사용자를 컬렉션에 추가하는 중에 성능 문제가 발생합니다. NPR-20699: CQ-4225733용 핫픽스
* AEM에서 Brand Portal에 게시는 Dynamic Media 세트에 대해 허용되지 않습니다. NPR-20320: CQ-4221147용 핫픽스
* 공백 및 악센트가 있는 비디오가 렌디션 페이지에 대한 비디오를 생성하지 않습니다. NPR-19961: CQ-4221014용 핫픽스
* 자산 API의 여러 폴더 처리 문제가 해결되었습니다. NPR-20569
* AEM Dynamic Media Classic(이전 Scene7)이 AEM 서버의 자산을 동기화하지 못합니다. 이 문제는 Cloud Service 구성에서 대상 패치 경로가 루트 경로 하위 폴더를 가리킬 때 발생합니다. CQ-4228265
* `{com.day.commons.osgi.wrapper/com.day.commons.osgi.wrapper.commons-email/1.2.0-0002}`을 교체하는 Apache commons `{org.apache.commons/commons-email/1.5}`의 이메일 번들이 추가되었습니다.

### Sites {#sites-10}

* 관리 권한 문제: 페이지 속성에서 닫힌 사용자 그룹 멤버를 제거할 수 없습니다. NPR-20631
* 게시 관리를 통해 페이지를 게시할 때 입력한 워크플로 이름을 알림 상자에서 사용할 수 있어야 합니다. NPR-20046: CQ-4221586용 핫픽스
* 리치 텍스트 편집기의 두 행에 스타일이 지정된 텍스트를 적용한 다음 한 단락에 병합하면 스타일이 지정된 범위가 제거됩니다. NPR-20110: CQ-4223051용 핫픽스
* 속성 편집 대화 상자의 여러 탭에 있는 필드 속성을 변경했을 때 변경 사항이 저장되지 않는 경우가 있습니다. NPR-20286
* 콘텐츠 조각에 붙여넣은 콘텐츠 끝에 예기치 않은 태그가 있습니다. NPR-20413: CQ-4224014용 핫픽스
* 외부 타겟팅 리소스에서 콘텐츠 리소스의 정책을 가져오도록 Adobe Campaign에 메커니즘을 구현했습니다. NPR-20667
* 리치 텍스트 플러그인이 multifield Touch UI의 인라인과 전체 화면 막대에 대해 작동하지 않습니다. NPR-20973

### 캠페인 {#campaign-1}

* 자리 표시자가 여러 개의 Parsys 구성 요소가 포함된 페이지에 표시되지 않습니다. NPR-20436; CQ-4215000용 핫픽스

### 상거래 {#commerce-4}

* 경험 조각이 Internet Explorer 11에서 제대로 표시되지 않습니다. NPR-20161: CQ-4223319용 핫픽스
* 상거래 워크플로에서 여러 이미지가 포함된 기본 제품을 기반으로 변형을 작성할 때 빈 이미지가 자동으로 삽입됩니다. NPR-20068: CQ-4222048용 핫픽스
* 제품 콘솔의 컬렉션 페이지에서 태그별 필터링이 작동하지 않습니다. NPR-20292: CQ-4224023용 핫픽스

### 커뮤니티 {#communities-8}

* 검색 결과가 검색 결과 구성 요소와 일치하지 않습니다. NPR-20070: CQ-4220913용 핫픽스
* 게시된 구성 요소에 대한 모든 중재자 관련 활동에 대해서 이메일 알림이 트리거되지 않습니다. NPR-20122
* 익명 커뮤니티 사용자에 대해 결과가 없는 빈 페이지 매김이 표시됩니다. NPR-20136: CQ-4220738용 핫픽스
* UGC가 스팸으로 감지되거나 사용자가 미리 중재한 사이트에서 게시할 때 경고 트리거를 구성합니다. NPR-20274: CQ-96850용 핫픽스
* 올바르지 않은 리디렉션 및 페이지 새로 고침 문제를 포함하여 AEM Communities 사이트 페이지의 여러 문제가 해결되었습니다. NPR-20344
* CommunityUserOperationExtension이 클래스 캐스트 예외로 실행됩니다. NPR-20532: CQ-4224385용 핫픽스
* Communities 사이트를 생성한 후에는 컨텍스트 경로가 URL 앞에 추가되지 않기 때문에 사용자가 사이트맵에서 이 사이트를 열 수 없습니다. NPR-20730

### 통합 {#integration-6}

* Analytics 기존 인증서를 WSSE 인증으로 마이그레이션하는 중입니다. NPR-19962: CQ-4218071용 핫픽스
* 수정이 실패하고 오류가 발생하여 세그먼트를 다시 활성화하는 중입니다. NPR-20054: CQ-4218401용 핫픽스
* 작성자 인스턴스에서 양식 검색 방법을 사용할 수 없도록 Search&amp;Promote Cloud Service 구성에서 이 방법을 무시합니다. NPR-20447: CQ-4206076용 핫픽스
* 콘텐츠 패키지에 있는 모호한 필터 정의로 인해 Search&amp;Promote 기능을 설치할 때 경로를 덮어씁니다. NPR-20808

### 모바일 온디맨드 {#mobile-on-demand}

* TXT 유형의 자산에 대한 메타데이터 속성이 표시될 때마다 이 속성이 다른 메타데이터 편집기에 표시됩니다. NPR-20239

### 플랫폼 {#platform-3}

* 닫히지 않은 리소스 확인자 예외를 해결했습니다. NPR-19749: Granite용 핫픽스 - 19143
* 작업 대시보드에 기본 상태 확인과 함께 사용자 정의 카드가 표시되도록 요청합니다. NPR-20145
* 페이지 편집기의 주석 레이어가 Internet Explorer 11에서 제대로 작동하지 않습니다. NPR-20222: CQ-4222818용 핫픽스
* 사용자 에이전트를 복제 에이전트의 관리자로 설정할 때 세션 누출이 발생합니다. NPR-20578
* requestAttributes가 다른 data-sly-resource 문에 대해 설정 해제됩니다. NPR-20639: 4226206용 핫픽스
* AEM의 OOTB 자산에 대한 curl Head 요청 문제가 수정되었습니다. NPR-20781: CQ-4221520용 핫픽스

### 프로젝트 {#projects-1}

* 프로젝트 콘솔에서 다른 프로젝트에 액세스하는 데 시간이 더 오래 걸립니다. NPR-20314
* AEM 6.3.0.1을 설치하면 `dam-update-service` 사용자의 키 저장소가 제거됩니다. NPR-20018
* 일부 사용자 정의 배포의 경우 addTask 모듈에서 담당자를 선택하려는 사용자가 사용자 선택기의 목록을 채우는 데 시간이 오래 걸립니다. NPR-20283: CQ-4224193용 핫픽스

### 사용자 인터페이스 {#user-interface-3}

* 대화 상자의 속성에도 불구하고 색상 필드가 “항상 필요”로 설정됩니다. NPR-19702
* 스크롤 막대가 Internet Explorer 11의 전체 화면에서 Multi-field 구성 요소에 대해 표시되지 않습니다. NPR-20261: CQ-4219782용 핫픽스
* 잘못된 결과를 생성하는 연속 쿼리가 트리거되는 경우 이전 쿼리가 중단되지 않습니다. NPR-20398: GRANITE-19306용 핫픽스

### 워크플로 {#workflow-1}

* 사용자에게 받은 편지함에 수신한 워크플로 작업에 대한 알림이 표시되지 않습니다. NPR-20213: CQ-4221639용 핫픽스
* 워크플로 모델의 대화 상자 참가자 단계에서 드롭다운을 클릭했을 때 OOTB granite 사용자 선택기에 사용자가 로드되지 않습니다. NPR-20236

## Forms {#forms-10}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-10}

#### 적응형 양식 {#adaptive-forms-3}

* 반복된 패널에 대한 집계 표현식 지원이 누락되었습니다. NPR-20861
* 연관된 양식 데이터 모델 서비스가 값을 반환하지 않을 때도 드롭다운에 마지막으로 저장된 값이 표시됩니다. NPR-20710
* 규칙 편집기에서 부울 제약 조건을 사용하여 기존 규칙을 편집할 수 없습니다. NPR-21128

#### 양식 포털 {#form-portal}

* 해당 자산 유형이 XDP가 아닌 경우에도 HTML 프로필이 적응형 양식에 대해 표시됩니다. NPR-20079

#### 백엔드 통합 {#backend-integration-2}

* true 또는 false 간에 스위치 구성 요소의 값을 설정할 수 없습니다. NPR-21111

#### OSGI 워크플로 {#osgi-workflow}

* 워크플로 제출 관리는 10개의 애플리케이션만 나열합니다. CQ-4230193

#### HTML5 양식 {#html-forms-3}

* 하위 양식과 같은 XDP 양식 오브젝트의 이름은 액세스 가능성 구성에 정의되지 않으면 해당 도구 설명으로 표시됩니다. NPR-20523

### Forms JEE 설치 관리자 {#forms-jee-installer-9}

#### 프로세스 관리 {#process-management-2}

* FormSetPrefillApp 시작 지점은 AEM Forms 앱의 양식 세트 필드를 미리 채우지 않습니다. NPR-20950

#### Forms - AEM(LiveCycle) {#forms-aem-livecycle}

* 중요 보안 취약성에 대한 최신 CTJPEG2K 라이브러리를 설치합니다. 이 경우 XMLFM(AEM 및 IfBA), RM, PDFG 모듈에 영향을 줍니다. NPR-20625: NPR-21337.

### 기능 팩 포함됨 {#feature-packs-included}

#### AEM Forms 앱 {#aem-forms-app}

* AEM Forms 앱에서 OSGi 워크플로 작업 지원을 사용하도록 설정했습니다. CQ-4222638

### 6.3.1.2에 포함된 OSGi 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-6}

AEM 6.3.1.2에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/6_3_1_2-bundle-list.txt)

AEM 6.3.1.2에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/6_3_1_2-content-package-list.txt)
AEM 누적 수정 팩 6.3.1.1은 2017년 10월, AEM 6.3 서비스 팩 1(6.3.1.0)의 일반 공급 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩의 주요 사항은 다음과 같습니다.

* Brand Portal에 게시 작업을 기본 메타데이터 스키마 양식에 사용하도록 설정했습니다.
* dc: 제목 속성이 `String [] (multifield)`으로 설정된 이미지에 대한 이미지 카드의 제목을 표시할 때 비헤이비어가 변경됩니다.
* 시간의 서버측 렌더링을 foundation-time 구성 요소로 대체했습니다.
* AEM에서 tagadmin/tagging 콘솔의 Brand Portal에 태그를 게시하도록 설정합니다.
* 콘텐츠 조각을 소비할 JSON API를 게시했습니다.
* 내장된 저장소(Apache Jackrabbit Oak)가 버전 1.6.5으로 업데이트되었습니다.

### 자산 {#assets-11}

* 속성이 동일한 두 필드를 유형이 다른 속성 필드와 매핑하면 내부 오류가 발생합니다. NPR-19462: CQ-4216828용 HF
* dc: 제목과 dc: 설명이 CRXDE Lite의 복수 필드 값으로 변경되지 않습니다. NPR-19570: CQ-4209086용 HF
* 작성자 모드에서 비디오 재생 환경을 테스트하기 위해 동적 뷰어에 가장 낮은 품질의 비디오 렌디션이 로드됩니다. NPR-19004
* 이름에 공백이 있는 자산에 대한 동적 렌디션을 다운로드할 수 없습니다. NPR-19433: CQ-4211738용 핫픽스
* Chrome을 사용하여 열 보기에 전체 페이지/자산 목록을 로드할 수 없습니다. NPR-19566: CQ-4214248용 핫픽스
* 스키마 또는 검색 패싯 또는 사전 설정을 선택하는 경우 Brand Portal에 게시 옵션을 사용할 수 없습니다. NPR-19550
* 열 보기에서 자산을 선택하고 편집을 클릭하면 페이지에 오류가 반환됩니다. NPR-20301: CQ-4224052용 핫픽스
* 양수 및 음수 시간대가 교차할 때 자산 만료 표시가 꺼집니다. NPR-20329: CQ-4219333용 핫픽스

### 캠페인 {#campaign-2}

* 캠페인에 대해 기본 경험을 선택한 경우 캠페인 슬라이더 구성 요소가 표시되지 않습니다. NPR-19213

### 통합 {#integration-7}

* 익명 사용자로 액세스할 때 사용자 정의 at.js 파일이 게시되지 않습니다. NPR-19542: CQ-4219592용 핫픽스
* 구성 마법사의 타겟팅 엔진 필드가 Adobe Target이 아닌 ContextHub(AEM)로 설정되어 있습니다. NPR-19320: CQ-4218465용 HF
* 경험을 생성하는 동안 대상자 섹션이 손상되었습니다. NPR-19110
* 대상 모듈을 편집하고 두 번 이상 저장하면 타겟팅 대화 상자가 타겟팅 모드에 표시되지 않습니다. NPR-19144: CQ-4216708용 핫픽스
* 문서에 대한 액세스 속성이 클래식 UI의 Adobe Digital Publishing Solution에서 잘못 설정됩니다. NPR-19367
* 사용자가 여러 영역에 액세스할 수 있는 경우 Campaign을 통해 오퍼를 개인화할 때 잘못된 자동 접기 동작이 수행됩니다. NPR-19290: CQ-4218029용 핫픽스

### Sites {#sites-11}

* 인스턴스를 AEM 6.1SP2-CFP3로 업그레이드하면 Sidekick.js의 변경 코드로 인해 Multi-composite 필드 드롭다운 값이 다시 채워지지 않습니다. NPR-19450: CQ-4194771용 HF
* WCMMode.EDIT는 작성 모드에서 대상 구성 요소에 대해 작동하지 않습니다. NPR-19387
* 콘텐츠 조각을 소비할 JSON API를 게시했습니다. NPR-19500
* 굵게, 기울임꼴, 밑줄 기능이 작성자 대화 상자의 리치 텍스트 편집기 필드에 대해 작동하지 않습니다. NPR-19670: NPR-19718: CQ-4219088용 핫픽스

### 모바일 온디맨드 {#mobile-on-demand-1}

* 전체 크기 이미지를 사용할 때 AEM 설명서 콘솔의 문제를 렌더링하면 속도가 느려집니다. NPR-19088

### 번역 {#translation-5}

* 번역 프로젝트에 대한 미리보기를 생성할 수 없습니다. NPR-19289

### 보안 {#security}

* SSL 연결 오류입니다. 서버에 보안 연결을 설정할 수 없습니다. NPR-19628

### 커뮤니티 {#communities-9}

* 미리 중재된 사이트를 사용하여 게시하는 콘텐츠에서 Mail이 트리거됩니다. NPR-20008
* 게시된 구성 요소에 대한 모든 중재자 관련 활동에 대해서 이메일 알림이 작동하지 않습니다. NPR-19767: CQ-4218060용 HF

### 플랫폼 {#platform-4}

* AEM 프로덕션 서버 배포에 안정성 문제가 있습니다. NPR-19707
* AEM 6.3으로 업그레이드한 후 스크립트로 구현된 태그를 참조하는 사용자 정의 taglib을 찾을 수 없습니다. NPR-19087
* AEM 6.3.1에 대한 HTL 버그 수정 사항입니다. NPR-19161
* 리치 텍스트 필드를 multi-field 구성 요소에서 편집할 수 없습니다. NPR-19604: Granite-16755용 핫픽스
* Adobe 이메일 템플릿 서비스는 사용자 정의 사용자 템플릿에 태그를 추가합니다. NPR-19190
* Oak 1.6.5.용 핫픽스 NPR-19148

### 상거래 {#commerce-5}

* XF 변형 편집기를 선택한 후에도 워크플로 시작 버튼은 영향을 주지 않습니다. NPR-19642: CQ-4207796용 핫픽스

### 프로젝트 {#projects-2}

* 프로젝트 편집기에서 프로젝트 자산 폴더에 자산을 복사하고 붙여넣을 수 없습니다. NPR-19619: CQ-4215321용 핫픽스

### 웹 콘텐츠 관리 {#web-content-management}

* 롤아웃 화면에서 Live Copy 페이지에 해당하는 확인란을 선택하거나 선택 취소할 수 없습니다. NPR-19518
* 현재 모든 탭 및 필드를 벌크 버전에 사용할 수 있으므로 페이지 속성의 벌크 편집은 올바르게 사용할 수 없습니다. NPR-19451
* 클래식 UI에서 이미지를 편집할 때 OOTB 속성 및 이미지 정렬 속성이 표시되지 않습니다. NPR-19488: CQ-4217914용 HF

### 사용자 인터페이스 {#user-interface-4}

* Google Chrome 브라우저를 사용하는 경우 사용자가 TouchUI의 열 보기를 사용하여 전체 페이지/자산 목록을 로드할 수 없습니다. NPR-19566: CQ-4214248용 핫픽스

### Brand Portal {#brand-portal-1}

* 댓글 및 주석과 함께 AEM의 자산을 게시할 수 없습니다. NPR-19590: CQ-4218386용 핫픽스
* AEM에서 tagadmin/tagging 콘솔의 Brand Portal에 태그를 게시하도록 설정합니다. NPR-20271: CQ-4223948용 핫픽스
* Brand Portal 클라우드 서비스 구성 UI의 “활성화됨” 필드를 수정합니다. CQ-4211101용 핫픽스
* 검색 양식 복제가 실패했습니다. CQ-4220080용 핫픽스

## Forms {#forms-11}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 AEM Forms 릴리스를 참조하십시오.

### Forms 추가 기능 패키지 {#forms-add-on-package-11}

#### 적응형 양식 {#adaptive-forms-4}

* JEE에 제출 워크플로는 JEE 측에서 AEM으로 출력 매개변수를 다시 반환하지 않고 “값이 기본값이 아니므로 무시” 오류가 발생합니다. NPR-20265
* 적응형 양식은 Safari에서 PDF를 첨부 파일로 허용하지 않습니다. NPR-19625
* RestoreGuideState는 customcontextproperty 맵을 덮어씁니다. CQ-4222877
* Cloud Service를 사용하여 Google `reCaptcha`를 구성할 때 외부 연결에 org.apache.http.proxyconfigurator 구성이 필요한 환경에서는 POST 호출이 프록시를 통과하는 것 같지 않습니다. NPR-20454
* XSD 스키마를 기반으로 한 적응형 양식은 마침표(.) 이외의 소수 구분 기호가 있는 로케일을 사용하여 설치할 때 숫자 필드에 대해 잘못된 XML값을 제출하므로 오류가 발생합니다. NPR-20444
* 서드파티 서버에 대한 HTTP 요청을 만드는 동안 “Apache HTTP 구성 요소 프록시 구성”에 대해 설정된 프록시 설정이 적용되지 않습니다. HTTP GET 또는 POST 호출 사용 시 연결 제한 시간 문제가 발생합니다. NPR-20457, NPR-20456, NPR-20455, NPR-20451

#### Forms 데이터 통합 {#forms-data-integration}

* SOAP 서비스의 출력으로 UTF-8 문자가 영어가 아닌 로케일의 적응형 양식 필드에 올바르게 복사되지 않습니다. NPR-20238: NPR-20103

#### 서신 관리 {#correspondence-management-1}

* 단어 파일에서 콘텐츠 복사 붙여넣기를 수행하면 텍스트 편집기에서 해당 콘텐츠 색상 및 글꼴이 손실됩니다. NPR-19521

#### 어셈블러 서비스 {#assembler-services}

* PDFA-1b 형식에 대한 문서의 규정 준수 확인 중에 Acrobat과 AEM의 결과 불일치가 발생했습니다. NPR-19280

#### 워크플로 {#workflow-2}

* 프록시를 통해 연결할 수 있도록 HTTP 호출을 허용하는 워크플로 서명 단계입니다. NPR-20529

#### HTML5 양식 {#html-forms-4}

* preSubmit 이벤트에 대한 지원이 추가되었습니다. NPR-20604

### Forms JEE 설치 관리자 {#forms-jee-installer-10}

#### 프로세스 관리 {#process-management-3}

* 양식이 최대화/최소화되어 초안으로 저장되거나 전달된 경우 작업 영역에서 워크플로 첨부 파일, 노트 및 세부 사항 탭이 작동하지 않습니다. NPR-20243
* HTML 작업 영역에서 데이터를 제출한 후 여러 줄 텍스트 필드(TextArea)가 새 줄 바꿈 문자를 유지하지 않거나 텍스트에서 중단됩니다. NPR-20085

#### 프로세스 보고 {#process-reporting}

* Null 포인터 예외로 인해 프로세스 보고가 데이터를 제대로 가져오지 않습니다. NPR-19759

>[!NOTE]
>
>[AEM Forms 릴리스](aem-forms-releases.md) 문서에 나열된 LiveCycle 임베드 패키지를 설치하여 문제를 해결합니다.

#### 표준 서비스 {#standard-services}

* docConvertor가 PDF의 평면화 투명성을 지원하지 않으며, PDF/A를 생성하지 못합니다. NPR-16228: CQ-4214488용 핫픽스

#### 코어 {#core-2}

* JBoss® 애플리케이션에서 클러스터 구성으로 실행 중인 AEM Forms 서버가 중지되면 데이터베이스에서 애플리케이션 서버의 연결이 해제됩니다. 이로 인해 데이터 손상 문제가 발생할 수 있습니다. NPR-19724

### 기능 팩 포함됨 {#feature-packs-included-1}

* 자산에 대한 필수 필드 유효성 검사가 누락되었으므로 드롭다운 메타데이터 스키마 필드를 필수로 만들 수 없습니다. NPR-17882: CQ-4208373용 FP

### 6.3.1.1에 포함된 OSGi 번들 및 콘텐츠 패키지 {#osgi-bundles-and-content-packages-included-in-7}

AEM CFP 6.3.1.1에 포함된 OSGi 번들 목록

[파일 가져오기](assets/do-not-localize/bundle-list.txt)

AEM CFP 6.3.1.1에 포함된 콘텐츠 패키지 목록

[파일 가져오기](assets/do-not-localize/content-package-list.txt)

AEM 누적 수정 팩 6.3.0.2는 2017년 4월, AEM 6.3의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다.

AEM 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 사용자 액세스 제어의 사용 가능성
* 버전 1.6.2의 내장 저장소(Apache Jackrabbit Oak)가 포함되어 있음
* 닫히지 않은 리소스 확인자 문제가 해결됨
* 스마트 콘텐츠 서비스에 대한 구성 단순화
* 콘텐츠 조각 유효성 검사 문제가 해결됨
* 하이브리드 디바이스에서 메타데이터 스키마의 편집 가능성이 향상됨
* 라이브 카피의 구성 요소 수준의 동기화 문제가 해결됨
* 열 보기에서 콘텐츠가 많은 페이지의 유용성이 향상됨
* 긴 제목이 있는 페이지에 대한 페이지 이름 지정 규칙 준수를 향상함
* Touch UI의 캠페인 개인화 환경이 개선됨
* 다양한 프로젝트 오버레이 문제에 대한 수정 사항

### 플랫폼 {#platform-5}

* Oak 1.6.2.용 핫픽스 NPR-16993
* 필터를 사용하여 omnisearch를 여는 동안 경로가 더는 설정되지 않습니다. NPR-17398: CQ-4204870용 핫픽스
* AEM에서 사용자 권한 변경 사항 감사 가능성에 대한 요구 사항. NPR-17061
* DM 클라우드 서비스의 연결 속도가 느리므로 “파일이 너무 많이 열려 있습니다” 예외가 발생합니다. CQ-4211407

### 자산 {#assets-12}

* 다른 옵션을 사용하여 스마트 콘텐츠 서비스를 구성하는 데 유용성 문제가 있습니다. NPR-18200: CQ-4201557용 핫픽스
* 이진 형식의 리소스 누출이 S3 데이터 저장소로 스트리밍됩니다. NPR-18041: CQ-4209506용 핫픽스
* ASCII/UTF-8로 인코딩된 텍스트 파일이 AEM Assets에 업로드되고 썸네일 생성이 실패하는 경우 오류가 발생합니다. NPR-18006: CQ-4209345용 CFP
* 기본 메타데이터 스키마로 인해 콘텐츠 조각 유효성 검사가 실패합니다. NPR-17769: CQ-4211111용 핫픽스
* com.day.cq.dam.s7dam.common.analytics.impl.SiteCatalystReportRunner에서 리소스 확인자가 닫히지 않음. NPR-17598: CQ-4209018용 CFP
* Brand Portal에 자산을 게시하기 위해 여러 복제 에이전트를 생성하도록 요청합니다. NPR-17189
* 일본어 폴더에 있는 자산에 대한 리뷰 작업이 작동하지 않습니다. CQ-4204782
* 자산이 해당 속성 페이지에서 이동되면 Null 포인터 예외가 발생합니다. CQ-4204251
* 자산이 InDesign 문서에 여러 번 연결되는 경우 AEM은 속성 페이지에서 해당 자산에 대한 후속 참조를 추적하지 못합니다. CQ-4204186
* 하이브리드 디바이스의 Chrome에서 편집할 때 메타데이터 스키마 양식에 새 탭 추가 시 문제가 발생합니다. CQ-4201810
* 중복 자산이 업로드되면 중복 감지 대화 상자에서 중복 자산을 선택하지 않은 경우에도 (삭제/유지) 옵션이 모든 자산에 적용됩니다. CQ-4201673
* 들어오는 참조가 150개 이상인 자산 폴더를 이동하면 null 포인터 예외가 발생합니다. CQ-4200981
* 다운로드한 자산 폴더의 경우, ZIP 파일의 콘텐츠를 추출할 때 충돌이 발생하면 기본 옵션이 둘 다 유지가 아닌 버전 만들기로 표시됩니다. CQ-97800
* 앱에 대해 읽기 전용 권한이 있는 사용자는 AEM Mobile 콘텐츠 관리에서 콘텐츠를 미리 볼 수 없습니다. NPR-17486: CQ-4209690용 CFP
* 카탈로그 만들기 버튼이 카탈로그 콘솔의 열 보기에서 작동하지 않습니다. CQ-4209952

### Sites {#sites-12}

* data-sly-resource 속성을 통해 이미지/비디오 구성 요소를 임베드할 때 문제가 발생합니다. NPR-18182: CQ-4212100용 CFP
* 상속이 LiveCopy에서 다시 적용될 때 현지화된 구성 요소가 원래 양식으로 복원되지 않는 문제를 수정했습니다. NPR-18172: CQ-4211379용 핫픽스
* Touch UI의 열 보기에서 콘텐츠가 많은 페이지를 탐색하는 데 문제가 발생합니다. NPR-17799: CQ-4199611용 핫픽스
* `com.day.cq.wcm.core.impl.VersionManagerImpl`에서 리소스 확인자가 닫히지 않았습니다. NPR-17789: CQ-4211152용 CFP
* 긴 페이지 제목에 대한 규칙에 따라 페이지 이름이 생성되지 않습니다. NPR-17633: CQ-4209056용 핫픽스
* JBoss® EAP 6.4에 배포된 AEM 6.3의 Touch UI에서 페이지 작성과 관련된 문제가 발생합니다. NPR-17589: CQ-4210137 핫픽스
* 중첩된 그룹이 있는 경우 워크플로 상태 제공자로 인해 인스턴스가 잠깁니다. NPR-17556: CQ-4202056에 대한 CFP 요청
* 다음 오브젝트에서 리소스 확인자가 닫히지 않았습니다.

   * `com.day.cq.wcm.undo.impl.BinaryValueManagerImpl` NPR-17497: CQ-4208673용 CFP
   * `com.day.cq.commons.impl.ThumbnailProviderManagerImpl` NPR-17495: CQ-4208668용 CFP
   * `com.day.cq.wcm.workflow.impl.WcmWorkflowServiceImpl` NPR-17494: CQ-4208669용 CFP
   * `com.day.crx.delite.impl.AuthHttpContext` NPR-17493: GRANITE-17404용 CFP

### 통합 {#integrations-1}

* AEM Day HTTP Client 3.1 OSGI가 다이제스트 인증을 필요로 하는 프록시로 구성된 경우 발생할 수 있는 AEM 검색 구성 요소 오류가 해결되었습니다. NPR 18128: NPR-18029용 핫픽스
* 클래식 UI를 통해 캠페인 및 관련 경험을 개인화할 때 문제가 발생합니다. NPR-18127: CQ-4211559용 핫픽스
* 사이트의 루트 페이지로 브랜드/영역을 설정할 때 상속이 취소되면 하위 페이지의 영역에 대해 복원할 수 없습니다. NPR-17753: CQ-4210139용 핫픽스

### 워크플로 {#workflow-3}

* 영구 워크플로에서 외부 프로세스 단계가 지속되기 전에 변경된 프로세스 기록 및 메타데이터가 변경되었습니다. NPR-17848: GRANITE-17757용 핫픽스
* 워크플로 대화 상자 필드의 값이 작업 항목 노드에서 지속되지 않습니다. NPR-17734: CQ-4210369용 핫픽스
* 받은 편지함에서 작업을 편집할 때 구문 분석할 수 없는 오류가 발생합니다. CQ-4208749

### 프로젝트 {#projects-3}

* 다양한 프로젝트 오버레이 문제에 대한 수정 사항입니다. NPR-17733
* 프로젝트 모듈의 포드를 재구성하면 구성 가능성이 작아집니다. CQ-4209859
* 페이지가 번역 작업에 추가되면 자산 경로가 현지화된 해당 사이트로 변경됩니다. CQ-4206007

### 보안 {#security-1}

* LDAP 사용자에 대한 아바타 이미지 업로드 시 문제가 발생합니다. NPR-16561
* XSS 취약성을 선점하기 위해 Apache Sling API에서 업그레이드된 버전의 org.apache.sling.servlets.post 서블릿(2.3.22)을 사용하도록 요청합니다. NPR-18963

## Forms {#forms-12}

AEM Forms 수정 사항은 릴리스와 함께 제공되는 Forms 추가 기능 패키지 및 기타 패치 설치 관리자를 통해 게재됩니다. 자세한 내용은 [AEM Forms 릴리스](aem-forms-releases.md)를 참조하십시오.

AEM Forms의 주요 사항은 다음과 같습니다.

* 서신 관리 텍스트 모듈, 편지 미리보기 및 프로그래밍 방식으로 서신 작성 관리 UI를 실행하여 수정합니다.
* PDF/A-1b 유효성 검사, 큰 이미지 파일을 PDF로 변환, PDF Generator의 일본어 PDF 문서에 대한 수정 사항입니다.
* 서신 관리, 문서 보안 및 Forms Workflow에 대한 유용성 수정 사항입니다.
* 서명 쓰기 필드에 대한 감사 이벤트를 캡처하도록 지원을 추가했습니다.

### Forms 추가 기능 패키지 {#forms-add-on-package-12}

**서신 관리**

* 서신 관리 조각을 편집할 때 텍스트 편집기에 처리된 텍스트와 함께 인라인 조건이 표시됩니다. CQ-4211930
* 서신 관리 편지를 작성하는 경우 편지에 대한 설명이 저장되지 않습니다. NPR-18089
* 글머리 기호 목록 위와 아래에 있는 추가 여백이 텍스트 편집기에 표시되지만, HTML 및 PDF 렌디션에는 표시되지 않습니다. NPR-18126
* HTML 제출에서 POST 방법을 사용하면 서신 작성 UI가 실행되지 않습니다. NPR-18202
* 텍스트 모듈이 저장되고 텍스트 모듈의 표현식에 열기 또는 닫기 표현식 태그가 없으면 오류 메시지가 표시되지 않습니다. 텍스트 모듈에 오류 메시지가 표시되고 편지에서 렌더링되지 않습니다. NPR-18535
* 새 콘텐츠가 추가되거나 `Enter` 키를 누르면 div 태그가 텍스트 모듈에 추가됩니다. NPR-18240

**어셈블러**

* PDF/A-1b 규정 준수에 대한 PDF 문서의 유효성을 확인할 때 AEM Forms가 유효성 검사 오류를 반환합니다. PDFA_CONTENT_003_DEVICE_DEPENDENT_COLOR_USED. Adobe Preflight 및 서드파티 소프트웨어로 유효성을 확인할 때 PDF 문서에 오류가 반환되지 않습니다. NPR-18011
* PDF/A-1b 규정 준수에 대한 PDF 문서의 유효성을 확인할 때 AEM Forms가 유효성 검사 오류를 반환합니다. 양식 필드에는 여러 개의 모양이 있습니다. PDF 문서가 PDF/A-1b 규정을 준수합니다. NPR-18013

**감시 폴더**

* 워크플로를 사용하여 파일을 처리하도록 선택할 때 감시 폴더를 작성하는 중에 워크플로 모델 선택 드롭다운이 잘려서 표시됩니다. NPR-17566

**HTML5 양식**

* AEM Forms가 서명 쓰기 필드에 대한 감사 이벤트를 캡처하지 않습니다. NPR-15286

**Forms 관리자**

* AEM Forms UI는 가장 오래된 첫 번째 주문의 모든 자산을 나열합니다. 사용자가 최신 순서로 자산을 재정렬할 수 없습니다. NPR-18450

**Java™ API 참조**

com.adobe.livecycle.content 클래스에 대한 JavaDocs가 추가되었습니다. NPR-18468

### Forms JEE 설치 관리자 {#forms-jee-installer-11}

**PDF Generator**

* PDF Generator 서비스가 100MB 이상의 이미지를 PDF 문서로 변환하지 못합니다. CQ-4208628
* 일본어 OCR로 PDF Generator 서비스를 사용하면 반전된 PDF가 생성됩니다. NPR-17602

**프로세스 관리**

* TaskContext 변수가 AEM Forms 프로세스에 대해 채워지지 않습니다. NPR-18199

**문서 보안**

* Microsoft® Excel 및 Microsoft® PowerPoint에서 Microsoft® Office용 AEM 문서 보안 확장으로 보호된 문서를 여는 데 시간이 오래 걸립니다. CQ-4212358
* 새 정책이 작성되고 기존 이름과 동일한 이름의 정책이 있는 경우 내부 서버 오류가 발생합니다. NPR-18247

## 기능 팩 포함됨 {#feature-packs-included-2}

* AEM에서 사용자 권한 변경 사항 감사 가능성에 대한 요구 사항. NPR-17061

AEM 누적 수정 팩 6.3.0.1은 2017년 4월, AEM 6.3의 일반 출시 이후 다수의 내부 및 고객 수정 사항을 포함한 중요한 업데이트입니다. AEM 누적 수정 팩의 주요 사항은 다음과 같습니다.

* 다음 영역이 개선되었습니다.

   * 콘텐츠 조각, Sites 및 리치 텍스트 편집기, 규칙 편집기 및 템플릿 편집기 구성 요소
   * 소셜 검토 및 Facebook 소셜 로그인
   * 번역 작업 구성 및 시작
   * 소셜 커뮤니티의 알림에 액세스하기 위한 응답 시간
   * DAM 저장소에 검토 작업 표시

* 오버레이와 CFP 간의 충돌을 감지하기 위한 패키지 관리자의 유효성 검사 옵션 제공

## 소프트웨어 배포를 통한 CFP용 지침 다운로드 {#download-instructions-for-cfp-via-package-share}

[소프트웨어 배포](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html)에서 직접 CFP 패키지를 다운로드하거나 다음 단계를 수행할 수 있습니다.

1. [소프트웨어 배포](https://experience.adobe.com/downloads)를 엽니다. 소프트웨어 배포에 로그인하려면 Adobe ID가 필요합니다.
1. 헤더 메뉴에 제공된 **[!UICONTROL Adobe Experience Manager]**&#x200B;를 누릅니다.
1. 패키지 이름을 탭하고 **[!UICONTROL EULA 약관 동의]**&#x200B;를 선택한 후 **[!UICONTROL 다운로드]**&#x200B;를 탭합니다.

## 설치 지침 {#installation-instructions}

이 섹션에서는 CFP를 설치하기 위한 요구 사항 및 단계를 안내합니다.

### 설치하기 전에 {#before-you-install}

>[!NOTE]
>
>Adobe에서 제공하는 선택적 기능 팩은 릴리스 버전 및 누적 수정 팩에 종속되어 있습니다. 기능 팩이 설치되어 있는 경우 [AEM 고객 지원 센터](https://experienceleague.adobe.com/?support-solution=General#support)에 문의하여 이 AEM 6.3용 누적 수정 팩과의 호환성을 확인하십시오.

>[!NOTE]
>
>패키지 설치를 시도하기 전에 모든 새 설치 패키지에서 유효성 검사를 실행하는 것이 좋습니다. 사전 유효성 검사는 설치 전에 발견된 모든 오류를 분석 및 보고하고, 그러한 오류에 대해 사전에 사용자에게 경고합니다.
>
>[https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)에서 유효성 검사 옵션에 대한 설명서에 액세스할 수 있습니다.

* AEM 6.3.3.0은 CFP를 위한 필수 구성 요소입니다. AEM 설치를 AEM 6.3으로 업그레이드하는 방법에 대한 세부 지침은 [업그레이드 설명서](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)를 참조하십시오.
* RDBMK 또는 MongoDB를 사용한 클러스터 배포를 위해 패키지 관리자를 사용하는 작성자 인스턴스에 CFP 패키지를 설치할 수 있습니다.
* 누적 수정 팩을 설치하기 전에 스냅샷을 작성하거나 AEM 인스턴스를 백업하십시오.
* CFP는 제거할 수 없습니다.

### 새 로거 추가 {#adding-new-loggers}

SP/CFP 설치 중에 디버그 수준 로깅을 구성하고 활동 로그를 검색하려면 아래 단계를 수행하십시오.

* 아래 속성을 사용하여 기본 위치 [http://localhost:4502/system/console/slinglog](http://localhost:4502/system/console/slinglog)에 로거를 추가할 수 있습니다.

   * 로그 수준: 디버그
   * 추가: false
   * 로그 파일: logs/activity.log
   * 로거: org.apache.jackrabbit.vault.packaging.impl.ActivityLog

activity.log가 crx -quickstart /logs 폴더에 생성됩니다.

### 소프트웨어 배포를 통해 누적 수정 팩 설치 {#install-the-cumulative-fix-pack-via-package-share}

1. [소프트웨어 배포](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq640/cumulativefixpack/aem-6.4.8-cfp-2.0.zip) 링크를 클릭하면 패키지를 다운로드할 수 있습니다.

1. [패키지 관리자](http://localhost:4502/crx/packmgr/index.jsp)를 열고 **[!UICONTROL 패키지 업로드]**&#x200B;를 클릭하여 패키지를 업로드합니다.

1. 패키지 이름을 선택하고 **[!UICONTROL 설치]**&#x200B;를 클릭합니다.

### 자동 설치 {#automatic-installation}

CFP는 다음과 같은 방법으로 실행 중인 인스턴스에 자동으로 설치할 수 있습니다.

* 서버가 실행되는 동안 `../crx-quickstart/install`에 패키지를 둡니다. 패키지가 자동으로 설치됩니다.
* [패키지 관리자에서 HTTP API](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)를 사용하여 `cmd=install&recursive=true`를 사용하는지 확인합니다. 이 경우 중첩된 패키지가 설치됩니다.

### 설치 확인 {#validate-installation}

1. 제품 정보 페이지(`/system/console/ productinfo`)의 설치된 제품 아래에 이제 업데이트된 버전 문자열 “Adobe Experience Manager, 버전 6.3.3.8”이 표시됩니다.
1. 모든 OSGI 번들은 OSGi 콘솔에서 ACTIVE이거나 FRAGMENT입니다(웹 콘솔 사용: `/system/console/bundles`).

>[!NOTE]
>
>패키지를 성공적으로 설치하면 콘텐츠 패키지가 성공적으로 설치되었음을 나타내는 정보 메시지가 오류 로그에 표시됩니다. (예: “콘텐츠 패키지 **AEM-6.3.3-Cumulative-Fix-Pack-7**&#x200B;이 성공적으로 설치되었습니다.”)

>[!NOTE]
>
>AEM 6.3.3.1 이후 Jackrabbit FileVault의 로그 수준이 메시지 대부분에 대해 INFO에서 DEBUG으로 변경되었습니다. AEM 6.3.3.1 이상에 설치된 콘텐츠 패키지에 대한 설치 로그를 가져오려면 org.apache.jackrabbit.vault.packaging.impl에 DEBUG 로그 레벨을 사용합니다.

### AEM Forms 설치 {#install-aem-forms}

>[!NOTE]
>
>AEM Forms를 사용하지 않는 경우 이 섹션을 건너뜁니다.

#### AEM Forms 추가 기능 설치 {#install-forms}

1. AEM 6.3.3.x CFP 패키지를 설치했는지 확인합니다.
1. 운영 체제에 대한 [AEM Forms 릴리스](aem-forms-releases.md)에 나열된 해당 양식 추가 기능 패키지를 다운로드합니다.
1. [AEM Forms 추가 기능 패키지 설치](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)에 설명된 대로 Forms 추가 기능 패키지를 설치합니다.

#### AEM Forms JEE 번들 패키지 설치 {#install-aem-forms-jee-bundles-package}

별도의 설치 관리자를 통해 AEM Forms JEE의 수정 사항이 전달됩니다. JEE의 AEM Forms에 CFP를 설치하는 방법에 대한 자세한 내용은 [AEM Forms JEE에 CFP 설치](install-cfp-aem-forms-jee.md)를 참조하십시오.

#### Forms Designer 설치 관리자 {#designer-installer}

1. 업데이트를 설치하려면 Designer 6.2.0_&lt;Language>_Cumulative_QF.msp 파일을 실행합니다.
1. 시작 화면에서 **업데이트**&#x200B;를 클릭합니다. 설치가 시작됩니다.
1. 설치가 완료되면 **완료**&#x200B;를 클릭합니다.

## AEM Forms JEE(JBoss® EAP)에 대한 구성 설정 {#configuration-settings-for-aem-forms-jee-jboss-eap}

>[!NOTE]
>
>6.3.3.0 이상 릴리스를 설치하는 경우 다음 절차를 수행하여 JBoss® 애플리케이션 서버에 대한 설정을 구성합니다. Oracle WebLogic 또는 IBM® WebSpehere 애플리케이션 서버에서 실행 중인 AEM Forms 서버에 6.3.3.0을 설치하는 경우 추가 구성이 필요하지 않습니다. 자세한 내용은 [AEM 6.3.3.0 릴리스 정보](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)를 참조하십시오.

## Search&amp;Promote 통합에 대한 구성 업데이트 {#configuration-updates-for-search-promote-integration}

AEM 누적 수정 팩 6.3.0.2 및 이후 릴리스에서 Search&amp;Promote 통합에 사용된 OSGi 구성은 **Apache HTTP 구성 요소 프록시 구성**&#x200B;입니다. Day Commons HTTP Client 3.1의 프록시 구성은 이제 사용되지 않습니다.

## 알려진 문제 {#known-issues}

* 다음 오류 및 경고는 AEM CFP 6.3.3.x 설치 중에 발생할 수 있으며, 무시해도 됩니다.

   * &#42;경고&#42; [OsgiInstallerImpl] org.apache.jackrabbit.vault.packaging.impl.InstallHookProcessorImpl Hook /META-INF/vault/hooks/cloudservices-wfchangeinstallhook-0.0.2-jar-with-dependencies.jar에서 런타임 예외가 발생했습니다.
   * &#42;오류&#42; [OsgiInstallerImpl] [com.adobe.cq.social.cq-social-jcr-provider com.adobe.cq.social.provider.jcr.impl.SpiSocialJcrResourceProviderImpl(2174)] 등록 변경으로 등록 취소를 완료할 때까지 기다리는 중 시간이 초과되었습니다. CQ-4209974.
   * org.apache.sling.engine.impl.SlingRequestProcessorImpl ServletResolver 서비스가 누락되어 상태 503 보내기 요청을 처리할 수 없습니다.
   * com.day.cq.wcm.mobile.core.MobileUtil isMobileResource: 리소스 [/bin/receive]를 확인할 수 없고, 페이지 관리자를 사용할 수 없습니다.
   * org.apache.sling.servlets.resolver.internal.SlingServletResolver: 오류 처리기를 호출하면 오류가 발생합니다.
   * org.apache.sling.servlets.resolver.internal.SlingServletResolver 원래 오류가 null입니다.
   * org.apache.sling.engine.impl.DefaultErrorHandler 오류 처리기의 java.io.IOException 처리 실패
   * &#42;오류&#42; [FelixDispatchQueue] com.day.cq.dam.cq-dam-core FrameworkEvent 오류(org.osgi.framework.ServiceException: 서비스 팩토리가 null을 반환했습니다. (구성 요소: com.day.cq.dam.handler.standard.ps.PostScriptHandler))

**Brand Portal**

* 6.3.1.2 이상에서 스마트 컬렉션에 대한 Brand Portal에 게시 버튼이 제거되었습니다.

**사용자 인터페이스**

>[!NOTE]
>
>이러한 두 가지 문제의 영향을 받는 경우 [AEM 고객 지원 센터](https://experienceleague.adobe.com/?support-solution=General#support)에 문의하십시오.

* 관리자 검색 기능의 여러 요청으로 인해 높은 CPU 사용률이 관찰됩니다. NPR-24229
* 구성 요소를 다시 열 때 PathField가 pathBrowser에서 선택되지 않습니다. NPR-24177

## NPR-27692에 필요한 구성 설정 {#configuration-settings-required-for-npr}

>[!NOTE]
>
>이 구성 설정은 CFP 6.3.3.2 이상에 적용됩니다. `sling`.properties 파일의 부트 위임 속성을 업데이트하도록 안내합니다.

adobe- LiveCycle® - cq -author.ear/ cq .war의 변경 내용을 수동으로 업데이트하려면 아래 설명된 단계를 따르십시오.

* AEM 서버를 중지합니다.
* adobe-livecycle-cq-author.ear/cq.war로 이동합니다.
* 편집할 adobe-livecycle-cq-author.ear/cq.war/WEB-INF/web.xml을 엽니다.

   * **sling.bootdelegation.ibm** param-name 값을 다음과 같이 업데이트합니다.

   * `com.ibm.xml.&#42;,com.ibm.crypto.pkcs11impl.provider,com.ibm.pkcs11,com.ibm.pkcs11.nat`

   * 위와 같이 변경하면 init-param은 다음과 같습니다.

     &lt;init-param>
&lt;param-name>sling.bootdelegation.ibm&lt;/param-name> &lt;param-value>com.ibm.xml.&#42;,com.ibm.crypto.pkcs11impl.provider,com.ibm.pkcs11,com.ibm.pkcs11.nat&lt;/param-value>
&lt;/init-param>

* WebSphere® Application Server에서 이전 엔터프라이즈 아카이브(EAR) 파일을 제거하고 [https://helpx.adobe.com/kr/pdf/aem-forms/6-3/install-single-server-websphere.pdf](https://helpx.adobe.com/kr/pdf/aem-forms/6-3/install-single-server-websphere.pdf)의 섹션 10.2에 나와 있는 단계에 따라 업데이트된 EAR 파일을 설치합니다.
* 파일을 저장하고 서버를 다시 시작합니다. [https://helpx.adobe.com/kr/pdf/aem-forms/6-3/install-single-server-websphere.pdf](https://helpx.adobe.com/kr/pdf/aem-forms/6-3/install-single-server-websphere.pdf)

## NPR-23208에 필요한 구성 설정 {#configuration-settings-required-for-npr-1}

>[!NOTE]
>
>이 구성 설정은 6.3.2.2 이상에 적용됩니다. 이 설정에 따르면 “merge_preserve” acHandling으로 인해 ACL(액세스 제어 목록)이 CFP를 통해 업데이트되지 않으므로 CRX-DE를 통해 수동으로 ACL 정책을 업데이트하도록 안내합니다.

**수동으로 ACL 정책 추가에 대한 설명서**

ACL 정책을 업데이트하려면 CRX-DE를 통해 아래 액세스 제어를 추가합니다.

`1)` “/content” 경로에서
`a)` Principal : reference-adjustment-service
Type : Allow
Privileges : jcr:read, jcr:modifyProperties
Restrictions : rep:glob=&quot;/&#42;/jcr:content&quot;
`b)` Principal : reference-adjustment-service
Type : Allow
Privileges : jcr:read, jcr:modifyProperties
Restrictions : rep:glob=&quot;/&#42;/jcr:content/&#42;&quot;

`2)` “/content/usergenerated” 경로에서
`a)` Principal : reference-adjustment-service
Type : Allow
Privileges : `jcr:write`

`3)` “/etc” 경로에서
`a)` Principal : reference-adjustment-service
Type : Allow
Privileges : jcr:read, jcr:modifyProperties
Restrictions : rep:glob=&quot;/&#42;/jcr:content&quot;
`b)` Principal : reference-adjustment-service
Type : Allow
Privileges : jcr:read, jcr:modifyProperties
Restrictions : rep:glob=&quot;/&#42;/jcr:content/&#42;&quot;

## NPR-19450에 필요한 구성 설정 {#configuration-settings-required-for-npr-2}

>[!NOTE]
>
>이 구성 설정은 CFP 6.3.1.1 이상에 적용됩니다.

**CQ.PAGE_PROPERTIES_MAX_RECURSION_LEVEL 속성을 구성합니다.**

이 속성은 저장소에 있는 노드가 페이지 속성을 가져오는 데 사용될 때까지 페이지 ` /jcr:content` 노드 아래의 노드 하위 트리의 최대 깊이를 제어합니다. 이 속성에 지정된 수준 아래에 있는 노드는 무시됩니다.

기본값은 1입니다. 파일 constants.js(`/libs/cq/ui/widgets/source/constants.js`)를 오버레이하고 `CQ.PAGE_PROPERTIES_MAX_RECURSION_LEVEL` 속성의 주석을 해제하여 값을 재정의합니다. 그런 다음 필요한 값(페이지 속성 데이터가 저장될 때까지 페이지의 `/jcr:content` 아래의 최대 깊이)을 할당합니다.

**페이지의 `/jcr:content` 노드 아래의 노드 수가 1000개를 초과하도록 여러 페이지 변형을 만들어야 하는 경우 다음 단계를 사용하여 구성을 변경합니다.**

* Apache Sling의 속성 JSON 최대 결과를 구성합니다.
* `/system/console/ configMgr`을 사용하여 서블릿 가져오기
* 해당 값을 > 1000(현재 기본값)보다 큰 수로 설정하여 위에 구성된 깊이가 될 때까지 이 수가 / `/jcr:content` 하위 트리의 총 노드 수보다 큰 수가 되도록 합니다.

이 프로세스를 통해 sling GET 서블릿이 모든 필수 노드를 반환할 수 있습니다.

## Uber Jar {#uber-jar}

6.3.3.8용 Uber Jar을 Adobe Public Maven 저장소에서 사용할 수 있습니다.

Maven 프로젝트에서 Uber Jar를 사용하려면 [Uber jar 사용 방법](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)을 참조하여 프로젝트 POM에 다음 종속성을 포함하십시오.

```TXT
<dependency>
 <groupId>com.adobe.aem</groupId>
 <artifactId>uber-jar</artifactId>
 <version>6.3.3.8</version>
 <classifier>apis</classifier>
 <scope>provided</scope>
</dependency>
```

## 제거된/더 이상 사용되지 않는 기능 {#deprecated}

이 섹션에는 AEM 6.3에서 제거되었거나 이제 사용되지 않는 기능이 나와 있습니다.

| 영역 | 기능 | 대체 | 버전 |
|----|-----|-----|-----|
| Assets과 Adobe Creative Cloud 통합 | [AEM과 Creative Cloud 폴더 공유](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)는 Creative 사용자에게 AEM의 자산에 대한 액세스 권한을 제공하는 방법으로 AEM 6.2에 도입되었습니다. Creative Cloud 애플리케이션에서 새롭게 출시된 기능인 Adobe Asset Link는 우수한 사용자 경험을 제공합니다. 또한 Photoshop, InDesign 및 Illustrator에서 직접 AEM 자산에 액세스할 수 있는 강력한 권한을 제공합니다.</br></br> Adobe는 폴더 공유 기능에 대한 추가 개선을 하지 않습니다. 고객은 AEM에 해당 기능이 포함된 동안 교체를 사용해 보시기 바랍니다. | Adobe Asset Link 또는 데스크탑 앱. 자세한 내용은 [AEM Creative Cloud 통합](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions) 문서를 참조하십시오. | AEM 6.3.3.x |

## OSGi 번들 및 콘텐츠 패키지가 포함됨 {#osgi-bundles-and-content-packages-included-1}

다음 텍스트 문서에는 CFP에 포함된 OSGi 번들 및 콘텐츠 패키지가 기재되어 있습니다.

* [AEM 6.3.3.8에 포함된 OSGi 번들 목록](assets/do-not-localize/list_of_osgi_bundlesincludedin6338.txt)

* [AEM 6.3.3.8에 포함된 콘텐츠 패키지 목록](assets/do-not-localize/list_of_content_packageincludedin6338.txt)

>[!MORELIKETHIS]
>
>* [AEM 릴리스 및 업데이트](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/aem-releases-updates)
>* [AEM 6.3 핫픽스 페이지](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/aem-releases-updates)
>* [AEM 6.3 릴리스 정보](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)
>* [AEM 제품 페이지](https://business.adobe.com/products/experience-manager/adobe-experience-manager.html)
>* [AEM 6.3 설명서](https://experienceleague.adobe.com/ko/docs/experience-manager-release-information/aem-release-updates/previous-updates/aem-previous-versions)
>* [Adobe 우선 순위 제품 업데이트](https://www.adobe.com/kr/subscription/priority-product-update.html) 구독
