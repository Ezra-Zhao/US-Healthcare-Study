# HIPAA 与患者权利概览

这篇讲什么：
- HIPAA（1996 年联邦法）到底管什么：它约束的是医院、诊所、保险公司、药房这些机构怎么处理你的健康信息，不是"谁都不能谈你的病情"这么简单。
- 患者手里的实权：查阅和复制自己的病历、要求更正、知道病历被披露给了谁、拒绝某些分享——以及行使这些权利的实际路径。
- 两条容易混淆的线：急诊不能拒诊靠的是 EMTALA；知情同意主要在州法里。另附联邦与州的分工：执照归州管，部分州的隐私法比 HIPAA 更严。

---

## 一、HIPAA 管什么：机构的义务，不是患者的枷锁

### 中文
HIPAA 全称 Health Insurance Portability and Accountability Act，1996 年通过。它在隐私方面的核心文件是 HHS（美国卫生与公众服务部）制定的《隐私规则》（Privacy Rule），约束对象叫"受约束实体"（Covered Entities）：医疗服务提供者（医院、诊所、药师等，凡是电子化传输健康信息的）、健康保险计划、医疗信息交换中心（Clearinghouse），以及它们的业务伙伴（Business Associates，如账单公司、云服务商）。

它保护的是 PHI（Protected Health Information，受保护健康信息）——能对应到个人的诊断、治疗、付款信息。规则的基本盘：机构只能在治疗、付款、医疗运营（Treatment / Payment / Health Care Operations，简称 TPO）范围内使用和披露 PHI，超出这个范围原则上要患者书面授权（Authorization）；机构的使用和披露还受"最小必要"（Minimum Necessary）标准约束——只用完成那件事所必需的最少信息（治疗所需的披露是例外，不受此限）。与之配套的还有《安全规则》（Security Rule，管电子病历的系统安全）和《泄露通知规则》（Breach Notification Rule，信息泄露后必须通知受影响的个人和 HHS）。

两个常见误解要澄清。第一，HIPAA 不约束普通人——朋友、雇主（在其雇主身份下）、记者问你病情，不违反 HIPAA，他们不在约束名单里。第二，HIPAA 本身**没有给患者个人起诉的权利**（No private right of action）：觉得机构违规，向 HHS 的民权办公室（OCR）投诉，由政府调查处罚；想让法院判赔，通常要走州法的其他路径（如州隐私法、侵权法）。

### English
HIPAA — the Health Insurance Portability and Accountability Act of 1996 — protects health information mainly through HHS's Privacy Rule. It binds "covered entities": health care providers who transmit health information electronically (hospitals, clinics, pharmacies), health plans, and health care clearinghouses — plus their business associates, such as billing companies and cloud vendors.

What it protects is PHI (protected health information): diagnosis, treatment, and payment information that can be tied to an individual. The baseline rule: PHI may be used and disclosed for treatment, payment, and health care operations (TPO); most other uses require the patient's written authorization, and uses and disclosures are subject to the "minimum necessary" standard — only the least information needed for the task (disclosures for treatment are an exception to that standard). Two companion rules matter as well: the Security Rule (safeguards for electronic PHI) and the Breach Notification Rule (affected individuals and HHS must be notified after a breach).

Two misconceptions are worth clearing up. First, HIPAA does not bind ordinary people — a friend, an employer acting as an employer, or a journalist asking about your condition violates no HIPAA rule, because they are not on the covered list. Second, HIPAA gives patients **no private right of action**: if an institution mishandles your information, you complain to the HHS Office for Civil Rights (OCR), which investigates and can impose penalties. Compensation through a court usually has to run through other routes, such as state privacy statutes or tort law.

### Español (译稿)
La HIPAA —Health Insurance Portability and Accountability Act, de 1996— protege la información sanitaria principalmente mediante la Privacy Rule del HHS (Departamento de Salud y Servicios Humanos). Obliga a las «entidades cubiertas» (covered entities): proveedores sanitarios que transmiten información de salud electrónicamente (hospitales, clínicas, farmacias), planes de salud y centros de compensación (clearinghouses), además de sus socios comerciales (business associates), como empresas de facturación o proveedores de nube.

