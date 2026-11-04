# 临床试验注册与结果公开怎么管：FDAAA §801、ClinicalTrials.gov 与 42 CFR Part 11

> 个人学习笔记，不构成法律或医疗建议。本文只讲临床试验的注册与结果公开制度，不评价任何具体试验的疗效与安全性。条文与时限以 eCFR 现行文本、FDA 与 NIH 官方说明为准。全文不写剂量。本仓《临床研究怎么管》一篇讲受试者保护与 IRB，本文专讲注册与公开这一条线，不重复。

## 中文主文

### 一、为什么要有这套制度：试验不能只挑好看的报

临床试验注册与结果公开要解决的是一个老问题：试验做了不登记、结果不好就不发表，公众与医生看到的证据图景就会系统性偏斜。联邦的公开登记底盘分两步搭起来：1997 年《食品药品管理现代化法》先要求为重症疾病设立试验登记库，2007 年《食品药品管理修正法》（FDAAA, Pub. L. 110-85）第 801 节大幅扩围——把登记与结果报告义务写进《公共卫生服务法》§ 402(j)（42 U.S.C. § 282(j)），义务对象从少数试验扩到一大类「适用临床试验」，并配上罚款与资助后果。登记与结果提交的平台是 ClinicalTrials.gov，由国家医学图书馆（National Library of Medicine, NLM，隶属 NIH）运营。2016 年卫生与公众服务部发布最终规则（final rule），把法条落成可执行细则，编为 42 C.F.R. Part 11，2017 年 1 月 18 日生效、2017 年 4 月 18 日为合规日；同日 NIH 另发自家资助政策，把义务再扩一圈（见第六节）。

### 二、谁必须注册：适用临床试验（ACT）的定义

义务的触发点是试验是否属于「适用临床试验」（applicable clinical trial, ACT），定义在 42 U.S.C. § 282(j)(1)(A) 与 42 C.F.R. § 11.10 一线，大意分药物与器械两支：

- **适用药物临床试验**：受 FDA 监管产品的对照临床研究（controlled clinical investigation），但 I 期药物试验除外；
- **适用器械临床试验**：评价器械健康结局的前瞻性临床研究，但小型可行性（small feasibility）研究除外；FDA 依法要求的儿科上市后监测研究也算在内；
- 组合产品按其主要作用模式归入相应一支判定。

不在 ACT 里的试验（比如 I 期药物试验、观察性研究、纯行为干预而无 FDA 监管产品的研究），FDAAA 本身不强制登记——但可能被 NIH 资助政策、期刊投稿要求（ICMJE 把登记作为发表前提）等其他规则够到，判断时要分开看是哪一套规则在问。判定拿不准时，ClinicalTrials.gov 官方提供 ACT 判定清单（checklist）与细化说明，逐项对号，不要凭感觉。

### 三、谁负责：责任方（responsible party）只有一个

登记与报告义务落在「责任方」一个人头上，规则在 42 U.S.C. § 282(j)(1)(A)(ix) 与 42 C.F.R. Part 11：默认是试验的申办方（sponsor）；申办方可以书面指定主要研究者（principal investigator）担任，但被指定者须同时满足四个条件——负责试验的实施、能够接触并控制试验数据、有权发表试验结果、有能力完成全部提交要求。四条缺一，责任仍回到申办方。实务上最常见的事故是申办方与研究者互相以为对方在管，机构层面应以书面指定与内部台账把责任方定死。

### 四、注册时限：首例入组后 21 天

时限口径以 42 C.F.R. § 11.24 为准：责任方须在首例受试者入组（enrollment of the first participant）后不迟于 21 个日历日完成注册提交。注意这是「入组后 21 天」的法定最后线，不是「建议在入组前登记」——期刊与多数机构政策都要求或鼓励入组前先登记，实务上提前做才是稳妥口径，但引用法条时别把两者混成一句。注册信息不是交一次就完：依 § 11.64，登记信息至少每 12 个月复核更新一次，其中招募状态变化、试验完成等特定要素须在变化后 30 天内更新；平台审核退回的问题要在规定时限内更正回应。

