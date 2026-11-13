# 疫苗不良事件报告 VAERS 怎么管：联邦监测系统、法定报告义务与加州衔接

> 选题说明：医疗法律法规板块。本轮法规候选三题经 ls/grep 实查：「医疗机构语言服务与口译权利」仓内已有《医疗中的残疾与语言权利怎么管》专篇（含 ACA 第 1557 条语言服务整节），撞题弃用；「处方药折扣卡与 copay accumulator」已有流程专篇与 PBM 法规篇覆盖大半，未选；「疫苗不良事件报告 VAERS」全仓无本体——仅在《疫苗伤害补偿怎么管 VICP》篇第五节与药房打疫苗流程篇各作一句邻居提及，故成篇，与 VICP 篇以指针分工：那篇管伤害补偿怎么赔，本篇管不良事件怎么报、谁必须报、报上去的数据能说明什么与不能说明什么。事实经 HHS/CDC 的 VAERS 官方页面与《美国法典》第 42 卷原文回核。

## 中文主文

### 一、先定性：VAERS 是监测的耳朵，不是定责的法庭

疫苗不良事件报告系统（Vaccine Adverse Event Reporting System, VAERS）是美国的全国性疫苗安全监测系统，1990 年起运行，由疾病控制与预防中心（CDC）与食品药品监督管理局（FDA）共同管理。它的法律出身是 1986 年《国家儿童疫苗伤害法》（National Childhood Vaccine Injury Act, NCVIA），成文于《美国法典》第 42 卷第 300aa-1 条起。定性先钉死三句：VAERS 收集的是「报告」，不是「结论」；它负责听见异常信号，不负责判定某支疫苗是否造成了某个事件；报告本身未经核实，CDC 的 WONDER 数据库页面把话说在前面——VAERS 报告可能不完整、不准确、属巧合或无法核实，单凭报告数量不能证明因果关系，也不能算出事件发生率。

### 二、谁必须报：法定义务在第 300aa-25 条

报告义务分两摊。记录摊在第 300aa-25 条第 (a) 款：接种方必须在受种者的永久病历里记下四样——接种日期、疫苗生产企业与批号、接种执行人的姓名地址与职务。报告摊在第 (b) 款：每一名医疗服务提供者与每一家疫苗生产企业，都必须报告三类事项——(A)《疫苗伤害表》所列事件，包括第 300aa-14 条第 (b) 款情形，时限为事件发生后 7 天内或伤害表规定的更长期间；(B) 生产企业说明书中列明的禁忌反应；(C) 法规另行要求的其他事项。注意这条义务不挑疫苗品种的年龄段，条文覆盖的是依法进入该框架的疫苗接种活动；企业一侧另有《联邦法规汇编》第 21 卷第 600.80 条，要求生产企业把获知的不良事件报给 FDA。

### 三、两个「表」不要混：报告事件表与伤害表不是一回事

VAERS 官网专门立了一张《接种后可报告事件表》（Table of Reportable Events Following Vaccination, RET），并明说它与《疫苗伤害表》（Vaccine Injury Table, VIT）是两张不同的表。分工是：RET 回答「什么必须报」——它反映第 300aa-25 条的法定报告口径，表上的时间窗是报告时限；VIT 回答「什么推定可赔」——它服务于 VICP 补偿程序的因果推定，时间窗是补偿口径。把两张表混用是最常见的误读：某事件在 RET 上，不等于它在 VIT 上，更不等于已经认定疫苗致害。顺带把第三个邻居分清：接种前发给受种者的《疫苗信息声明》（VIS）出自第 300aa-26 条，是告知文件，不是不良事件报告。

### 四、谁都可以报，报了会怎样

除了法定义务人，人人可报：医疗人员、生产企业、受种者本人与家属、公众，都可以在 vaers.hhs.gov 提交报告；CDC 与 FDA 官方口径还鼓励医疗人员把临床上重要或意料之外的事件报上去，哪怕不确定与疫苗有没有关系。数据一侧：VAERS 数据自 1990 年至今公开可查，公开的是原始报告数据。信号处理一侧：报告汇成异常模式（unusual pattern）时，才触发进一步分析——CDC 一侧有疫苗安全数据链（Vaccine Safety Datalink, VSD）与临床免疫安全评估项目（CISA），FDA 一侧有 BEST 系统，这些主动监测与病历级核查系统才是把「相关性怀疑」往因果判断推进的工具。另有两头要说清：一是明知虚假仍提交 VAERS 报告，触犯《美国法典》第 18 卷第 1001 条（虚假陈述）；二是 CDC 与 FDA 不就某一份报告向个人提供医疗建议，个人诊疗问题回到自己的医生那里。把账算一遍：系统 1990 年运行至今，2026 减 1990 等于 36 年数据；共同管理的联邦机构 2 家；法定职能一句话——它是一台信号探测器，不是一台因果判决机。

### 五、与 VICP 的分工：报告不自动变索赔