Lo protegido es la PHI (protected health information): información de diagnóstico, tratamiento y pago que puede vincularse a una persona. La regla de base: la PHI puede usarse y divulgarse para tratamiento, pago y operaciones sanitarias (TPO); la mayoría de los demás usos requiere la autorización escrita del paciente, y los usos y divulgaciones se rigen por el principio de «mínimo necesario» (minimum necessary): solo la información imprescindible para la tarea (las divulgaciones con fines de tratamiento son una excepción a este principio). La acompañan la Security Rule (salvaguardas para la PHI electrónica) y la Breach Notification Rule (obligación de notificar a las personas afectadas y al HHS tras una brecha de seguridad).

Conviene aclarar dos malentendidos. Primero, la HIPAA no obliga a las personas comunes: un amigo, un empleador en su condición de tal o un periodista que pregunta por su enfermedad no infringe la HIPAA, porque no están en la lista de entidades cubiertas. Segundo, la HIPAA **no otorga a los pacientes un derecho de acción privada**: si una institución maneja mal su información, la queja va a la Oficina de Derechos Civiles (OCR) del HHS, que investiga y puede sancionar. Una indemnización judicial suele tener que buscarse por otras vías, como las leyes estatales de privacidad o la responsabilidad civil.

---

## 二、患者权利清单：病历首先是你的

### 中文
HIPAA 给患者最实用的几项权利，都在《隐私规则》里，落到行动上是这样：

- **查阅与复制病历（Right of Access）**：你有权查看并取得自己病历的副本，纸质或电子形式都可。机构一般须在 30 天内提供（可依法延长一次并书面说明）。费用只能是合理的复制/人工成本，不能漫天要价。这两年实务上更快：多数机构的患者门户（Patient Portal，如 MyChart）里化验结果、影像报告直接可见——联邦《21 世纪治愈法案》（21st Century Cures Act）的"信息封锁"（Information Blocking）禁令要求机构不得无故拖延向患者开放电子病历。
- **要求更正（Amendment）**：发现病历写错（过敏史、诊断、用药记录），可以书面要求更正；机构可以拒绝，但必须书面说明理由，你的异议声明会附在病历里。
- **披露清单（Accounting of Disclosures）**：有权知道过去六年里自己的 PHI 披露给过哪些机构（治疗、付款、运营类的常规披露不在此清单范围内，这是常被忽略的例外）。
- **限制与保密沟通**：可以要求机构限制某些披露；特别地，如果你自费全额支付了某项服务，你有权要求机构不把这项信息披露给你的保险计划，机构必须同意。也可以要求换一种联系方式（比如不要往家里打电话）。
- **指定个人代表**：未成年人的父母、持医疗代理权（Health Care Proxy / Power of Attorney）的人，可以代你行使这些权利；各州对未成年人自己可控的病历范围（性健康、心理健康等）另有规定。

行使路径：找机构的隐私官（Privacy Officer）或病历科（Medical Records / HIM 部门），多数有固定表格。被拒绝或拖延时，向 HHS OCR 在线投诉是免费且正式的下一步。

### English
The most practical rights HIPAA gives patients, translated into actions:

- **Right of access**: you may inspect and obtain a copy of your medical records, on paper or electronically. The institution generally must respond within 30 days (one extension is allowed, with a written explanation), and fees are limited to reasonable copying/labor costs. In practice it is often faster now: patient portals (such as MyChart) show lab results and imaging reports directly, and the information-blocking rules under the 21st Century Cures Act bar institutions from unreasonably delaying patients' access to their electronic records.
- **Amendment**: if your record contains an error — an allergy, diagnosis, or medication listed wrongly — you may request a correction in writing. The institution may deny it, but must explain in writing, and your statement of disagreement goes into the record.
- **Accounting of disclosures**: you may learn which organizations received your PHI over the past six years — with a commonly missed exception: routine disclosures for treatment, payment, and operations are not included in this accounting.
- **Restrictions and confidential communications**: you may ask an institution to limit certain disclosures. Notably, if you pay in full out of pocket for a service, you have the right to require that the information not be disclosed to your health plan, and the institution must honor that. You may also request contact by alternative means or at an alternative location.
- **Personal representatives**: parents of minors and holders of a health care proxy / power of attorney can exercise these rights on your behalf; state law carves out areas (such as sexual and mental health) where minors control their own records.