### 五、结果时限：主要完成日期后 12 个月，延期有明文通道

结果信息（results information）的标准时限在 42 C.F.R. § 11.44(a)：不迟于主要完成日期（primary completion date）后 1 年提交。先对齐这个日期的定义：最后一名受试者为主要结局的最终数据收集而接受检查或干预的日期，试验按方案完成还是提前终止都一样算；提前终止的试验同样要交结果，不是只有「做成」的试验才交。

赶不上标准时限时，规则给了明文延期通道，但都要走认证或申请程序、不是自动顺延：

- **认证延期一（§ 11.44(b)）**：所研究产品此前已获批/许可/准市，现为新用途寻求批准的，可提交认证延后结果公开，截止点与认证后发生的特定事件挂钩，自认证提交之日起最长不超过 2 年；
- **认证延期二（§ 11.44(c)）**：所研究产品尚未获批、正在寻求首次批准/许可/准市的，同样可认证延期，上限口径同为认证后最长 2 年一线；
- **良好事由延期（good cause extension）**：不属于上两类的特殊情形，可依规则向 NIH 提出延期申请并说明理由，批不批由官方裁量，不写申请等于没有延期。

结果提交的内容是结构化汇总结果（受试者流动、各结局指标、不良事件等模块），走 ClinicalTrials.gov 的协议注册与结果系统（PRS）录入，经平台质检后公开；提交的是汇总数据，不是逐个受试者的原始记录。

### 六、NIH 2017 政策：资助口径比法条再宽一圈

与最终规则同日发布的《NIH 资助临床试验信息传播政策》（NIH Policy on Dissemination of NIH-funded Clinical Trial Information, NOT-OD-16-149）是政策、不是法规，约束力来自资助条件本身：凡 NIH 全部或部分资助的临床试验——不论期别、不论干预类型、不论是否属于 ACT——都要在 ClinicalTrials.gov 登记并提交结果，适用于 2017 年 1 月 18 日及以后提交的资助申请。时限与法规同构：入组后 21 天内登记、主要完成日期后 1 年内交结果。实务后果是：一个 I 期药物试验可能不欠 FDAAA 的账，却欠 NIH 政策的账；只按 ACT 定义判断义务、漏掉资助政策，是学术机构最常见的合规缺口。执行抓手也在资助端：NIH 可因登记或结果不合规而暂停或终止资助、影响后续拨款，机构层面的合规核验写在资助条款里。

### 七、罚则与执行：FDA 执法、平台标注、资助后果三管齐下

- **民事罚款**：未登记、未提交结果信息或提交虚假误导信息，是《食品、药品和化妆品法》下的禁止行为；罚款口径依 42 U.S.C. § 282(j)(5) 与 FDCA 罚则一线：经程序认定违规可处 10,000 美元量级的罚款（法定基数），收到不合规通知后仍不改正的，按日再罚 10,000 美元量级直至改正，具体金额经通胀调整、以 FDA 当期执法文件为准，本文只记量级不写死当年数字。
- **执法路径**：FDA 是 FDAAA 登记义务的执法机关（HHS 已将该执法权授予 FDA），路径大致是先发不合规通知（Notice of Noncompliance）给改正机会，再决定是否罚款；试验记录上会被标注未合规状态，公众在 ClinicalTrials.gov 上看得见。
- **许可与资助的连带**：向 FDA 提交药品或器械上市申请时，须就所涉适用临床试验的登记与结果合规提交认证（实务上用 Form FDA 3674）；联邦资助的试验不合规，可招致资助扣留或追回。历史执行强度曾长期偏弱、近年 FDA 发出的不合规通知增多，引用执行现状时以 FDA 官方清单当期状态为准，不把个案写成普遍结论。