在接种点最容易发生的误会，是以为报了 VAERS 就等于启动了补偿。两条线并行不互通：VAERS 是安全监测线，目的是发现信号，任何人可报、不设索赔资格审查；VICP 是补偿线，走《疫苗伤害表》与联邦索赔法院（Court of Federal Claims）的请愿程序，有资格与时限门槛，细节见本仓《疫苗伤害补偿怎么管》专篇。实务顺序因此是：发生疑似不良事件，先救治、再按第 300aa-25 条记全病历四要素并依法报告 VAERS；要谈补偿，再单独评估 VICP 请愿。报告 VAERS 不影响请愿资格，不报也不在文本上直接剥夺请愿权，但病历与报告记录会成为后续任何程序里最基础的事实底盘——这正是第 (a) 款把接种日期、企业与批号、接种者信息钉进永久病历的原因。

### 六、加州衔接：报告走联邦系统，加州另有免疫登记账

加州没有一套与 VAERS 并行的州级不良事件报告系统：不良事件报告走联邦 VAERS 这一条口子。加州自己的账在另一侧——接种剂次记录进入加州免疫登记系统（California Immunization Registry, CAIR），那是「谁打了哪一针」的接种账，不是「打完出了什么事」的不良事件账，两本账不要混。药房场景的州法底盘仍在本仓药房打疫苗流程篇：药剂师接种权限出自《商业与职业法典》第 4052.8 条一带，接种前发 VIS、接种后依法记录与报告的义务，与本篇第 300aa-25 条的联邦记录与报告义务叠在一起执行。学校与托幼场景的免疫要求与医疗豁免走本仓《疫苗要求怎么管》篇，不在本篇范围。

### 七、读 VAERS 数据的纪律：给学习者的四条

一是任何人引用 VAERS 数字下因果结论，先回到 CDC 的免责口径：报告未经核实、不能单独证明因果、不能算发生率。二是看信号不看绝对数：系统价值在异常模式触发 VSD、CISA、BEST 等核查，而不是某个事件的报告条数本身。三是区分三张纸：RET（必须报什么）、VIT（推定赔什么）、VIS（接种前告知什么）。四是回到记录源头：批号、企业、日期、接种者这四样在接种当场记全，事后任何监测与补偿程序都站在这一页病历上。来源：HHS 的 VAERS 官网（vaers.hhs.gov）与《接种后可报告事件表》、CDC WONDER 的 VAERS 数据说明、《美国法典》第 42 卷第 300aa-25 条与第 300aa-26 条、《联邦法规汇编》第 21 卷第 600.80 条、《美国法典》第 18 卷第 1001 条。

## English

### How Vaccine Adverse Event Reporting (VAERS) Is Governed: The Federal Monitoring System, Statutory Reporting Duties and the California Connection

Topic check: of the three regulatory candidates this round, the language-services topic already has a dedicated article in this repo (the ADA/Section 504/ACA Section 1557 piece) and the copay-accumulator topic is largely covered by an existing process article and the PBM article; VAERS has no article of its own — it appears only as a one-line neighbor mention in the VICP compensation article and the pharmacy vaccination article — so it is taken here, cross-referencing the VICP piece: that one covers compensation; this one covers reporting.

1. Nature. The Vaccine Adverse Event Reporting System (VAERS) is the national vaccine-safety monitoring system, operating since 1990 and co-managed by the CDC and the FDA. Its statutory home is the National Childhood Vaccine Injury Act of 1986, at 42 U.S.C. sections 300aa-1 et seq. Three sentences fix its character: VAERS collects reports, not conclusions; it listens for unusual signals rather than deciding whether a vaccine caused an event; and its reports are unverified — CDC's WONDER documentation states that reports may be incomplete, inaccurate, coincidental or unverifiable, and that report counts alone cannot establish causation or incidence rates.

2. Who must report. 42 U.S.C. section 300aa-25(a) requires the administering provider to record in the recipient's permanent medical record the date of administration, the vaccine manufacturer and lot number, and the name, address and title of the person administering it. Section 300aa-25(b) requires each health care provider and each vaccine manufacturer to report (A) events in the Vaccine Injury Table, including events under section 300aa-14(b), within 7 days or any longer Table period, (B) contraindicating reactions specified in the manufacturer's package insert, and (C) other matters required by regulation. Manufacturers additionally report all adverse events made known to them to FDA under 21 C.F.R. section 600.80.

3. Two tables, not one. The VAERS Table of Reportable Events Following Vaccination (RET) states what must be reported under section 300aa-25, and VAERS itself notes it differs from the Vaccine Injury Table (VIT): RET timeframes are reporting windows, VIT timeframes serve the compensation presumption in VICP. An event's place on the RET does not put it on the VIT and does not establish that a vaccine caused harm. A third neighbor document, the Vaccine Information Statement (VIS) under section 300aa-26, is pre-vaccination information, not a report.

