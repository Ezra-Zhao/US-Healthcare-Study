# 电子处方与管制药电子处方怎么管：DEA 的 EPCS 与加州第 11168 条及例外

> 个人学习笔记，不构成法律建议，也不构成医疗建议。本篇讲处方从纸面搬到电子系统之后，普通电子处方与管制药电子处方分别受哪套规则管、加州的强制电子传输线又怎么落地；全篇只写制度框架，不写任何药物剂量与频次。联邦与州的执行口径会调整，办理与执业前务必回 DEA、CMS 与加州当期官方口径复核一次。

## 中文主文

### 一、先分两层：普通电子处方的地基，与管制药电子处方的加严线

电子处方（e-prescribing）不是一套规则管到底，要先分两层。第一层是普通处方的电子传输：处方者开方、电子系统把处方传到药房、药师核验调配，这条线的法律地基主要在州药房法——各州承认以电子方式生成与传输的处方与纸质处方具有同等效力，并对传输的真实性、完整性与保密性提出要求。往上一层还有电子签名的一般法律背景：联邦《电子签名法》（ESIGN）与各州普遍采用的《统一电子交易法》（UETA）确立了电子记录与电子签名不因其电子形式而被否认效力的原则，一句带过即可，日常执业真正要对的还是药房法与处方规则本身。

第二层是管制药的电子处方，英文缩写 EPCS（Electronic Prescriptions for Controlled Substances）。管制药一旦允许用电子方式开，风险点就变了：纸质处方的防伪靠纸张与笔迹，电子处方的防伪全靠身份与系统——谁在签名、签名密钥在谁手里、软件有没有被动手脚，都必须有硬规则。所以联邦给 EPCS 单独加了一整套严于普通电子处方的要求，主管机关是缉毒局（Drug Enforcement Administration，DEA）。本篇的主线就是这第二层，外加联邦的推动线与加州的强制线；与仓内两篇的分工先说清：《远程医疗开管制药怎么管》管的是远程场景下谁有资格开管制药（Ryan Haight 法一线），《受控物质怎么管》管的是管制药的分级、DEA 登记与加州 CURES 的总框架，本篇只管「电子这张处方怎么签、怎么传才算数」这一段，不重复前两篇。

### 二、联邦 EPCS 的硬规则：21 CFR Part 1311 的四根柱子

DEA 的 EPCS 规则写在《联邦法规》第 21 篇第 1311 部分（21 CFR Part 1311），骨架可以记成四根柱子。

第一根是处方者身份核验。处方者启用电子签名资格之前，身份须先经过核验——不是自己在系统里点一下同意就算数，而是要通过规则认可的身份证明流程，确认屏幕后面的人就是执照上的那个人。

第二根是双因素认证。签署管制药电子处方时，处方者须使用双因素认证：从知识因素（只有本人知道的口令一类）、持有因素（本人持有的令牌、密钥载体一类）、生物特征因素（指纹等生物识别一类）三类里同时用上两类。三类取两类，这是这套规则最常被考、也最常在系统配置上出错的一条——只输一个口令就签掉管制药处方，不符合 EPCS 的签名口径。

第三根是应用软件须经认证审计。处方者与药房使用的电子处方应用，须通过规则要求的第三方审计或认证，确认软件在身份管理、签名、记录保存与安全控制上达到 Part 1311 的标准。换句话说，合规不只是医生个人的事，诊所采购与配置的系统本身先要过这一关；换系统、换供应商时，这一项要重新核对，不能默认新系统自动合规。

第四根是签名密钥的个人控制。处方者的签名凭据只归处方者本人控制，不得共享、不得交他人代签。助理帮着把处方内容录入系统是一回事，最后的签署动作与凭据使用必须是处方者本人——凭据借人、口令共享，在 EPCS 框架下是直接踩线的行为，出问题时责任也回到处方者本人头上。

药房一侧同样有对应义务：接收 EPCS 的药房系统也要满足 Part 1311 对应用与记录的要求，电子处方记录按规则保存、备查。整条链的设计思路一以贯之：每一张管制药电子处方，都要能回溯到一个经过身份核验的人、一次双因素签署动作和一套经过审计的软件。

### 三、联邦推动线：SUPPORT 法第 2003 节与 Medicare Part D

规则允许之外，联邦还用支付线推着走。《SUPPORT 法》（SUPPORT for Patients and Communities Act）第 2003 节要求：在 Medicare Part D 之下，管制药处方原则上走电子处方，即按 EPCS 的方式开具。执行落在医疗保险与医疗补助服务中心（CMS）一侧，CMS 自 2023 年起按其合规口径推进执行，对不符合要求的情形有相应的合规处置与例外、豁免安排——具体哪些情形算例外、处置怎么走，以 CMS 当期公布的口径为准，本文不写死。读这条线要抓住两点：第一，它是借 Part D 支付场景推 EPCS 落地，不是另创一套签名标准，签名与系统的技术标准仍回 Part 1311；第二，它只覆盖 Part D 这一场景，管制药电子处方的州法要求另行并行适用，联邦支付线合规不等于州线自动合规。

### 四、加州线：《健康与安全法典》第 11168 条的强制电子传输与法定例外

加州的线比联邦支付线更宽：不是只管 Part D，而是管加州处方本身。依据是《健康与安全法典》（Health and Safety Code）第 11168 条，由 AB 2789 制定，自 2022 年 1 月 1 日起生效。主规则一句话：加州的处方原则上须以电子方式生成与传输，也就是处方者开方默认走电子传输，不再把纸质处方当常态。

例外按条文结构克制地记，遇到具体情形回条文原文与当期指引核对，不自行扩缩。大类包括：技术或电力故障等导致电子传输客观上做不到的情形；在加州以外调配等跨州情形；兽医处方等条文点名的场景；以及条文列举的其他法定例外。例外的共同点是「电子做不到或不适用」，不是「处方者觉得纸质更方便」——便利不是例外理由，这是读第 11168 条时最要紧的一条分界。