### 八、FDA 与 NIH 的分工：一句话对照

平台是 NIH 的（NLM 运营 ClinicalTrials.gov、负责登记系统与数据公开），规则是 HHS 定的（42 C.F.R. Part 11），FDAAA 的执法是 FDA 的（通知与罚款），NIH 政策那一圈由 NIH 自己用资助条件执行。四家名字常被混写，记成「NIH 建库收数、FDA 执法罚款、NIH 另管自家钱袋」就不会乱。本仓读者若是患者或家属：查一个试验登没登记、结果交没交，直接在 ClinicalTrials.gov 按登记号（NCT 编号）或疾病与机构检索，记录页会显示注册日期、更新历史与结果提交状态，这比任何二手转述都硬。

### 九、加州一格：无独立试验注册法

加州没有另设一套临床试验注册法，也没有州级的试验注册数据库——在加州开展的试验，注册与结果公开同样走联邦 ClinicalTrials.gov 这一条线，按 ACT 定义与 NIH 政策判断义务。加州自有的一层落在受试者保护而不是注册：《加州人体医学实验受试者保护法》（Health & Safety Code §§ 24170 起，含实验受试者权利法案）在知情同意与受试者权利上给加州参与者加了一层州法保障，它与联邦 Common Rule、FDA 受试者保护规则并行，但不产生第二个登记动作。州层面对研究机构的管理主要经 IRB 与机构政策落地，研究者在加州判断义务时，先联邦后州法、别到州法里找不存在的注册条款。

### 十、易错点清单

- 易错一：把「21 天」说成入组前登记——法定线是首例入组后 21 天内，入组前登记是期刊与机构的更严口径。
- 易错二：以为只有获批产品的试验才交结果——42 C.F.R. Part 11 口径下 ACT 原则上都要交结果，产品未获批走的是认证延期、不是免交。
- 易错三：以为提前终止就不用交结果——终止试验同样在 12 个月时限内。
- 易错四：只查 ACT、漏查 NIH 政策——NIH 资助的非 ACT 试验同样欠登记与结果。
- 易错五：以为罚则只是吓唬——罚款、记录标注与资助后果是三条独立的线，任何一条落地都是实质代价。

*声明：个人学习笔记，不构成法律或医疗建议。来源：FDAAA § 801（Pub. L. 110-85）与 42 U.S.C. § 282(j)；42 C.F.R. Part 11（§§ 11.10、11.24、11.44、11.64）；NIH 政策通知 NOT-OD-16-149 与 ClinicalTrials.gov 官方说明；FDA 关于登记合规与不合规通知的官方口径；加州 Health & Safety Code §§ 24170 起。具体以 eCFR 与各机构当期官方文本为准。全文不写剂量。*

---

## English

Clinical trial registration and results reporting in the United States rest on Section 801 of the FDA Amendments Act of 2007 (FDAAA), codified at 42 U.S.C. § 282(j), and implemented by the HHS final rule at 42 CFR Part 11 (effective January 18, 2017, compliance date April 18, 2017). The duty applies to "applicable clinical trials" (ACTs) as defined at 42 CFR § 11.10: controlled clinical investigations of FDA-regulated drugs other than phase 1 trials, and prospective clinical studies of health outcomes for devices other than small feasibility studies, including FDA-required pediatric postmarket surveillance. One "responsible party" bears the duty — the sponsor by default, or a principal investigator designated in writing only if the investigator runs the trial, controls the data, holds publication rights, and can meet all submission requirements. Registration is due not later than 21 calendar days after enrollment of the first participant (42 CFR § 11.24); records must be updated at least every 12 months, with specified elements such as recruitment status updated within 30 days (§ 11.64). Results information is due not later than one year after the primary completion date (§ 11.44(a)), including for trials terminated early. Two certification-based delays are available — for a new use of an already approved product (§ 11.44(b)) and for initial approval of an unapproved product (§ 11.44(c)), each capped at two years after certification — plus a discretionary good-cause extension. ClinicalTrials.gov itself is operated by the National Library of Medicine within NIH; FDA enforces FDAAA (notices of noncompliance, then civil money penalties on the order of $10,000, with additional per-day penalties after notice, inflation-adjusted), noncompliant records are flagged publicly, grant funds can be withheld, and marketing applications must certify compliance (Form FDA 3674). Separately, the NIH policy on dissemination of NIH-funded clinical trial information (NOT-OD-16-149) applies to funding applications submitted on or after January 18, 2017 and reaches every NIH-funded clinical trial regardless of phase, intervention type, or ACT status, on the same 21-day and one-year timelines, enforced through funding terms. California has no clinical trial registration statute or state registry of its own — trials in California register federally — while its Human Subjects in Medical Experiments law (Health & Safety Code §§ 24170 et seq.) adds a state layer on consent and subject rights, not a second registration duty. *Personal study notes only, not legal or medical advice. No dosages are given anywhere in this article.*