4. Anyone may report, and what happens next. Providers, manufacturers, recipients, families and the public may all file at vaers.hhs.gov, and health professionals are encouraged to report clinically significant or unexpected events even when unsure of causation. Public data cover 1990 to the present and consist of initial reports. Only an unusual pattern triggers deeper analysis — CDC's Vaccine Safety Datalink (VSD) and CISA Project, and FDA's BEST system — which are the chart-level tools that move a suspicion toward a causal assessment. Knowingly filing a false VAERS report violates 18 U.S.C. section 1001, and CDC/FDA do not provide individual medical advice about a report. The arithmetic: 2026 minus 1990 equals 36 years of data, 2 co-managing federal agencies, and one statutory job — a signal detector, not a causation machine.

5. Reporting is not claiming. VAERS (monitoring, open to anyone) and VICP (compensation, through the Vaccine Injury Table and a petition in the Court of Federal Claims, with eligibility and deadline gates — see this repo's VICP article) run in parallel and do not convert into each other. The practical order: treat first, then record the four section 300aa-25(a) elements and report to VAERS as the law requires; assess a VICP petition separately. The record and the report become the factual base of any later proceeding, which is why the statute pins them into the permanent medical record.

6. California. California runs no parallel state adverse-event system: reports go to federal VAERS. The state's own ledger is different — doses go into the California Immunization Registry (CAIR), a record of who received which dose, not an adverse-event ledger. Pharmacy vaccination authority sits in Business and Professions Code section 4052.8 territory (see this repo's pharmacy vaccination article), and the federal recording and reporting duties of section 300aa-25 apply on top. School and childcare immunization requirements and medical exemptions are covered by this repo's vaccine-requirements article.

7. Reading discipline. Four rules: never draw a causal conclusion from VAERS numbers without the CDC caveats (unverified, cannot alone prove causation, cannot yield rates); read signals, not raw counts — the system's value is patterns triggering VSD, CISA or BEST review; keep the three documents separate (RET, VIT, VIS); and go back to the source record — lot number, manufacturer, date and administrator, recorded completely at the visit, are what every later monitoring or compensation step stands on. Sources: vaers.hhs.gov and its Table of Reportable Events Following Vaccination, CDC WONDER VAERS documentation, 42 U.S.C. sections 300aa-25 and 300aa-26, 21 C.F.R. section 600.80, and 18 U.S.C. section 1001.

## Español (traducción inicial · 初译待校)

### Cómo se rige el reporte de eventos adversos de vacunas (VAERS): el sistema federal de vigilancia, los deberes legales de reporte y la conexión con California

Verificación de tema: de los tres candidatos regulatorios de esta ronda, el de servicios de lenguaje ya tiene artículo propio en este repositorio y el de acumuladores de copago está en gran parte cubierto; VAERS no tiene artículo propio —solo aparece como mención breve en el artículo de compensación VICP y en el de vacunación en farmacias—, así que se desarrolla aquí.

1. Naturaleza. El Vaccine Adverse Event Reporting System (VAERS) es el sistema nacional de vigilancia de seguridad de vacunas, en funcionamiento desde 1990 y cogestionado por los CDC y la FDA. Su base legal es la National Childhood Vaccine Injury Act de 1986, en el título 42 del U.S. Code, artículos 300aa-1 y siguientes. Tres frases fijan su carácter: VAERS recoge informes, no conclusiones; escucha señales inusuales en lugar de decidir si una vacuna causó un evento; y sus informes no están verificados —la documentación de CDC WONDER advierte que los informes pueden ser incompletos, inexactos, coincidentes o no verificables, y que el número de informes por sí solo no prueba causalidad ni permite calcular tasas de incidencia—.

2. Quién debe reportar. El artículo 300aa-25(a) exige que quien administra registre en la historia clínica permanente del receptor la fecha de administración, el fabricante de la vacuna y el número de lote, y el nombre, la dirección y el cargo de quien administra. El apartado (b) exige a cada proveedor de salud y a cada fabricante reportar: (A) los eventos de la Vaccine Injury Table, incluidos los del artículo 300aa-14(b), dentro de los 7 días o el plazo mayor que fije la tabla; (B) las reacciones contraindicantes indicadas en el prospecto del fabricante; y (C) otros asuntos exigidos por reglamento. Los fabricantes reportan además a la FDA todos los eventos adversos de los que tengan conocimiento, conforme a 21 C.F.R. 600.80.

3. Dos tablas, no una. La tabla de eventos reportables tras la vacunación (RET) de VAERS indica qué debe reportarse según el artículo 300aa-25, y el propio VAERS subraya que difiere de la Vaccine Injury Table (VIT): los plazos de la RET son ventanas de reporte y los de la VIT sirven a la presunción de compensación del VICP. Que un evento figure en la RET no lo coloca en la VIT ni establece que una vacuna haya causado daño. Un tercer documento vecino, la hoja de información sobre vacunas (VIS) del artículo 300aa-26, es información previa a la vacunación, no un informe.