责任落点也要记准两条。第一，药房一侧：药房收到纸质或口头处方，并不因此违法——第 11168 条的强制义务压在处方者一侧，药房照常按药房法核验与调配，不因处方的传输形式替处方者背锅。第二，处方者一侧：无例外理由而不走电子传输的，问题落在处方者这边，按当期口径可能面临向其执照委员会的转介等处置，细目以条文与委员会当期口径为准。还有一条实务衔接：管制药在加州走电子传输，还要同时满足联邦 EPCS 的 Part 1311 要求与加州受控物质框架下的 CURES 等义务，三套线是叠加关系，不是三选一，具体分工看仓内《受控物质怎么管》一篇。

### 五、要点清单

- 分层：普通电子处方看州药房法（ESIGN 与 UETA 只是电子签名的一般背景）；管制药电子处方另加 DEA 的 EPCS 加严线。
- EPCS 四根柱子（21 CFR Part 1311）：处方者身份核验、双因素认证（三类因素取两类）、应用软件经认证审计、签名密钥处方者个人控制不得共享。
- 推动线：SUPPORT 法第 2003 节要求 Part D 下管制药走电子处方，CMS 自 2023 年起按当期合规口径执行，技术标准仍回 Part 1311。
- 加州线：《健康与安全法典》第 11168 条（AB 2789，2022 年 1 月 1 日生效）——处方原则上须电子传输，例外限技术或电力故障、跨州调配、兽医等法定情形，便利不是例外。
- 责任：药房收到纸质或口头处方不因此违法，处罚与转介的落点在处方者一侧；远程开药资格看 Ryan Haight 专篇，管制药总框架看受控物质专篇，本篇只管电子签署与传输这一段。

*声明：个人学习笔记，不构成法律建议，也不构成医疗建议。来源：缉毒局（DEA）管制药电子处方规则（21 CFR Part 1311）；《SUPPORT 法》第 2003 节与医疗保险与医疗补助服务中心（CMS）Part D 电子处方合规公开口径；加州《健康与安全法典》第 11168 条（AB 2789，2022 年 1 月 1 日生效）；联邦《电子签名法》（ESIGN）与《统一电子交易法》（UETA）一般背景。执行与例外细目以当期官方口径为准。本篇全篇不涉及药物剂量与频次。个人学习笔记，不构成法律/税务/医疗建议。*

---

## English

### 1. Two layers: the foundation for ordinary electronic prescribing, and the stricter line for controlled substances