How to act: contact the institution's Privacy Officer or medical records (HIM) department; most have standard forms. If you are refused or stonewalled, a complaint to the HHS Office for Civil Rights is free and is the formal next step.

### Español (译稿)
Los derechos más prácticos que la HIPAA otorga a los pacientes, traducidos a acciones:

- **Derecho de acceso**: puede consultar y obtener copia de su historia clínica, en papel o en formato electrónico. La institución debe responder por lo general en 30 días (se permite una prórroga con explicación escrita), y las tarifas se limitan a costes razonables de copia y gestión. En la práctica hoy suele ser más rápido: los portales del paciente (como MyChart) muestran directamente resultados de laboratorio e informes de imagen, y las normas contra el bloqueo de información (information blocking) de la ley 21st Century Cures Act prohíben retrasar sin justificación el acceso del paciente a su historia electrónica.
- **Rectificación (amendment)**: si su historia contiene un error —una alergia, un diagnóstico o un medicamento mal registrados— puede pedir la corrección por escrito. La institución puede denegarla, pero debe explicarlo por escrito, y su declaración de desacuerdo quedará incorporada a la historia.
- **Registro de divulgaciones (accounting of disclosures)**: puede saber qué organizaciones recibieron su PHI en los últimos seis años, con una excepción que suele pasarse por alto: las divulgaciones rutinarias para tratamiento, pago y operaciones no figuran en ese registro.
- **Restricciones y comunicaciones confidenciales**: puede pedir que se limiten ciertas divulgaciones. En particular, si paga íntegramente de su bolsillo un servicio, tiene derecho a exigir que esa información no se divulgue a su plan de salud, y la institución debe aceptarlo. También puede pedir ser contactado por medios o en lugares alternativos.
- **Representantes personales**: los padres de menores y quienes tengan un poder de representación sanitaria (health care proxy / power of attorney) pueden ejercer estos derechos en su nombre; las leyes estatales reservan ámbitos (como salud sexual o mental) en los que el menor controla su propia historia.

Cómo ejercerlos: acuda al responsable de privacidad (Privacy Officer) o al departamento de historias clínicas (Medical Records / HIM); la mayoría dispone de formularios estándar. Si se lo deniegan o le dan largas, la queja ante la Oficina de Derechos Civiles del HHS es gratuita y es el paso formal siguiente.

---

## 三、EMTALA：急诊不能因为没钱拒诊

### 中文
电影里"没保险被推出急诊室"的情节，在法律上被一条 1986 年的联邦法堵死了：EMTALA（Emergency Medical Treatment and Labor Act）。它适用于参加 Medicare 的医院（事实上覆盖几乎所有有急诊室的医院），核心两条义务：

1. **医学筛查（Medical Screening Examination）**：任何人来到急诊，医院必须提供适当的筛查来判断是否存在急症（Emergency Medical Condition），不能因为支付能力、保险状态、身份而推迟或拒绝筛查。
2. **稳定病情（Stabilization）**：查出急症后，必须先给予稳定病情的治疗，或在符合严格条件时转院（转院要有患者/家属知情同意、接收方确认、转运风险说明等，俗称"适当转院"）。分娩中的产妇也在保护范围内。

边界也要说清：EMTALA 只管急诊阶段的筛查与稳定，不保证后续免费治疗，也不覆盖普通门诊；稳定之后的费用、账单照常存在。它和 HIPAA 是两部不同的法，经常被混在一起谈，其实一个管"不能拒之门外"，一个管"信息不能乱给"。