4. Cualquiera puede reportar, y qué sigue. Proveedores, fabricantes, receptores, familias y el público pueden presentar informes en vaers.hhs.gov, y se anima a los profesionales de salud a reportar eventos clínicamente importantes o inesperados aunque no estén seguros de la causalidad. Los datos públicos abarcan de 1990 a la actualidad y son informes iniciales. Solo un patrón inusual dispara un análisis más profundo —el Vaccine Safety Datalink (VSD) y el proyecto CISA de los CDC, y el sistema BEST de la FDA—, que son las herramientas a nivel de historia clínica que acercan una sospecha a una valoración causal. Presentar a sabiendas un informe falso en VAERS viola el artículo 1001 del título 18 del U.S. Code, y los CDC y la FDA no ofrecen asesoría médica individual sobre un informe. La cuenta: 2026 menos 1990 igual a 36 años de datos, 2 agencias federales cogestoras y una sola función legal: un detector de señales, no una máquina de causalidad.

5. Reportar no es reclamar. VAERS (vigilancia, abierto a cualquiera) y el VICP (compensación, mediante la Vaccine Injury Table y una petición ante el Court of Federal Claims, con requisitos y plazos: véase el artículo VICP de este repositorio) corren en paralelo y no se convierten el uno en el otro. El orden práctico: atender primero, registrar los cuatro elementos del artículo 300aa-25(a) y reportar a VAERS como exige la ley; valorar la petición VICP por separado. El registro y el informe se convierten en la base fáctica de cualquier procedimiento posterior.

6. California. California no mantiene un sistema estatal paralelo de eventos adversos: los informes van al VAERS federal. El registro propio del estado es otro: las dosis entran en el California Immunization Registry (CAIR), un registro de quién recibió qué dosis, no un registro de eventos adversos. La autoridad de vacunación en farmacias se sitúa en torno al artículo 4052.8 del Business and Professions Code (véase el artículo de vacunación en farmacias de este repositorio), y los deberes federales de registro y reporte del artículo 300aa-25 se aplican encima. Los requisitos de inmunización escolar y de guardería y las exenciones médicas están en el artículo de requisitos de vacunas de este repositorio.

7. Disciplina de lectura. Cuatro reglas: no extraer conclusiones causales de cifras de VAERS sin las advertencias de los CDC (no verificado, no prueba causalidad por sí solo, no da tasas); leer señales, no conteos brutos; mantener separados los tres documentos (RET, VIT, VIS); y volver al registro de origen: lote, fabricante, fecha y administrador, anotados por completo en el momento de la vacunación, son la base sobre la que se apoya todo paso posterior de vigilancia o compensación. Fuentes: vaers.hhs.gov y su tabla de eventos reportables, la documentación VAERS de CDC WONDER, los artículos 300aa-25 y 300aa-26 del título 42, 21 C.F.R. 600.80 y el artículo 1001 del título 18.

## 한국어 (초역 · 初译待校)

### 백신 이상반응 보고 VAERS는 어떻게 관리되는가: 연방 모니터링 체계, 법정 보고 의무, 캘리포니아 연결

주제 확인: 이번 라운드의 법규 후보 세 가지 중 언어 서비스 주제는 이 저장소에 이미 전용 글이 있고, 코페이 누적기 주제는 기존 글로 상당 부분 다뤄져 있어, 본체가 없는 VAERS를 택한다. VAERS는 VICP 보상 글과 약국 예방접종 글에서 한 줄씩 언급될 뿐이었다.

1. 성격. 백신 이상반응 보고 시스템(VAERS)은 1990년부터 운영되어 온 전국 백신 안전 모니터링 체계로, CDC와 FDA가 공동 관리한다. 법적 출신은 1986년 국가 아동 백신 피해법(NCVIA)이며 미국법전 제42편 제300aa-1조 이하에 자리한다. 성격을 세 문장으로 고정한다. VAERS는 결론이 아니라 보고를 모은다. 백신이 어떤 사건을 일으켰는지를 판정하지 않고 이상 신호를 듣는 쪽이다. 보고는 검증되지 않았으며, CDC의 WONDER 설명은 보고서가 불완전하거나 부정확하거나 우연이거나 확인할 수 없을 수 있고, 보고 건수만으로 인과관계를 증명하거나 발생률을 계산할 수 없다고 밝힌다.

2. 누가 보고해야 하는가. 제300aa-25조 (a)항은 접종자가 피접종자의 영구 의무기록에 접종 날짜, 백신 제조사와 로트 번호, 접종을 시행한 사람의 이름과 주소와 직함을 적도록 요구한다. (b)항은 모든 의료 제공자와 모든 백신 제조사에게 세 가지를 보고하도록 요구한다. (A) 백신 피해 표에 실린 사건으로 제300aa-14조 (b)항의 경우를 포함하며 시한은 사건 후 7일 이내 또는 표가 정한 더 긴 기간, (B) 제조사 설명서에 적힌 금기 반응, (C) 규정이 별도로 요구하는 기타 사항이다. 제조사는 추가로 연방규정집 제21편 제600.80조에 따라 알게 된 모든 이상반응을 FDA에 보고한다.