## Español (traducción de estudio, pendiente de revisión nativa)

El registro de ensayos clínicos y la publicación de resultados en Estados Unidos descansan en la sección 801 de la FDA Amendments Act de 2007 (FDAAA), codificada en 42 U.S.C. § 282(j), y desarrollada por la regla final de HHS en 42 CFR Parte 11 (en vigor desde el 18 de enero de 2017, con fecha de cumplimiento el 18 de abril de 2017). La obligación recae sobre los «ensayos clínicos aplicables» (ACT) definidos en 42 CFR § 11.10: investigaciones clínicas controladas de medicamentos regulados por la FDA, salvo los ensayos de fase 1, y estudios clínicos prospectivos de resultados en salud con dispositivos, salvo los pequeños estudios de viabilidad, incluida la vigilancia pediátrica poscomercialización exigida por la FDA. Responde una sola «parte responsable»: el patrocinador por defecto, o un investigador principal designado por escrito solo si dirige el ensayo, controla los datos, tiene derecho a publicar y puede cumplir todos los requisitos de envío. El registro vence a más tardar 21 días naturales después de la inscripción del primer participante (42 CFR § 11.24); el registro debe actualizarse al menos cada 12 meses, y ciertos elementos, como el estado de reclutamiento, dentro de los 30 días (§ 11.64). Los resultados vencen a más tardar un año después de la fecha de finalización primaria (§ 11.44(a)), también en ensayos terminados antes de tiempo. Existen dos demoras por certificación —nuevo uso de un producto ya aprobado (§ 11.44(b)) y aprobación inicial de un producto no aprobado (§ 11.44(c)), cada una con tope de dos años desde la certificación— y una prórroga discrecional por buena causa. ClinicalTrials.gov lo opera la National Library of Medicine, dentro de NIH; la FDA hace cumplir la FDAAA (avisos de incumplimiento y luego sanciones civiles del orden de 10.000 dólares, con multas diarias adicionales tras la notificación, ajustadas por inflación), los registros incumplidores se marcan públicamente, los fondos de subvenciones pueden retenerse y las solicitudes de comercialización deben certificar el cumplimiento (Formulario FDA 3674). Por separado, la política de NIH sobre difusión de información de ensayos financiados por NIH (NOT-OD-16-149) se aplica a solicitudes de financiación presentadas desde el 18 de enero de 2017 y alcanza a todo ensayo financiado por NIH sin importar fase, tipo de intervención o condición de ACT, con los mismos plazos de 21 días y un año, exigida mediante las condiciones de la subvención. California no tiene ley estatal de registro de ensayos ni registro propio —los ensayos en California se registran en el sistema federal—, mientras que su ley de sujetos humanos en experimentos médicos (Health & Safety Code §§ 24170 y siguientes) añade una capa estatal sobre consentimiento y derechos del participante, no un segundo registro. *Notas personales de estudio; no es consejo legal ni médico. Este artículo no indica dosis.*