Electronic prescribing is not one rulebook. The first layer is ordinary electronic transmission: a prescriber issues a prescription, a system transmits it to a pharmacy, and the pharmacy verifies and dispenses. Its legal foundation sits mainly in state pharmacy law, which treats electronically created and transmitted prescriptions as equivalent to paper ones, subject to authenticity, integrity and confidentiality requirements. Behind it stand the general electronic-signature frameworks — the federal ESIGN Act and the state Uniform Electronic Transactions Act (UETA) — which establish that an electronic record or signature is not to be denied effect solely because it is electronic. The second layer is electronic prescribing of controlled substances, EPCS. Once controlled substances may be signed electronically, the anti-forgery burden shifts from paper and handwriting to identity and systems, so the federal government added a rule set stricter than ordinary e-prescribing, administered by the Drug Enforcement Administration (DEA). This article follows that second layer, plus the federal payment push and California's mandate. It complements, and does not repeat, this repository's articles on telehealth prescribing of controlled substances (the Ryan Haight qualification line) and on controlled substances generally (schedules, DEA registration and California's CURES).

### 2. The federal EPCS rules: the four pillars of 21 CFR Part 1311

The DEA's EPCS rules are at 21 CFR Part 1311, and their frame is four pillars. First, identity proofing: before a prescriber may sign electronically, the prescriber's identity must be verified through the process the rule recognizes — the person behind the screen must be shown to be the licensed prescriber. Second, two-factor authentication: signing a controlled-substance prescription requires two of the three factor classes — something known (a password-type factor), something held (a token or key-carrier factor) and a biometric factor. Three classes, any two — a single password alone does not meet the EPCS signing standard. Third, certified and audited applications: the electronic prescribing applications used by prescribers and pharmacies must pass the third-party audit or certification the rule requires, covering identity management, signing, recordkeeping and security controls; changing systems means re-checking this pillar, not assuming compliance carries over. Fourth, personal control of signing credentials: a prescriber's signing credential is under that prescriber's sole control and may not be shared or handed to another person to sign with. Staff may help enter prescription content, but the signing act and the credential are the prescriber's own. Pharmacy-side systems carry matching Part 1311 duties for applications and records, so every controlled-substance e-prescription can be traced back to a proofed person, a two-factor signing act and an audited application.

### 3. The federal push: SUPPORT Act section 2003 and Medicare Part D

Beyond permission, federal law also pushes through payment. Section 2003 of the SUPPORT for Patients and Communities Act requires controlled-substance prescriptions under Medicare Part D to be transmitted electronically, in the EPCS manner. Enforcement sits with the Centers for Medicare & Medicaid Services (CMS), which has moved compliance forward since 2023 under its published compliance framework, with exceptions and enforcement arrangements as CMS currently publishes them — details follow CMS's current guidance. Two points to hold: this is a Part D payment-side push, not a new signing standard — the technical standard remains Part 1311 — and it covers the Part D setting only, alongside, not instead of, state-law requirements.

### 4. California: Health and Safety Code section 11168, the electronic-transmission mandate and its exceptions

California's line is broader than the federal payment line because it governs California prescriptions themselves. Health and Safety Code section 11168, enacted by AB 2789 and effective January 1, 2022, states the default: prescriptions in California are to be generated and transmitted electronically; paper is no longer the norm. Exceptions are read from the statute's own structure and are not to be stretched or shrunk by feel; in broad categories they include situations where electronic transmission is objectively impossible, such as technical or electrical failure; dispensing outside California and other cross-state situations; veterinary prescriptions and other scenarios the statute names; and the statute's remaining listed exceptions. Their common thread is impossibility or inapplicability, not convenience — a prescriber's preference for paper is not an exception. On responsibility, two points. The pharmacy side: a pharmacy that receives a paper or oral prescription does not thereby violate section 11168; the mandate rests on the prescriber. The prescriber side: transmitting other than electronically without an exception is the prescriber's problem, which under the current framework can lead to referral to the prescriber's licensing board, among other consequences, as the statute and board guidance currently state. For controlled substances in California, the federal Part 1311 requirements and the CURES framework stack on top of section 11168; the lines are cumulative, not alternatives.

### 5. Key points

- Layers: ordinary e-prescribing rests on state pharmacy law (ESIGN and UETA are only the general electronic-signature background); controlled substances add the DEA's stricter EPCS line.
- The four EPCS pillars (21 CFR Part 1311): identity proofing, two-factor authentication (any two of three factor classes), audited or certified applications, and personal, non-shared control of signing credentials.
- The push: SUPPORT Act section 2003 requires Part D controlled-substance prescriptions to go electronically; CMS has enforced since 2023 under its current compliance framework, and the technical standard remains Part 1311.
- California: Health and Safety Code section 11168 (AB 2789, effective January 1, 2022) makes electronic transmission the default, with exceptions limited to statutory situations such as technical or electrical failure, out-of-state dispensing and veterinary prescriptions — convenience is not an exception.
- Responsibility: a pharmacy receiving a paper or oral prescription does not thereby break the law; consequences land on the prescriber side.

*Note: Personal study notes only; not legal advice and not medical advice. Sources: Drug Enforcement Administration (DEA), Electronic Prescriptions for Controlled Substances, 21 CFR Part 1311; SUPPORT for Patients and Communities Act, section 2003, and Centers for Medicare & Medicaid Services (CMS) Part D electronic-prescribing compliance guidance; California Health and Safety Code section 11168 (AB 2789, eff. January 1, 2022); ESIGN Act and Uniform Electronic Transactions Act (UETA) as general background. Enforcement details and exceptions follow the official guidance in force. This article contains no medication details.*

---

## Español (译稿)

### 1. Dos capas: la base de la receta electrónica común y la línea reforzada para sustancias controladas

La receta electrónica no es un solo reglamento. La primera capa es la transmisión electrónica ordinaria: el prescriptor emite la receta, un sistema la transmite a la farmacia y la farmacia la verifica y dispensa. Su fundamento jurídico está sobre todo en la ley estatal de farmacia, que equipara las recetas creadas y transmitidas electrónicamente a las de papel, con requisitos de autenticidad, integridad y confidencialidad. Detrás están los marcos generales de firma electrónica —la ley federal ESIGN y la Uniform Electronic Transactions Act (UETA) de los estados—, que establecen que un registro o firma electrónicos no pierden efecto por ser electrónicos. La segunda capa es la receta electrónica de sustancias controladas, EPCS. Cuando las sustancias controladas pueden firmarse electrónicamente, la carga antifalsificación pasa del papel y la caligrafía a la identidad y los sistemas, por lo que el gobierno federal añadió un conjunto de reglas más estricto que el de la receta electrónica común, administrado por la Drug Enforcement Administration (DEA). Este artículo sigue esa segunda capa, más el impulso federal de pago y el mandato de California. Complementa, sin repetir, los artículos de este repositorio sobre prescripción de sustancias controladas por telemedicina (la línea de calificación de la ley Ryan Haight) y sobre sustancias controladas en general (clasificación, registro ante la DEA y el sistema CURES de California).

### 2. Las reglas federales del EPCS: los cuatro pilares del 21 CFR Part 1311

Las reglas EPCS de la DEA están en el 21 CFR Part 1311 y su estructura son cuatro pilares. Primero, verificación de identidad: antes de poder firmar electrónicamente, la identidad del prescriptor debe verificarse por el proceso que la regla reconoce; debe demostrarse que la persona tras la pantalla es el prescriptor con licencia. Segundo, autenticación de dos factores: firmar una receta de sustancia controlada exige dos de las tres clases de factores —algo que se sabe (tipo contraseña), algo que se posee (tipo token o soporte de clave) y un factor biométrico—; dos de tres, y una sola contraseña no cumple el estándar de firma del EPCS. Tercero, aplicaciones certificadas y auditadas: las aplicaciones de receta electrónica de prescriptores y farmacias deben superar la auditoría o certificación de terceros que exige la regla, en gestión de identidad, firma, registros y controles de seguridad; cambiar de sistema obliga a reverificar este pilar. Cuarto, control personal de las credenciales de firma: la credencial de firma es de control exclusivo del prescriptor y no puede compartirse ni entregarse a otra persona para que firme. El personal puede ayudar a cargar el contenido, pero el acto de firmar y la credencial son del prescriptor. Los sistemas de farmacia tienen deberes paralelos del Part 1311 sobre aplicaciones y registros, de modo que cada receta electrónica de sustancia controlada pueda rastrearse hasta una persona verificada, un acto de firma de dos factores y una aplicación auditada.

### 3. El impulso federal: la sección 2003 de la ley SUPPORT y Medicare Parte D

Además de permitir, la ley federal también impulsa por la vía del pago. La sección 2003 de la SUPPORT for Patients and Communities Act exige que las recetas de sustancias controladas bajo Medicare Parte D se transmitan electrónicamente, al modo EPCS. La aplicación corresponde a los Centers for Medicare & Medicaid Services (CMS), que desde 2023 avanzan el cumplimiento según su marco publicado, con excepciones y arreglos según la orientación vigente de CMS. Dos ideas a retener: es un impulso por el pago de la Parte D, no un nuevo estándar de firma —el estándar técnico sigue siendo el Part 1311— y cubre solo el escenario de la Parte D, en paralelo a los requisitos estatales, no en su lugar.

### 4. California: la sección 11168 del Health and Safety Code, el mandato de transmisión electrónica y sus excepciones

La línea de California es más amplia que la federal de pago porque regula las recetas californianas mismas. La sección 11168 del Health and Safety Code, creada por la AB 2789 y vigente desde el 1 de enero de 2022, fija la regla por defecto: las recetas en California deben generarse y transmitirse electrónicamente; el papel ya no es la norma. Las excepciones se leen de la estructura misma del estatuto y no deben estirarse ni recortarse por impresión; en categorías amplias incluyen situaciones en que la transmisión electrónica es objetivamente imposible, como fallos técnicos o eléctricos; la dispensación fuera de California y otras situaciones interestatales; las recetas veterinarias y demás escenarios que el estatuto nombra; y las restantes excepciones enumeradas. Su hilo común es la imposibilidad o la inaplicabilidad, no la comodidad: preferir el papel no es una excepción. En responsabilidad, dos puntos. Del lado de la farmacia: recibir una receta en papel u oral no infringe por sí solo la sección 11168; el mandato recae sobre el prescriptor. Del lado del prescriptor: transmitir sin vía electrónica y sin excepción es su problema, que en el marco vigente puede llevar, entre otras consecuencias, a la remisión a su consejo de licencias, según el estatuto y la orientación vigente. Para sustancias controladas en California, los requisitos federales del Part 1311 y el marco CURES se suman a la sección 11168: las líneas se acumulan, no se eligen.

### 5. Puntos clave

- Capas: la receta electrónica común descansa en la ley estatal de farmacia (ESIGN y UETA son solo el fondo general de firma electrónica); las sustancias controladas añaden la línea reforzada EPCS de la DEA.
- Los cuatro pilares del EPCS (21 CFR Part 1311): verificación de identidad, autenticación de dos factores (dos de tres clases), aplicaciones auditadas o certificadas y control personal e intransferible de las credenciales de firma.
- El impulso: la sección 2003 de la ley SUPPORT exige la vía electrónica para sustancias controladas en la Parte D; CMS aplica desde 2023 según su marco vigente, y el estándar técnico sigue siendo el Part 1311.
- California: la sección 11168 del Health and Safety Code (AB 2789, desde el 1 de enero de 2022) hace de la transmisión electrónica la regla, con excepciones limitadas a supuestos legales como fallo técnico o eléctrico, dispensación fuera del estado y recetas veterinarias; la comodidad no es excepción.
- Responsabilidad: la farmacia que recibe una receta en papel u oral no infringe por ello la ley; las consecuencias caen del lado del prescriptor.

*Nota: apuntes personales de estudio; no es asesoría legal ni médica. Fuentes: Drug Enforcement Administration (DEA), Electronic Prescriptions for Controlled Substances, 21 CFR Part 1311; SUPPORT for Patients and Communities Act, sección 2003, y orientación de cumplimiento de receta electrónica de la Parte D de los Centers for Medicare & Medicaid Services (CMS); California Health and Safety Code § 11168 (AB 2789, vigente desde el 1 de enero de 2022); ley ESIGN y Uniform Electronic Transactions Act (UETA) como fondo general. Los detalles de aplicación y las excepciones siguen la orientación oficial vigente. Este artículo no contiene detalles de medicamentos. (Traducción de estudio.)*

---

## 한국어 (초역 · 初译待校)

### 1. 두 층위: 일반 전자처방의 토대와 규제약물 전자처방의 가엄선

전자처방은 하나의 규칙으로 끝나지 않습니다. 첫 번째 층은 일반 전자 전송입니다. 처방자가 처방을 내고, 시스템이 약국으로 전송하며, 약국이 확인하고 조제합니다. 법적 토대는 주로 주 약사법에 있으며, 전자적으로 생성·전송된 처방을 종이 처방과 동등하게 취급하되 진정성, 완전성, 비밀유지에 대한 요건을 둡니다. 그 뒤에는 전자서명의 일반 틀인 연방 ESIGN법과 각 주의 UETA(Uniform Electronic Transactions Act)가 있어, 전자 기록과 전자서명이 전자적이라는 이유만으로 효력을 부정당하지 않는다는 원칙을 세웁니다. 두 번째 층이 규제약물 전자처방, EPCS입니다. 규제약물을 전자 방식으로 서명할 수 있게 되면 위조 방지의 부담이 종이와 필체에서 신원과 시스템으로 옮겨 가므로, 연방은 일반 전자처방보다 엄한 규칙을 따로 두었고 주관 기관은 Drug Enforcement Administration(DEA)입니다. 이 글은 이 두 번째 층과 연방의 지급 추진선, 캘리포니아의 강제선을 다룹니다. 원격진료로 규제약물을 여는 자격을 다룬 Ryan Haight 글, 분류와 DEA 등록 및 캘리포니아 CURES의 총틀을 다룬 규제물질 글과는 분업하며 반복하지 않습니다.

### 2. 연방 EPCS의 핵심 규칙: 21 CFR Part 1311의 네 기둥

DEA의 EPCS 규칙은 21 CFR Part 1311에 있으며 뼈대는 네 기둥입니다. 첫째, 처방자 신원 확인입니다. 전자서명 자격을 쓰기 전에 규칙이 인정하는 절차로 신원을 확인해야 합니다. 둘째, 이중 요소 인증입니다. 규제약물 전자처방에 서명할 때는 지식 요소(비밀번호류), 소지 요소(토큰·키 매체류), 생체 요소(지문 등) 세 종류 중 두 종류를 함께 써야 합니다. 세 종류 중 둘 — 비밀번호 하나만으로는 EPCS 서명 기준에 닿지 않습니다. 셋째, 응용 소프트웨어의 인증 감사입니다. 처방자와 약국이 쓰는 전자처방 응용은 신원 관리, 서명, 기록 보존, 보안 통제에 대해 규칙이 요구하는 제3자 감사나 인증을 통과해야 하며, 시스템을 바꾸면 이 항목을 다시 확인해야 합니다. 넷째, 서명 자격증명의 개인 통제입니다. 서명 자격증명은 처방자 본인만 통제하고 공유하거나 남에게 대신 서명하게 해서는 안 됩니다. 직원이 처방 내용을 입력하는 것과 마지막 서명 행위는 다른 일입니다. 약국 측 시스템에도 Part 1311의 응용·기록 의무가 대응해 걸려 있어, 규제약물 전자처방 한 장 한 장이 신원이 확인된 사람, 이중 요소 서명 행위, 감사받은 소프트웨어로 되짚어질 수 있게 설계되어 있습니다.

### 3. 연방 추진선: SUPPORT법 2003절과 Medicare Part D

허용을 넘어 연방은 지급선으로도 밀어붙입니다. SUPPORT for Patients and Communities Act 2003절은 Medicare Part D 아래에서 규제약물 처방이 원칙적으로 전자 방식으로, 즉 EPCS 방식으로 나가도록 요구합니다. 집행은 Centers for Medicare & Medicaid Services(CMS) 쪽에 있으며, CMS는 2023년부터 현행 준수 틀에 따라 집행을 진전시켜 왔고, 예외와 집행의 세부 내용은 CMS 현행 공표 기준을 따릅니다. 두 가지를 잡아 두십시오. 이것은 Part D 지급 장면을 통한 추진이지 새로운 서명 표준이 아니어서 기술 표준은 여전히 Part 1311로 돌아가며, Part D 장면만 덮을 뿐 주법 요구와 병행합니다.

### 4. 캘리포니아선: Health and Safety Code 11168조의 강제 전자 전송과 법정 예외

캘리포니아선은 연방 지급선보다 넓어서 캘리포니아 처방 자체를 규율합니다. 근거는 AB 2789로 제정되어 2022년 1월 1일부터 시행된 Health and Safety Code 11168조입니다. 기본 규칙은 처방이 원칙적으로 전자 방식으로 생성·전송되어야 한다는 것입니다. 예외는 조문 구조대로 절제해서 읽으며 임의로 넓히거나 좁히지 않습니다. 큰 갈래로는 기술·전력 고장처럼 전자 전송이 객관적으로 불가능한 경우, 캘리포니아 밖 조제 등 주 경계를 넘는 경우, 수의 처방 등 조문이 지목한 장면, 그리고 조문이 열거한 그 밖의 법정 예외가 있습니다. 예외의 공통점은 전자 방식이 불가능하거나 맞지 않는 경우이지, 종이가 편하다는 이유가 아닙니다. 책임 소재도 두 가지로 기억합니다. 약국 측은 종이 또는 구두 처방을 받았다는 것만으로 위법이 되지 않습니다. 강제 의무는 처방자 쪽에 있습니다. 처방자 측은 예외 사유 없이 전자 전송을 하지 않으면 문제가 처방자에게 돌아가며, 현행 틀에서는 면허 위원회로의 회부 등 처리가 따를 수 있어 세부 내용은 조문과 위원회 현행 기준을 따릅니다. 캘리포니아에서 규제약물은 11168조 위에 연방 Part 1311 요건과 CURES 틀이 겹쳐 적용됩니다. 세 선은 택일이 아니라 누적입니다.

### 5. 요점 정리

- 층위: 일반 전자처방은 주 약사법이 토대(ESIGN과 UETA는 전자서명의 일반 배경일 뿐)이고, 규제약물에는 DEA의 EPCS 가엄선이 더해집니다.
- EPCS 네 기둥(21 CFR Part 1311): 처방자 신원 확인, 이중 요소 인증(세 종류 중 둘), 인증 감사를 거친 응용 소프트웨어, 공유 금지된 서명 자격증명의 개인 통제.
- 추진선: SUPPORT법 2003절은 Part D 아래 규제약물의 전자처방을 요구하고, CMS가 2023년부터 현행 준수 틀로 집행하며, 기술 표준은 Part 1311로 돌아갑니다.
- 캘리포니아선: Health and Safety Code 11168조(AB 2789, 2022년 1월 1일 시행) — 처방은 원칙적으로 전자 전송, 예외는 기술·전력 고장, 주 밖 조제, 수의 처방 등 법정 경우로 한정되며 편의는 예외가 아닙니다.
- 책임: 약국이 종이·구두 처방을 받아도 그 자체로 위법이 아니고, 처리의 무게는 처방자 쪽에 있습니다.

*주: 개인 학습 노트이며 법률 자문도 의료 자문도 아닙니다. 출처: Drug Enforcement Administration(DEA)의 규제약물 전자처방 규칙(21 CFR Part 1311), SUPPORT for Patients and Communities Act 2003절과 Centers for Medicare & Medicaid Services(CMS)의 Part D 전자처방 준수 공개 기준, California Health and Safety Code 11168조(AB 2789, 2022년 1월 1일 시행), ESIGN법과 UETA 일반 배경. 집행과 예외의 세부 내용은 현행 공식 기준을 따릅니다. 이 글에는 약물 용량과 빈도가 없습니다. (초역으로 원어민 감수 대기 중입니다.)*

---

## Tiếng Việt (bản dịch sơ bộ · 初译待校)

### 1. Hai lớp: nền tảng của kê đơn điện tử thông thường và tuyến siết chặt cho thuốc kiểm soát

Kê đơn điện tử không do một bộ quy tắc duy nhất quản. Lớp thứ nhất là truyền đơn điện tử thông thường: người kê đơn ra đơn, hệ thống truyền tới nhà thuốc, nhà thuốc kiểm tra và cấp phát. Nền tảng pháp lý chủ yếu nằm ở luật dược của bang, coi đơn thuốc tạo và truyền bằng điện tử có giá trị như đơn giấy, kèm yêu cầu về tính xác thực, toàn vẹn và bảo mật. Phía sau là khung chữ ký điện tử chung — luật ESIGN liên bang và UETA (Uniform Electronic Transactions Act) của các bang — xác lập nguyên tắc hồ sơ và chữ ký điện tử không bị phủ nhận hiệu lực chỉ vì ở dạng điện tử. Lớp thứ hai là kê đơn điện tử cho thuốc kiểm soát, EPCS. Khi thuốc kiểm soát được ký điện tử, gánh nặng chống giả mạo chuyển từ giấy và nét chữ sang danh tính và hệ thống, nên liên bang đặt một bộ quy tắc nghiêm hơn kê đơn điện tử thông thường, do Drug Enforcement Administration (DEA) quản. Bài này đi theo lớp thứ hai, cộng tuyến thúc đẩy qua thanh toán của liên bang và tuyến bắt buộc của California; bài bổ sung chứ không lặp lại bài về kê thuốc kiểm soát qua telehealth (tuyến tư cách Ryan Haight) và bài về chất kiểm soát nói chung (phân loại, đăng ký DEA và CURES của California) trong kho này.

### 2. Quy tắc cứng liên bang của EPCS: bốn trụ cột của 21 CFR Part 1311

Quy tắc EPCS của DEA nằm tại 21 CFR Part 1311, với khung bốn trụ cột. Thứ nhất, xác minh danh tính người kê đơn: trước khi được ký điện tử, danh tính phải được xác minh qua quy trình mà quy tắc công nhận — người sau màn hình phải được chứng minh là chính người kê đơn có giấy phép. Thứ hai, xác thực hai yếu tố: ký đơn thuốc kiểm soát phải dùng hai trong ba loại yếu tố — yếu tố biết (dạng mật khẩu), yếu tố giữ (dạng token, vật mang khóa) và yếu tố sinh trắc (dạng vân tay); ba loại lấy hai, và chỉ một mật khẩu thì không đạt chuẩn ký của EPCS. Thứ ba, phần mềm ứng dụng phải qua kiểm toán chứng nhận: ứng dụng kê đơn điện tử của người kê đơn và nhà thuốc phải qua kiểm toán hoặc chứng nhận của bên thứ ba mà quy tắc yêu cầu, về quản lý danh tính, ký, lưu hồ sơ và kiểm soát an ninh; đổi hệ thống là phải kiểm tra lại trụ cột này. Thứ tư, kiểm soát cá nhân đối với chứng thư ký: chứng thư ký chỉ do chính người kê đơn kiểm soát, không được chia sẻ, không được giao người khác ký thay. Nhân viên có thể giúp nhập nội dung đơn, nhưng hành vi ký và chứng thư là của riêng người kê đơn. Hệ thống phía nhà thuốc cũng có nghĩa vụ tương ứng của Part 1311 về ứng dụng và hồ sơ, để mỗi đơn điện tử thuốc kiểm soát đều truy được về một người đã xác minh danh tính, một hành vi ký hai yếu tố và một phần mềm đã kiểm toán.

### 3. Tuyến thúc đẩy liên bang: mục 2003 của luật SUPPORT và Medicare Part D

Ngoài việc cho phép, luật liên bang còn thúc đẩy qua tuyến thanh toán. Mục 2003 của SUPPORT for Patients and Communities Act yêu cầu đơn thuốc kiểm soát thuộc Medicare Part D phải truyền bằng điện tử, theo cách EPCS. Việc thực thi nằm ở Centers for Medicare & Medicaid Services (CMS), cơ quan đã thúc đẩy tuân thủ từ năm 2023 theo khung tuân thủ đã công bố, với ngoại lệ và cách xử lý theo công bố hiện hành của CMS — chi tiết theo hướng dẫn hiện hành của CMS. Nắm hai điểm: đây là cú đẩy qua thanh toán Part D chứ không phải chuẩn ký mới — chuẩn kỹ thuật vẫn quay về Part 1311 — và nó chỉ bao phủ bối cảnh Part D, song song chứ không thay thế yêu cầu của luật bang.

### 4. Tuyến California: mục 11168 của Health and Safety Code, bắt buộc truyền điện tử và các ngoại lệ luật định

Tuyến California rộng hơn tuyến thanh toán liên bang vì nó quản chính đơn thuốc của California. Căn cứ là mục 11168 của Health and Safety Code, do AB 2789 ban hành, hiệu lực từ ngày 1 tháng 1 năm 2022. Quy tắc mặc định: đơn thuốc tại California phải được tạo và truyền bằng điện tử; giấy không còn là chuẩn thường ngày. Ngoại lệ đọc theo cấu trúc của chính điều luật, không tự nới hay thu hẹp; theo nhóm lớn gồm các tình huống truyền điện tử khách quan không thể thực hiện, như sự cố kỹ thuật hoặc điện; cấp phát ngoài California và các tình huốngข้าม bang khác; đơn thuốc thú y và các bối cảnh điều luật nêu tên; cùng các ngoại lệ liệt kê còn lại. Điểm chung của chúng là không thể hoặc không phù hợp, chứ không phải tiện lợi — thích dùng giấy không phải là ngoại lệ. Về trách nhiệm, hai điểm: phía nhà thuốc — nhận đơn giấy hoặc đơn miệng không vì thế mà vi phạm mục 11168, nghĩa vụ bắt buộc đặt ở phía người kê đơn; phía người kê đơn — truyền không bằng điện tử mà không có ngoại lệ là vấn đề của người kê đơn, theo khung hiện hành có thể dẫn tới chuyển hồ sơ lên hội đồng cấp phép cùng các hậu quả khác, theo điều luật và hướng dẫn hiện hành. Với thuốc kiểm soát tại California, yêu cầu Part 1311 liên bang và khung CURES chồng lên mục 11168: các tuyến cộng dồn, không phải chọn một.

### 5. Điểm chính

- Phân lớp: kê đơn điện tử thông thường dựa vào luật dược của bang (ESIGN và UETA chỉ là nền chung về chữ ký điện tử); thuốc kiểm soát cộng thêm tuyến EPCS nghiêm hơn của DEA.
- Bốn trụ cột EPCS (21 CFR Part 1311): xác minh danh tính người kê đơn, xác thực hai yếu tố (hai trong ba loại), phần mềm đã kiểm toán hoặc chứng nhận, và kiểm soát cá nhân không chia sẻ đối với chứng thư ký.
- Tuyến thúc đẩy: mục 2003 của luật SUPPORT yêu cầu thuốc kiểm soát trong Part D đi bằng điện tử; CMS thực thi từ năm 2023 theo khung tuân thủ hiện hành, và chuẩn kỹ thuật vẫn quay về Part 1311.
- Tuyến California: mục 11168 của Health and Safety Code (AB 2789, hiệu lực 1/1/2022) đặt truyền điện tử làm mặc định, ngoại lệ giới hạn ở các tình huống luật định như sự cố kỹ thuật hoặc điện, cấp phát ngoài bang và đơn thú y — tiện lợi không phải ngoại lệ.
- Trách nhiệm: nhà thuốc nhận đơn giấy hay đơn miệng không vì thế mà phạm luật; hậu quả rơi về phía người kê đơn.

*Lưu ý: Ghi chú học tập cá nhân; không phải tư vấn pháp lý cũng không phải tư vấn y tế. Nguồn: Drug Enforcement Administration (DEA), quy tắc kê đơn điện tử cho thuốc kiểm soát, 21 CFR Part 1311; SUPPORT for Patients and Communities Act, mục 2003, và hướng dẫn tuân thủ kê đơn điện tử Part D của Centers for Medicare & Medicaid Services (CMS); California Health and Safety Code mục 11168 (AB 2789, hiệu lực 1/1/2022); luật ESIGN và UETA làm nền chung. Chi tiết thực thi và ngoại lệ theo hướng dẫn chính thức hiện hành. Bài này không chứa chi tiết thuốc. (Bản dịch sơ bộ, chờ hiệu đính.)*

---

## हिन्दी (प्रारंभिक अनुवाद · 初译待校)

### 1. दो परतें: साधारण इलेक्ट्रॉनिक नुस्खे की नींव और नियंत्रित दवाओं की कड़ी रेखा

इलेक्ट्रॉनिक नुस्खा एक ही नियम-पुस्तिका से नहीं चलता। पहली परत साधारण इलेक्ट्रॉनिक प्रेषण है: नुस्खा-लेखक नुस्खा देता है, प्रणाली उसे फ़ार्मेसी तक भेजती है, फ़ार्मेसी जाँचकर दवा देती है। इसकी विधिक नींव मुख्यतः राज्य फ़ार्मेसी विधि में है, जो इलेक्ट्रॉनिक रूप से बनाए और भेजे गए नुस्खों को काग़ज़ी नुस्खों के समकक्ष मानती है, प्रामाणिकता, अखंडता और गोपनीयता की शर्तों के साथ। इसके पीछे इलेक्ट्रॉनिक हस्ताक्षर के सामान्य ढाँचे हैं — संघीय ESIGN Act और राज्यों का UETA (Uniform Electronic Transactions Act) — जो यह सिद्धांत स्थापित करते हैं कि इलेक्ट्रॉनिक अभिलेख या हस्ताक्षर केवल इलेक्ट्रॉनिक होने के कारण प्रभाव से वंचित नहीं होगा। दूसरी परत नियंत्रित दवाओं का इलेक्ट्रॉनिक नुस्खा, EPCS है। जब नियंत्रित दवाएँ इलेक्ट्रॉनिक रूप से हस्ताक्षरित हो सकती हैं, तो जालसाज़ी-रोध का भार काग़ज़ और हस्तलिपि से हटकर पहचान और प्रणालियों पर आ जाता है, इसलिए संघ ने साधारण ई-नुस्खे से कड़ा नियम-समूह जोड़ा, जिसका प्रशासन Drug Enforcement Administration (DEA) करता है। यह लेख उसी दूसरी परत को लेता है, साथ में संघ की भुगतान-प्रेरणा रेखा और कैलिफ़ोर्निया का अनिवार्य नियम। यह इस भंडार के टेलीहेल्थ से नियंत्रित दवा लिखने (Ryan Haight पात्रता रेखा) और नियंत्रित दवाओं के सामान्य ढाँचे (वर्गीकरण, DEA पंजीकरण और कैलिफ़ोर्निया का CURES) वाले लेखों का पूरक है, उनकी पुनरावृत्ति नहीं।

### 2. संघीय EPCS के कठोर नियम: 21 CFR Part 1311 के चार स्तंभ

DEA के EPCS नियम 21 CFR Part 1311 में हैं और उनका ढाँचा चार स्तंभों का है। पहला, नुस्खा-लेखक की पहचान-सत्यापन: इलेक्ट्रॉनिक हस्ताक्षर से पहले, नियम द्वारा मान्यता-प्राप्त प्रक्रिया से पहचान सत्यापित होनी चाहिए — पर्दे के पीछे का व्यक्ति वही लाइसेंसधारी नुस्खा-लेखक हो। दूसरा, द्वि-कारक प्रमाणीकरण: नियंत्रित दवा के नुस्खे पर हस्ताक्षर के लिए तीन कारक-वर्गों में से दो चाहिए — जानने वाला कारक (पासवर्ड-जैसा), रखने वाला कारक (टोकन या कुंजी-वाहक जैसा) और जीवमितीय कारक; तीन में से दो, केवल एक पासवर्ड EPCS हस्ताक्षर मानक को पूरा नहीं करता। तीसरा, प्रमाणित और ऑडिट की गई अनुप्रयोग-प्रणालियाँ: नुस्खा-लेखकों और फ़ार्मेसियों के इलेक्ट्रॉनिक नुस्खा अनुप्रयोगों को नियम की अपेक्षित तृतीय-पक्ष ऑडिट या प्रमाणन से गुज़रना होता है — पहचान प्रबंधन, हस्ताक्षर, अभिलेख-रक्षण और सुरक्षा नियंत्रणों पर; प्रणाली बदलने पर यह स्तंभ फिर से जाँचना होगा। चौथा, हस्ताक्षर साख का व्यक्तिगत नियंत्रण: हस्ताक्षर साख केवल नुस्खा-लेखक के अपने नियंत्रण में रहती है, साझा नहीं की जा सकती और किसी और को हस्ताक्षर के लिए नहीं दी जा सकती। कर्मचारी नुस्खे की सामग्री डालने में मदद कर सकते हैं, परंतु हस्ताक्षर का कार्य और साख नुस्खा-लेखक की अपनी है। फ़ार्मेसी पक्ष की प्रणालियों पर भी Part 1311 के संगत दायित्व हैं, ताकि हर नियंत्रित-दवा ई-नुस्खा एक सत्यापित व्यक्ति, एक द्वि-कारक हस्ताक्षर कार्य और एक ऑडिट की गई प्रणाली तक खोजा जा सके।

### 3. संघीय प्रेरणा रेखा: SUPPORT Act की धारा 2003 और Medicare Part D

अनुमति के आगे संघ भुगतान के रास्ते भी धकेलता है। SUPPORT for Patients and Communities Act की धारा 2003 कहती है कि Medicare Part D के अंतर्गत नियंत्रित दवाओं के नुस्खे इलेक्ट्रॉनिक रूप से, EPCS ढंग से, भेजे जाएँ। प्रवर्तन Centers for Medicare & Medicaid Services (CMS) के पास है, जो 2023 से अपने प्रकाशित अनुपालन ढाँचे के अनुसार अनुपालन आगे बढ़ा रहा है; अपवाद और प्रवर्तन व्यवस्था CMS के वर्तमान प्रकाशनों के अनुसार होगी — विवरण CMS के वर्तमान मार्गदर्शन से लें। दो बातें पकड़ें: यह Part D भुगतान-पक्ष का धक्का है, कोई नया हस्ताक्षर मानक नहीं — तकनीकी मानक Part 1311 ही रहता है — और यह केवल Part D परिवेश को ढकता है, राज्य विधि की आवश्यकताओं के साथ-साथ, उनकी जगह नहीं।

### 4. कैलिफ़ोर्निया रेखा: Health and Safety Code धारा 11168 का इलेक्ट्रॉनिक प्रेषण अनिवार्य नियम और उसके अपवाद

कैलिफ़ोर्निया की रेखा संघीय भुगतान रेखा से चौड़ी है क्योंकि वह कैलिफ़ोर्निया के नुस्खों को ही नियंत्रित करती है। Health and Safety Code धारा 11168, AB 2789 द्वारा अधिनियमित और 1 जनवरी 2022 से प्रभावी, डिफ़ॉल्ट नियम देती है: कैलिफ़ोर्निया में नुस्खे इलेक्ट्रॉनिक रूप से बनाए और भेजे जाएँगे; काग़ज़ अब सामान्य नहीं है। अपवाद विधान की अपनी संरचना से पढ़े जाएँगे, भावना से न बढ़ाए जाएँ न घटाए जाएँ; बड़े वर्गों में वे परिस्थितियाँ आती हैं जहाँ इलेक्ट्रॉनिक प्रेषण वस्तुतः असंभव हो, जैसे तकनीकी या बिजली की खराबी; कैलिफ़ोर्निया से बाहर वितरण और अन्य अंतर्राज्यीय परिस्थितियाँ; पशु-चिकित्सा नुस्खे और विधान द्वारा नामित अन्य परिदृश्य; और विधान के शेष सूचीबद्ध अपवाद। उनका साझा सूत्र असंभवता या अनुपयुक्तता है, सुविधा नहीं — काग़ज़ की पसंद कोई अपवाद नहीं है। दायित्व पर दो बिंदु: फ़ार्मेसी पक्ष — काग़ज़ी या मौखिक नुस्खा प्राप्त करने से फ़ार्मेसी अपने आप धारा 11168 का उल्लंघन नहीं करती; अनिवार्यता नुस्खा-लेखक पर है। नुस्खा-लेखक पक्ष — बिना अपवाद के इलेक्ट्रॉनिक रूप से न भेजना नुस्खा-लेखक की समस्या है, जो वर्तमान ढाँचे में, अन्य परिणामों के साथ, उसके लाइसेंस बोर्ड को संदर्भित किए जाने तक जा सकती है, जैसा विधान और बोर्ड मार्गदर्शन वर्तमान में कहते हैं। कैलिफ़ोर्निया में नियंत्रित दवाओं पर संघीय Part 1311 आवश्यकताएँ और CURES ढाँचा धारा 11168 के ऊपर जुड़ते हैं; रेखाएँ संचयी हैं, विकल्प नहीं।

### 5. मुख्य बिंदु

- परतें: साधारण ई-नुस्खा राज्य फ़ार्मेसी विधि पर टिका है (ESIGN और UETA केवल इलेक्ट्रॉनिक हस्ताक्षर की सामान्य पृष्ठभूमि हैं); नियंत्रित दवाएँ DEA की कड़ी EPCS रेखा जोड़ती हैं।
- EPCS के चार स्तंभ (21 CFR Part 1311): पहचान-सत्यापन, द्वि-कारक प्रमाणीकरण (तीन वर्गों में से कोई दो), ऑडिट या प्रमाणित अनुप्रयोग, और हस्ताक्षर साख का व्यक्तिगत, असाझा नियंत्रण।
- प्रेरणा: SUPPORT Act धारा 2003 Part D की नियंत्रित दवाओं के नुस्खों के इलेक्ट्रॉनिक जाने को कहती है; CMS 2023 से अपने वर्तमान अनुपालन ढाँचे के तहत प्रवर्तन कर रहा है, और तकनीकी मानक Part 1311 ही रहता है।
- कैलिफ़ोर्निया: Health and Safety Code धारा 11168 (AB 2789, 1 जनवरी 2022 से प्रभावी) इलेक्ट्रॉनिक प्रेषण को डिफ़ॉल्ट बनाती है, अपवाद तकनीकी या बिजली की खराबी, राज्य से बाहर वितरण और पशु-चिकित्सा नुस्खों जैसे वैधानिक मामलों तक सीमित हैं — सुविधा अपवाद नहीं है।
- दायित्व: काग़ज़ी या मौखिक नुस्खा प्राप्त करने से फ़ार्मेसी कानून नहीं तोड़ती; परिणाम नुस्खा-लेखक पक्ष पर पड़ते हैं।

*टिप्पणी: केवल व्यक्तिगत अध्ययन नोट; विधिक सलाह नहीं, चिकित्सा सलाह नहीं। स्रोत: Drug Enforcement Administration (DEA), नियंत्रित दवाओं के इलेक्ट्रॉनिक नुस्खे, 21 CFR Part 1311; SUPPORT for Patients and Communities Act, धारा 2003, और Centers for Medicare & Medicaid Services (CMS) का Part D इलेक्ट्रॉनिक-नुस्खा अनुपालन मार्गदर्शन; California Health and Safety Code धारा 11168 (AB 2789, 1 जनवरी 2022 से प्रभावी); ESIGN Act और UETA सामान्य पृष्ठभूमि के रूप में। प्रवर्तन विवरण और अपवाद वर्तमान आधिकारिक मार्गदर्शन के अनुसार होंगे। इस लेख में दवा का कोई विवरण नहीं है। (प्रारंभिक अनुवाद, समीक्षा लंबित।)*