3. 두 개의 표를 혼동하지 말 것. VAERS의 접종 후 보고 대상 사건 표(RET)는 제300aa-25조에 따라 무엇이 보고 대상인지를 밝히며, VAERS 스스로 백신 피해 표(VIT)와 다르다고 말한다. RET의 시간 창은 보고 시한이고, VIT의 시간 창은 VICP 보상의 인과 추정을 받친다. 어떤 사건이 RET에 있다고 해서 VIT에 있는 것도 아니고 백신이 피해를 일으켰다고 인정된 것도 아니다. 세 번째로 이웃한 문서인 제300aa-26조의 백신 정보 설명서(VIS)는 접종 전 안내문이지 이상반응 보고서가 아니다.

4. 누구든 보고할 수 있고, 그 다음은 어떻게 되는가. 제공자, 제조사, 피접종자, 가족, 일반 대중 모두 vaers.hhs.gov에서 보고할 수 있으며, 의료인은 인과관계가 확실하지 않아도 임상적으로 중요하거나 예상 밖의 사건을 보고하도록 권장받는다. 공개 데이터는 1990년부터 현재까지의 초기 보고이다. 이상한 패턴이 모일 때만 더 깊은 분석이 시작되는데, CDC 쪽의 백신 안전 데이터링크(VSD)와 CISA 프로젝트, FDA 쪽의 BEST 시스템이 그 병록 수준의 도구이다. 알면서 거짓으로 VAERS 보고를 제출하면 미국법전 제18편 제1001조(허위 진술)에 닿고, CDC와 FDA는 개별 보고에 대해 개인 의료 조언을 하지 않는다. 계산을 맞춰 보면, 2026 빼기 1990은 36년치 데이터, 공동 관리 연방 기관은 2곳, 법적 기능은 한 문장으로 신호 탐지기이지 인과 판결 기계가 아니다.

5. 보고는 청구가 아니다. VAERS(모니터링, 누구에게나 열림)와 VICP(보상, 백신 피해 표와 연방청구법원의 청원 절차, 자격과 시한의 문턱이 있으며 이 저장소의 VICP 글 참조)는 나란히 달리며 서로 바뀌지 않는다. 실무 순서는 먼저 치료하고, 제300aa-25조 (a)항의 네 요소를 기록하고 법이 요구하는 대로 VAERS에 보고한 뒤, VICP 청원은 따로 평가하는 것이다. 기록과 보고는 이후 모든 절차의 사실 바닥이 된다.

6. 캘리포니아. 캘리포니아에는 VAERS와 나란히 서는 주 차원의 이상반응 보고 체계가 없어 보고는 연방 VAERS 한 곳으로 간다. 주의 자체 장부는 다른 쪽에 있다. 접종 기록은 캘리포니아 예방접종 등록부(CAIR)로 들어가는데, 이는 누가 어떤 접종을 받았는지의 장부이지 이상반응 장부가 아니다. 약국 접종 권한은 사업 및 전문직법 제4052.8조 부근에 자리하며(이 저장소의 약국 예방접종 글 참조), 제300aa-25조의 연방 기록 및 보고 의무가 그 위에 겹쳐 적용된다. 학교와 보육 시설의 예방접종 요건과 의학적 면제는 이 저장소의 백신 요건 글을 따른다.

7. 읽는 규율. 네 가지이다. CDC의 주의를 빼고 VAERS 숫자로 인과 결론을 내리지 말 것(미검증, 단독으로 인과를 증명 못 함, 발생률을 못 냄). 절대 건수가 아니라 신호를 읽을 것. 세 문서를 나눌 것(RET, VIT, VIS). 원천 기록으로 돌아갈 것 — 로트 번호, 제조사, 날짜, 접종자를 접종 당시에 빠짐없이 적는 일이 이후 모든 모니터링과 보상 절차의 바닥이다. 출처는 vaers.hhs.gov와 그 보고 대상 사건 표, CDC WONDER의 VAERS 설명, 미국법전 제42편 제300aa-25조와 제300aa-26조, 연방규정집 제21편 제600.80조, 미국법전 제18편 제1001조이다.

## Tiếng Việt (bản dịch sơ bộ · 初译待校)

### Báo cáo sự cố bất lợi sau tiêm vắc-xin (VAERS) được quản lý thế nào: hệ thống giám sát liên bang, nghĩa vụ báo cáo theo luật và liên hệ California

Kiểm tra chủ đề: trong ba ứng viên pháp quy vòng này, chủ đề dịch vụ ngôn ngữ đã có bài riêng trong kho này và chủ đề bộ tích lũy copay đã được bao phủ phần lớn; VAERS chưa có bài riêng — chỉ xuất hiện như một nhắc nhỏ trong bài bồi thường VICP và bài tiêm chủng tại nhà thuốc — nên được chọn ở đây.