## 한국어 (초역, 원어민 감수 대기)

미국의 임상시험 등록과 결과 공개는 2007년 FDA 개정법(FDAAA) §801(42 U.S.C. § 282(j))과 이를 시행하는 HHS 최종 규칙 42 CFR Part 11(2017년 1월 18일 발효, 같은 해 4월 18일 준수일)에 근거합니다. 의무는 42 CFR § 11.10이 정의하는 '적용 임상시험(ACT)'에 적용됩니다. FDA 규제 약물의 1상을 제외한 대조 임상 연구, 소규모 타당성 연구를 제외한 의료기기의 건강 결과에 대한 전향적 임상 연구, 그리고 FDA가 요구하는 소아 시판 후 감시가 포함됩니다. '책임 당사자'는 하나뿐입니다. 기본은 의뢰자(sponsor)이고, 주요 연구자는 서면 지정을 받더라도 시험 실시 책임, 데이터 접근·통제, 결과 발표권, 제출 요건 이행 능력을 모두 갖출 때만 될 수 있습니다. 등록은 첫 참여자 등록 후 21일(역일) 이내가 기한입니다(42 CFR § 11.24). 기록은 최소 12개월마다 갱신하고 모집 상태 등 특정 요소는 30일 이내에 갱신합니다(§ 11.64). 결과 정보는 주요 완료일 후 1년 이내가 기한이며(§ 11.44(a)), 조기 종료된 시험도 마찬가지입니다. 인증 기반 연기가 두 가지 있습니다. 이미 승인된 제품의 새 용도에 대한 것(§ 11.44(b))과 미승인 제품의 최초 승인에 대한 것(§ 11.44(c))으로 각각 인증 후 최대 2년이며, 재량적인 정당한 사유 연기도 있습니다. ClinicalTrials.gov는 NIH 산하 National Library of Medicine이 운영합니다. FDA가 FDAAA를 집행하는데, 불이행 통지 후 1만 달러 수준의 민사 벌금(통지 후에는 일 단위 추가 벌금, 인플레이션 조정)이 가능하고, 불이행 기록은 공개적으로 표시되며, 연구비 보류와 시판 신청 시 준수 인증(Form FDA 3674)이 뒤따릅니다. 별도로 NIH 자금 지원 임상시험 정보 공개 정책(NOT-OD-16-149)은 2017년 1월 18일 이후 제출된 신청에 적용되며, 상(phase)·개입 유형·ACT 해당 여부와 무관하게 모든 NIH 지원 시험에 동일한 21일·1년 기한을 적용하고 자금 조건으로 집행합니다. 캘리포니아에는 주 자체의 임상시험 등록법이나 등록부가 없어 캘리포니아 시험도 연방 시스템에 등록합니다. 주법인 의학실험 피험자법(Health & Safety Code §§ 24170 이하)은 동의와 피험자 권리에 주 차원의 층을 더할 뿐 두 번째 등록 의무를 만들지 않습니다. *개인 학습 노트이며 법률·의료 자문이 아닙니다. 본 글에는 용량을 기재하지 않습니다. (초역 · 初译待校)*

## Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