### English
The movie scene of an uninsured patient being wheeled out of the ER is blocked by a 1986 federal statute: EMTALA (the Emergency Medical Treatment and Labor Act). It applies to Medicare-participating hospitals — effectively nearly every hospital with an emergency department — and imposes two core duties:

1. **Medical screening examination**: anyone who comes to the emergency department must receive an appropriate screening to determine whether an emergency medical condition exists. The hospital may not delay or deny that screening because of ability to pay, insurance status, or identity.
2. **Stabilization**: if an emergency condition is found, the hospital must provide treatment to stabilize it, or transfer the patient only under strict conditions — informed consent, a receiving facility that has agreed, documentation of risks and benefits (an "appropriate transfer"). Patients in active labor are expressly protected.

The limits matter too: EMTALA governs screening and stabilization in the emergency setting. It does not make follow-up care free, does not apply to ordinary clinic visits, and bills after stabilization still exist. EMTALA and HIPAA are different statutes that are often conflated — one says "you cannot be turned away," the other says "your information cannot be handed around."

### Español (译稿)
La escena cinematográfica del paciente sin seguro expulsado de urgencias está bloqueada por una ley federal de 1986: la EMTALA (Emergency Medical Treatment and Labor Act). Se aplica a los hospitales que participan en Medicare —en la práctica, casi todos los que tienen servicio de urgencias— e impone dos obligaciones centrales:

1. **Examen médico de cribado (medical screening examination)**: toda persona que llega a urgencias debe recibir un examen adecuado para determinar si existe una condición médica de emergencia. El hospital no puede retrasar ni negar ese examen por capacidad de pago, situación del seguro o identidad.
2. **Estabilización**: si se confirma una condición de emergencia, el hospital debe dar el tratamiento necesario para estabilizarla, o trasladar al paciente solo bajo condiciones estrictas: consentimiento informado, centro receptor que haya aceptado, documentación de riesgos y beneficios (un «traslado apropiado»). Las mujeres de parto están expresamente protegidas.

También hay que conocer los límites: la EMTALA regula el cribado y la estabilización en el contexto de urgencias. No hace gratuita la atención posterior, no se aplica a las consultas ordinarias, y las facturas tras la estabilización siguen existiendo. La EMTALA y la HIPAA son leyes distintas que a menudo se confunden: una dice «no pueden rechazarte» y la otra «tu información no puede divulgarse libremente».

---

## 四、知情同意在州法里，执照也在州里

### 中文
同意（Informed Consent）不是 HIPAA 的内容。手术、侵入性检查、麻醉这些要签的知情同意书，规则主要来自各州法律和判例：医生须告知诊断、拟做操作的性质与风险、替代方案及各自风险、不做的后果，患者（或其代理人）在理解后自愿同意。紧急情况下人已无意识又无法联系代理人时，有"紧急例外"，先救人再补程序。各州对同意的形式（书面/口头）、见证、语言翻译的要求各不相同。

联邦与州的分工，放在医疗领域是这样一张图：

- **联邦管**：HIPAA 隐私底线、EMTALA 急诊义务、Medicare/Medicaid 的支付规则、FDA 管药品和医疗器械上市、DEA 管管制药。
- **州管**：医生、护士、药师等所有职业的执照发放与纪律（State Boards）、医院执照、医疗责任（Malpractice）诉讼规则、知情同意细则、州自己的隐私法。
- **州法可以更严**：HIPAA 是"地板"不是"天花板"——州隐私法比 HIPAA 更保护患者的，按更严的执行（Preemption 规则：HIPAA 不推翻更严格的州法）。典型例子是加州的《医疗信息保密法》（CMIA, California Confidentiality of Medical Information Act），它约束范围更宽，还允许患者个人起诉索赔，正好补上 HIPAA 没有私人诉权的缺口。

所以遇到权利问题，排查顺序是：先 HIPAA（联邦底线）→ 再本州隐私法与执照法（往往更细、更严）→ 最后机构自己的政策（只能比法律更保护患者，不能更松）。