1. Bản chất. Hệ thống Báo cáo Sự cố Bất lợi sau Tiêm Vắc-xin (VAERS) là hệ thống giám sát an toàn vắc-xin toàn quốc, vận hành từ năm 1990 và do CDC cùng FDA đồng quản lý. Gốc luật của nó là Đạo luật Quốc gia về Thương tật do Vắc-xin ở Trẻ em năm 1986, tại Điều 300aa-1 và các điều tiếp theo của Bộ luật Hoa Kỳ tập 42. Ba câu chốt bản chất: VAERS thu thập báo cáo, không phải kết luận; nó lắng nghe tín hiệu bất thường chứ không phán quyết một vắc-xin có gây ra một sự cố hay không; và các báo cáo chưa được xác minh — tài liệu WONDER của CDC nói rõ báo cáo có thể không đầy đủ, không chính xác, trùng hợp hoặc không thể kiểm chứng, và riêng số lượng báo cáo không thể chứng minh quan hệ nhân quả hay tính được tỷ lệ mắc.

2. Ai phải báo cáo. Điều 300aa-25(a) yêu cầu người tiêm ghi vào hồ sơ y tế vĩnh viễn của người được tiêm: ngày tiêm, nhà sản xuất vắc-xin và số lô, cùng tên, địa chỉ và chức danh của người thực hiện tiêm. Khoản (b) yêu cầu mọi nhà cung cấp dịch vụ y tế và mọi nhà sản xuất vắc-xin báo cáo ba nhóm: (A) các sự cố trong Bảng Thương tật do Vắc-xin, gồm cả các trường hợp theo Điều 300aa-14(b), trong vòng 7 ngày hoặc khoảng thời gian dài hơn mà Bảng quy định; (B) các phản ứng chống chỉ định ghi trong tờ hướng dẫn của nhà sản xuất; và (C) các vấn đề khác do quy định yêu cầu. Nhà sản xuất còn phải báo cáo cho FDA mọi sự cố bất lợi mà họ biết được theo 21 C.F.R. 600.80.

3. Hai bảng, không phải một. Bảng các Sự cố Phải Báo cáo sau Tiêm chủng (RET) của VAERS nêu những gì phải báo cáo theo Điều 300aa-25, và chính VAERS lưu ý nó khác với Bảng Thương tật do Vắc-xin (VIT): khung thời gian của RET là cửa sổ báo cáo, còn khung thời gian của VIT phục vụ suy đoán bồi thường trong VICP. Một sự cố nằm trên RET không có nghĩa là nó nằm trên VIT, và không có nghĩa là đã xác định vắc-xin gây hại. Tài liệu thứ ba kề bên, Tờ Thông tin Vắc-xin (VIS) theo Điều 300aa-26, là thông tin trước tiêm, không phải báo cáo.

4. Ai cũng có thể báo cáo, và điều gì xảy ra tiếp theo. Nhà cung cấp, nhà sản xuất, người được tiêm, gia đình và công chúng đều có thể nộp báo cáo tại vaers.hhs.gov, và nhân viên y tế được khuyến khích báo cáo các sự cố quan trọng về lâm sàng hoặc bất ngờ ngay cả khi chưa chắc về quan hệ nhân quả. Dữ liệu công khai bao phủ từ 1990 đến nay và là dữ liệu báo cáo ban đầu. Chỉ khi xuất hiện một mẫu hình bất thường mới kích hoạt phân tích sâu hơn — Vaccine Safety Datalink (VSD) và Dự án CISA của CDC, cùng hệ thống BEST của FDA — những công cụ ở cấp hồ sơ bệnh án mới đẩy một nghi ngờ tiến về phía đánh giá nhân quả. Cố ý nộp báo cáo VAERS sai sự thật vi phạm 18 U.S.C. 1001, và CDC/FDA không đưa ra lời khuyên y tế cá nhân về một báo cáo. Phép tính: 2026 trừ 1990 bằng 36 năm dữ liệu, 2 cơ quan liên bang đồng quản lý, và một chức năng theo luật duy nhất — một máy dò tín hiệu, không phải một máy phán quyết nhân quả.

5. Báo cáo không phải là đòi bồi thường. VAERS (giám sát, mở cho mọi người) và VICP (bồi thường, qua Bảng Thương tật do Vắc-xin và đơn thỉnh cầu tại Tòa Thỉnh cầu Liên bang, có điều kiện và thời hạn — xem bài VICP của kho này) chạy song song và không chuyển đổi qua lại. Thứ tự thực hành: điều trị trước, ghi đủ bốn yếu tố của Điều 300aa-25(a) và báo cáo VAERS theo luật yêu cầu; đánh giá đơn VICP riêng. Hồ sơ và báo cáo trở thành nền tảng thực tế của mọi thủ tục về sau.