Việc đăng ký thử nghiệm lâm sàng và công bố kết quả tại Hoa Kỳ dựa trên Điều 801 của Đạo luật Sửa đổi FDA năm 2007 (FDAAA), được luật hóa tại 42 U.S.C. § 282(j), và được triển khai bởi quy tắc cuối cùng của HHS tại 42 CFR Phần 11 (hiệu lực 18 tháng 1 năm 2017, ngày tuân thủ 18 tháng 4 năm 2017). Nghĩa vụ áp dụng cho các «thử nghiệm lâm sàng thuộc diện áp dụng» (ACT) theo định nghĩa tại 42 CFR § 11.10: nghiên cứu lâm sàng có đối chứng với thuốc chịu quản lý của FDA, trừ thử nghiệm giai đoạn 1, và nghiên cứu lâm sàng tiến cứu về kết cục sức khỏe của thiết bị, trừ nghiên cứu khả thi quy mô nhỏ, bao gồm cả giám sát hậu mại nhi khoa do FDA yêu cầu. Chỉ có một «bên chịu trách nhiệm»: mặc định là nhà tài trợ, hoặc nghiên cứu viên chính được chỉ định bằng văn bản chỉ khi người đó điều hành thử nghiệm, kiểm soát dữ liệu, có quyền công bố kết quả và có khả năng đáp ứng mọi yêu cầu nộp hồ sơ. Đăng ký phải hoàn thành không muộn hơn 21 ngày lịch sau khi tuyển người tham gia đầu tiên (42 CFR § 11.24); hồ sơ phải được cập nhật ít nhất mỗi 12 tháng, và một số yếu tố như tình trạng tuyển mộ phải cập nhật trong vòng 30 ngày (§ 11.64). Thông tin kết quả phải nộp không muộn hơn một năm sau ngày hoàn thành chính (§ 11.44(a)), kể cả với thử nghiệm chấm dứt sớm. Có hai cơ chế trì hoãn theo chứng nhận — công dụng mới của sản phẩm đã được phê duyệt (§ 11.44(b)) và phê duyệt lần đầu của sản phẩm chưa được phê duyệt (§ 11.44(c)), mỗi cơ chế tối đa hai năm kể từ ngày chứng nhận — cùng cơ chế gia hạn vì lý do chính đáng theo xét duyệt. ClinicalTrials.gov do Thư viện Y khoa Quốc gia thuộc NIH vận hành; FDA thực thi FDAAA (thông báo không tuân thủ, rồi phạt tiền dân sự ở mức khoảng 10.000 đô la, cộng thêm phạt theo ngày sau khi đã thông báo, có điều chỉnh theo lạm phát), hồ sơ không tuân thủ bị đánh dấu công khai, kinh phí tài trợ có thể bị giữ lại, và hồ sơ xin lưu hành phải chứng nhận tuân thủ (Mẫu FDA 3674). Riêng chính sách của NIH về phổ biến thông tin thử nghiệm lâm sàng do NIH tài trợ (NOT-OD-16-149) áp dụng cho đơn xin tài trợ nộp từ 18 tháng 1 năm 2017 và bao phủ mọi thử nghiệm được NIH tài trợ bất kể giai đoạn, loại can thiệp hay tư cách ACT, với cùng mốc 21 ngày và một năm, được thực thi qua điều kiện tài trợ. California không có luật đăng ký thử nghiệm lâm sàng hay sổ đăng ký riêng của bang — thử nghiệm tại California đăng ký theo hệ thống liên bang — trong khi luật của bang về đối tượng con người trong thí nghiệm y khoa (Health & Safety Code §§ 24170 trở đi) bổ sung một tầng bảo vệ về đồng ý và quyền của người tham gia, chứ không tạo thêm nghĩa vụ đăng ký thứ hai. *Ghi chú học tập cá nhân, không phải tư vấn pháp lý hay y tế. Bài này không ghi liều lượng. (bản dịch sơ bộ · 初译待校)*

## हिन्दी (प्रारंभिक अनुवाद, मूल-भाषी समीक्षा लंबित)