### English
Informed consent is not part of HIPAA. The consent forms you sign for surgery, invasive procedures, and anesthesia are governed mainly by state statutes and case law: the physician must explain the diagnosis, the nature and risks of the proposed procedure, the alternatives and their risks, and the consequences of declining, and the patient (or representative) must agree voluntarily after understanding. Emergencies have an exception — when a patient is unconscious and no representative is reachable, treatment proceeds first. States differ on form (written vs oral), witnesses, and interpreter requirements.

The federal–state map in health care looks like this:

- **Federal**: the HIPAA privacy floor, EMTALA emergency duties, Medicare/Medicaid payment rules, FDA approval of drugs and devices, DEA control of controlled substances.
- **State**: licensure and discipline of every health profession (state boards), hospital licensing, medical-malpractice rules, informed-consent specifics, and state privacy statutes.
- **States may be stricter**: HIPAA is a floor, not a ceiling. Where a state privacy law protects patients more than HIPAA, the stricter law controls (the preemption rule: HIPAA does not displace more stringent state law). A textbook example is California's CMIA (Confidentiality of Medical Information Act), which reaches further than HIPAA and — unlike HIPAA — allows patients to sue for damages themselves, filling exactly the gap HIPAA leaves.

So when a rights question comes up, work in this order: HIPAA (the federal floor) → your state's privacy and licensing law (often more detailed and stricter) → the institution's own policies (which may only protect patients more than the law, never less).

### Español (译稿)
El consentimiento informado no forma parte de la HIPAA. Los formularios que se firman para cirugías, procedimientos invasivos y anestesia se rigen principalmente por las leyes y la jurisprudencia estatales: el médico debe explicar el diagnóstico, la naturaleza y los riesgos del procedimiento propuesto, las alternativas y sus riesgos, y las consecuencias de rechazarlo; el paciente (o su representante) debe aceptar voluntariamente tras comprenderlo. En emergencias hay una excepción: si el paciente está inconsciente y no se puede localizar a un representante, se trata primero. Los estados difieren en la forma (escrita u oral), los testigos y los requisitos de intérprete.

El mapa federal-estatal en sanidad es el siguiente:

- **Ámbito federal**: el suelo de privacidad de la HIPAA, las obligaciones de urgencias de la EMTALA, las reglas de pago de Medicare/Medicaid, la aprobación de medicamentos y dispositivos por la FDA y el control de sustancias por la DEA.
- **Ámbito estatal**: licencias y disciplina de todas las profesiones sanitarias (juntas estatales), licencias hospitalarias, normas de responsabilidad médica (malpractice), detalles del consentimiento informado y leyes estatales de privacidad.
- **Los estados pueden ser más estrictos**: la HIPAA es un suelo, no un techo. Cuando una ley estatal de privacidad protege más al paciente que la HIPAA, se aplica la más estricta (regla de preemption: la HIPAA no desplaza las leyes estatales más rigurosas). Un ejemplo clásico es la CMIA de California (Confidentiality of Medical Information Act), de alcance más amplio que la HIPAA y que —a diferencia de esta— sí permite al paciente demandar por daños, cubriendo justo el hueco que deja la HIPAA.

Ante un problema de derechos, el orden de revisión es: primero la HIPAA (suelo federal); después la ley estatal de privacidad y licencias (a menudo más detallada y estricta); por último, las políticas de la propia institución (que solo pueden proteger al paciente más que la ley, nunca menos).

---

参考来源：HHS Office for Civil Rights 的 HIPAA 官方说明与 Privacy Rule 条文（45 CFR Part 164）、CMS 的 EMTALA 官方资料、加州 CMIA（Civil Code §56 起）、21st Century Cures Act 信息封锁规则（ONC）。

*本文为个人学习笔记，不构成法律建议，也不构成医疗建议。具体权利纠纷请咨询医疗法律师或向 HHS OCR、各州执照委员会咨询投诉。*