6. California. California không vận hành hệ thống báo cáo sự cố bất lợi cấp bang song song: báo cáo đi về VAERS liên bang. Sổ sách riêng của bang nằm ở phía khác — các liều tiêm đi vào Hệ thống Đăng ký Tiêm chủng California (CAIR), tức sổ ghi ai đã nhận liều nào, chứ không phải sổ sự cố bất lợi. Thẩm quyền tiêm chủng tại nhà thuốc nằm quanh Điều 4052.8 của Bộ luật Kinh doanh và Nghề nghiệp (xem bài tiêm chủng tại nhà thuốc của kho này), và nghĩa vụ ghi chép, báo cáo liên bang của Điều 300aa-25 áp dụng chồng lên trên. Yêu cầu tiêm chủng của trường học và nhà trẻ cùng miễn trừ y tế nằm ở bài yêu cầu vắc-xin của kho này.

7. Kỷ luật đọc dữ liệu. Bốn quy tắc: không rút kết luận nhân quả từ con số VAERS khi bỏ qua các lưu ý của CDC (chưa xác minh, không tự nó chứng minh nhân quả, không tính được tỷ lệ); đọc tín hiệu chứ không đọc con số tuyệt đối; tách bạch ba tài liệu (RET, VIT, VIS); và quay về hồ sơ gốc — số lô, nhà sản xuất, ngày và người tiêm, được ghi đầy đủ ngay tại buổi tiêm, là nền mà mọi bước giám sát hay bồi thường sau đó đứng lên. Nguồn: vaers.hhs.gov và Bảng các Sự cố Phải Báo cáo sau Tiêm chủng của nó, tài liệu VAERS của CDC WONDER, Điều 300aa-25 và 300aa-26 của Bộ luật Hoa Kỳ tập 42, 21 C.F.R. 600.80 và 18 U.S.C. 1001.

## हिन्दी (प्रारंभिक अनुवाद · 初译待校)

### टीका प्रतिकूल घटना रिपोर्टिंग (VAERS) कैसे शासित है: संघीय निगरानी प्रणाली, वैधानिक रिपोर्टिंग कर्तव्य और कैलिफ़ोर्निया संबंध

विषय-जाँच: इस चक्र के तीन नियामक उम्मीदवारों में से भाषा-सेवा विषय पर इस भंडार में पहले से एक अलग लेख है और copay accumulator विषय काफी हद तक कवर है; VAERS का अपना कोई लेख नहीं है — वह केवल VICP मुआवज़ा लेख और फ़ार्मेसी टीकाकरण लेख में एक-एक पंक्ति में आता है — इसलिए यहाँ उसे लिया गया है।

1. स्वरूप। Vaccine Adverse Event Reporting System (VAERS) राष्ट्रीय टीका-सुरक्षा निगरानी प्रणाली है, 1990 से चल रही है और CDC व FDA द्वारा संयुक्त रूप से प्रबंधित है। इसका वैधानिक घर 1986 का National Childhood Vaccine Injury Act है, U.S. Code के खंड 42 की धारा 300aa-1 व आगे। तीन वाक्य इसका चरित्र तय करते हैं: VAERS रिपोर्टें इकट्ठा करता है, निष्कर्ष नहीं; वह यह तय नहीं करता कि किसी टीके ने कोई घटना घटाई, वह असामान्य संकेत सुनता है; और इसकी रिपोर्टें असत्यापित होती हैं — CDC के WONDER प्रलेखन में कहा गया है कि रिपोर्टें अपूर्ण, अशुद्ध, संयोगात्मक या असत्यापनीय हो सकती हैं, और केवल रिपोर्ट-संख्या से कार्य-कारण सिद्ध नहीं होता और घटना-दर नहीं निकलती।

2. किसे रिपोर्ट करना है। धारा 300aa-25(a) चाहती है कि टीका लगाने वाला प्राप्तकर्ता के स्थायी चिकित्सा अभिलेख में टीकाकरण की तिथि, टीके का निर्माता व लॉट नंबर, और लगाने वाले व्यक्ति का नाम, पता व पद दर्ज करे। धारा 300aa-25(b) प्रत्येक स्वास्थ्य प्रदाता और प्रत्येक टीका निर्माता से तीन बातों की रिपोर्ट चाहती है: (A) Vaccine Injury Table के घटना-प्रकार, धारा 300aa-14(b) के प्रकारों समेत, घटना के 7 दिनों के भीतर या Table द्वारा निर्दिष्ट लंबी अवधि में; (B) निर्माता के package insert में बताए गए contraindicating प्रतिक्रियाएँ; और (C) नियमन द्वारा अपेक्षित अन्य मामले। निर्माता इसके अतिरिक्त 21 C.F.R. 600.80 के तहत अपने ज्ञान में आई सभी प्रतिकूल घटनाएँ FDA को रिपोर्ट करते हैं।

3. दो तालिकाएँ, एक नहीं। VAERS की Table of Reportable Events Following Vaccination (RET) बताती है कि धारा 300aa-25 के तहत क्या रिपोर्ट करना आवश्यक है, और VAERS स्वयं नोट करता है कि यह Vaccine Injury Table (VIT) से भिन्न है: RET के समय-खंड रिपोर्टिंग खिड़कियाँ हैं, VIT के खंड VICP में मुआवज़े के अनुमान के काम आते हैं। किसी घटना का RET पर होना उसे VIT पर नहीं रखता और यह स्थापित नहीं करता कि टीके ने नुक़सान किया। तीसरा पड़ोसी दस्तावेज़, धारा 300aa-26 के तहत Vaccine Information Statement (VIS), टीकाकरण से पहले की जानकारी है, रिपोर्ट नहीं।