संयुक्त राज्य में नैदानिक परीक्षणों का पंजीकरण और परिणामों का प्रकटीकरण FDA Amendments Act 2007 (FDAAA) की धारा 801 पर आधारित है, जो 42 U.S.C. § 282(j) में संहिताबद्ध है, और HHS के अंतिम नियम 42 CFR Part 11 (18 जनवरी 2017 से प्रभावी, अनुपालन तिथि 18 अप्रैल 2017) से लागू होता है। यह दायित्व 42 CFR § 11.10 में परिभाषित «applicable clinical trials» (ACT) पर लगता है: चरण 1 परीक्षणों को छोड़कर FDA-विनियमित दवाओं की नियंत्रित नैदानिक जाँचें, और छोटे व्यवहार्यता अध्ययनों को छोड़कर उपकरणों के स्वास्थ्य-परिणामों के prospective नैदानिक अध्ययन, जिनमें FDA द्वारा अपेक्षित बाल-चिकित्सा postmarket surveillance भी शामिल है। «Responsible party» केवल एक होता है — डिफ़ॉल्ट रूप से sponsor, या लिखित रूप से नामित principal investigator, और वह भी तभी जब वह परीक्षण चलाता हो, डेटा पर नियंत्रण रखता हो, परिणाम प्रकाशित करने का अधिकार रखता हो और सभी जमा-शर्तें पूरी कर सकता हो। पंजीकरण की अंतिम तिथि पहले प्रतिभागी के नामांकन के बाद अधिकतम 21 कैलेंडर दिन है (42 CFR § 11.24); अभिलेख कम से कम हर 12 महीने में अद्यतन किए जाने चाहिए, और भर्ती-स्थिति जैसे निर्दिष्ट तत्व 30 दिनों के भीतर (§ 11.64)। परिणाम-जानकारी primary completion date के बाद अधिकतम एक वर्ष में देनी होती है (§ 11.44(a)), समय से पहले समाप्त परीक्षणों के लिए भी। प्रमाणन-आधारित दो विलंब उपलब्ध हैं — पहले से अनुमोदित उत्पाद के नए उपयोग के लिए (§ 11.44(b)) और अनुमोदित न हुए उत्पाद के प्रारंभिक अनुमोदन के लिए (§ 11.44(c)), दोनों की सीमा प्रमाणन के बाद अधिकतम दो वर्ष है — साथ ही विवेकाधीन good-cause विस्तार भी है। ClinicalTrials.gov का संचालन NIH के अंतर्गत National Library of Medicine करता है; FDAAA का प्रवर्तन FDA करता है (गैर-अनुपालन की सूचना, फिर लगभग 10,000 डॉलर के क्रम के civil money penalties, सूचना के बाद प्रतिदिन अतिरिक्त दंड, मुद्रास्फीति-समायोजित), गैर-अनुपालन वाले अभिलेख सार्वजनिक रूप से चिह्नित होते हैं, अनुदान रोका जा सकता है, और विपणन आवेदनों को अनुपालन प्रमाणित करना होता है (Form FDA 3674)। अलग से, NIH-वित्तपोषित नैदानिक परीक्षण जानकारी के प्रसार पर NIH नीति (NOT-OD-16-149) 18 जनवरी 2017 को या उसके बाद जमा किए गए वित्तपोषण आवेदनों पर लागू होती है और चरण, हस्तक्षेप के प्रकार या ACT स्थिति की परवाह किए बिना हर NIH-वित्तपोषित परीक्षण तक पहुँचती है, उन्हीं 21-दिन और एक-वर्ष की समय-सीमाओं के साथ, और वित्तपोषण शर्तों से लागू होती है। California के पास अपना नैदानिक परीक्षण पंजीकरण कानून या राज्य रजिस्ट्री नहीं है — California के परीक्षण संघीय प्रणाली में ही पंजीकृत होते हैं — जबकि चिकित्सा प्रयोगों में मानव विषयों पर उसका कानून (Health & Safety Code §§ 24170 आगे) सहमति और प्रतिभागी अधिकारों पर राज्य-स्तर जोड़ता है, दूसरा पंजीकरण दायित्व नहीं बनाता। *व्यक्तिगत अध्ययन नोट; कानूनी या चिकित्सा सलाह नहीं। इस लेख में कोई खुराक नहीं दी गई है। (प्रारंभिक अनुवाद · 初译待校)*

---

*声明：个人学习笔记，不构成法律、税务或医疗建议（personal study notes only; not legal, tax, or medical advice）。*