4. कोई भी रिपोर्ट कर सकता है, और आगे क्या होता है। प्रदाता, निर्माता, प्राप्तकर्ता, परिवार और जनता सभी vaers.hhs.gov पर रिपोर्ट दाख़िल कर सकते हैं, और स्वास्थ्य पेशेवरों को प्रोत्साहित किया जाता है कि वे नैदानिक रूप से महत्वपूर्ण या अप्रत्याशित घटनाएँ रिपोर्ट करें, भले ही कार्य-कारण पर अनिश्चित हों। सार्वजनिक डेटा 1990 से वर्तमान तक का है और प्रारंभिक रिपोर्टों का है। केवल असामान्य पैटर्न ही गहरे विश्लेषण को ट्रिगर करता है — CDC का Vaccine Safety Datalink (VSD) और CISA Project, और FDA का BEST system — जो अभिलेख-स्तर के उपकरण हैं जो किसी संदेह को कार्य-कारण मूल्यांकन की ओर ले जाते हैं। जानबूझकर झूठी VAERS रिपोर्ट दाख़िल करना 18 U.S.C. धारा 1001 का उल्लंघन है, और CDC/FDA किसी रिपोर्ट पर व्यक्तिगत चिकित्सा परामर्श नहीं देते। हिसाब: 2026 घटा 1990 बराबर 36 वर्षों का डेटा, 2 संयुक्त-प्रबंधक संघीय एजेंसियाँ, और एक वैधानिक काम — एक संकेत-संसूचक, कार्य-कारण मशीन नहीं।

5. रिपोर्ट करना दावा करना नहीं है। VAERS (निगरानी, सबके लिए खुला) और VICP (मुआवज़ा, Vaccine Injury Table व Court of Federal Claims में याचिका के माध्यम से, पात्रता और समय-सीमा के द्वार समेत — इस भंडार का VICP लेख देखें) समानांतर चलते हैं और आपस में नहीं बदलते। व्यवहारिक क्रम: पहले उपचार, फिर धारा 300aa-25(a) के चार तत्व दर्ज करें और कानून के अनुसार VAERS रिपोर्ट करें; VICP याचिका का मूल्यांकन अलग से करें। अभिलेख और रिपोर्ट किसी भी बाद की कार्यवाही का तथ्यात्मक आधार बन जाते हैं।

6. कैलिफ़ोर्निया। कैलिफ़ोर्निया कोई समानांतर राज्य प्रतिकूल-घटना प्रणाली नहीं चलाता: रिपोर्टें संघीय VAERS को जाती हैं। राज्य की अपनी बही दूसरी ओर है — खुराकें California Immunization Registry (CAIR) में जाती हैं, जो इसका अभिलेख है कि किसने कौन-सी खुराक ली, प्रतिकूल घटनाओं की बही नहीं। फ़ार्मेसी टीकाकरण अधिकार Business and Professions Code की धारा 4052.8 के आसपास स्थित है (इस भंडार का फ़ार्मेसी टीकाकरण लेख देखें), और धारा 300aa-25 के संघीय अभिलेख व रिपोर्टिंग कर्तव्य उसके ऊपर लागू होते हैं। स्कूल व शिशु-देखभाल टीकाकरण आवश्यकताएँ और चिकित्सा छूट इस भंडार के टीका-आवश्यकता लेख में हैं।

7. पढ़ने का अनुशासन। चार नियम: CDC की चेतावनियों के बिना VAERS संख्याओं से कार्य-कारण निष्कर्ष न निकालें (असत्यापित, अकेले कार्य-कारण सिद्ध नहीं करता, दर नहीं देता); निरपेक्ष गिनती नहीं, संकेत पढ़ें; तीनों दस्तावेज़ अलग रखें (RET, VIT, VIS); और मूल अभिलेख पर लौटें — लॉट नंबर, निर्माता, तिथि और लगाने वाला, टीकाकरण के समय पूरी तरह दर्ज, वह आधार है जिस पर निगरानी या मुआवज़े का हर बाद का कदम खड़ा होता है। स्रोत: vaers.hhs.gov और उसकी Table of Reportable Events Following Vaccination, CDC WONDER का VAERS प्रलेखन, 42 U.S.C. धारा 300aa-25 व 300aa-26, 21 C.F.R. 600.80, और 18 U.S.C. धारा 1001।

---

*个人学习笔记，不构成医疗建议。本文为疫苗安全监测制度学习笔记；报告义务与表格口径以 HHS 的 VAERS 官网与《美国法典》现行原文为准，数据使用口径以 CDC 公开说明为准。后四语（西／韩／越／印）为初译待校。*
