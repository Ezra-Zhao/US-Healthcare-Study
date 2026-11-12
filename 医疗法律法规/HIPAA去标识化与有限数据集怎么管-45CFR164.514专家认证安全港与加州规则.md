# HIPAA 去标识化与有限数据集怎么管：45 C.F.R. § 164.514 的专家认证、安全港与加州规则

这篇讲什么：
- 医疗法律法规板块的 HIPAA 线已有总览、民事罚款与执法、泄露通知、访问权与修正权、去世后病历隐私等专篇，唯独「数据怎样才算不再是 PHI」这一格没有本体专篇——本篇专拆 45 C.F.R. § 164.514 的去标识化（de-identification）与有限数据集（limited data set）。
- 选题经 ls/grep 实查：任务单法规候选三位——HIPAA 泄露通知规则已有本体专篇（《医疗信息泄露怎么管》）、患者医疗记录获取权与复制费已有本体专篇（《病历能看能改吗》）、医院价格透明规则已有本体专篇（《医院价格透明怎么管》，45 C.F.R. Part 180 全覆盖），三位均属撞题放弃；「164.514」与「有限数据集」全仓零命中、去标识化仅在医疗 AI 篇一段带过，无本体专篇，故改选本篇。
- 条文以 eCFR 现行文本为准，方法细节对照 HHS 民权办公室（OCR）的去标识化方法指南。全篇不写任何药物剂量与频次。

## 中文主文

### 一、先定性：去标识化完成，数据就不再是 PHI

§ 164.514(a) 的标准只有一句：健康信息若不能识别个人、且没有合理依据认为它能被用来识别个人，就不再是「可识别个人健康信息」。法律后果很直接：去标识化数据不再是受保护健康信息（PHI），使用与披露脱离 HIPAA 隐私规则的授权框架——研究、质量分析、产品开发拿到这种数据，不需要逐人授权，也不再受最小必要与披露记账那一套约束。但「不再是 PHI」是一句有条件的话：必须经本篇第二、三节的两种法定方法之一做出来，自己觉得「看不出是谁」不算数。把姓名删掉就宣布去标识化，是实务中最常见的误判。

### 二、方法一：专家认证法（§ 164.514(b)(1)）

第一条路靠人：由具备公认统计与科学原理知识和经验的人（专家）实际运用这些原理与方法，判定该信息被预期接收方单独或结合其他可得信息用来识别个人的风险「非常小」（very small），并把所用的方法与支持结论的分析结果形成文档留存。三个要点：专家不要求某个特定学位或证照，关键是统计与科学方法上的真实胜任；结论必须结合预定接收方能拿到的数据环境判断，同一数据集换一个接收方，风险结论可能翻转；文档要留，口头说「风险很小」不构成认证。这条路的好处是灵活——可以保留更多分析价值高的数据元素（如较细的日期与地理粒度），代价是要请到合格专家并把分析做扎实。

### 三、方法二：安全港法（§ 164.514(b)(2)）——删满 18 类，外加无实际知悉

第二条路靠清单：把下列 18 类标识符全部去掉（对象包括个人本人及其亲属、雇主与家庭成员），且受保主体对剩余信息能识别个人一事没有实际知悉（actual knowledge），才算完成。18 类逐项列明：

1. 姓名；2. 州以下各级地理细分（街道地址、城市、县、邮政编码及等效地理编码，邮编仅在下文条件下保留前三位）；3. 与个人直接相关的全部日期元素（只可保留年份）以及 89 岁以上年龄（须合并为「90 岁或以上」一档）；4. 电话号码；5. 传真号码；6. 电子邮箱地址；7. 社会安全号码；8. 病历号；9. 健康计划受益人号码；10. 账号；11. 证书与执照号码；12. 车辆标识符与序列号（含车牌）；13. 器械标识符与序列号；14. 网络地址（URL）；15. IP 地址；16. 生物识别标识符（含指纹与声纹）；17. 全面部照片及可比图像；18. 任何其他唯一识别号码、特征或代码（兜底项，第 (c) 款的再识别码除外）。

两处细则最容易翻车。邮编：同一前三位所覆盖区域按人口普查局现行公开数据合计人口超过 20,000 人时，前三位可以保留；否则一律改为 000。算例（本地复算两遍）：某前三位区域合计人口 18,500 人，20,000 减 18,500 等于 1,500，未过线，前三位须改为 000。年龄：92 岁不能写 92，只能写「90 岁或以上」；同理入院、出院、出生、死亡等日期只留年份，月与日都属于要删的日期元素。

### 四、再识别码（§ 164.514(c)）：留一把钥匙，但钥匙不能照着锁配

受保主体可以给去标识化信息配一个代码或类似记录，方便日后把数据重新对应到个人。条件两条：代码不得由该个人的相关信息推导出来或与之相关（不能拿生日、病历号片段拼码），且再识别的机制不得外泄。重新识别出来的信息，重新回到 PHI 的待遇。这一节的存在说明去标识化与匿名化不是同义词：HIPAA 允许「可逆的去标识化」，但把钥匙的保管条件写死。

### 五、有限数据集（§ 164.514(e)）：中间车道——仍是 PHI，但免了授权

很多研究场景里，安全港删得太多（日期全删，研究没法做），专家认证又请不起。§ 164.514(e) 给了中间车道：有限数据集去掉 16 类直接标识符，但可以保留日期（就诊、入院、出院、死亡等）与城市、州、邮编等地理信息。代价有三：第一，它仍然是 PHI，没有脱离隐私规则；第二，只能用于三类目的——研究、公共卫生、医疗运营，其他目的不行；第三，披露前必须与接收方签数据使用协议（data use agreement），协议须写明允许的用途与使用者、接收方的保障义务、不得再识别个人或联系个人、发现违规使用须报告等条款。手续上它免了逐人授权，但协议就是它的门票，免协议交付有限数据集，等于把中间车道当成了去标识化车道。

### 六、三条车道对比与常见误区

- 完全 PHI：授权路径全套适用；有限数据集：仍是 PHI、三类目的、必须有数据使用协议；去标识化数据：不是 PHI、用途脱离授权框架，但必须经专家认证或安全港两种方法之一做成。
- 误区一：只删姓名和病历号就叫去标识化——18 类没删满，安全港不成立。
- 误区二：把有限数据集当去标识化数据对外发——它仍是 PHI，无协议披露是违规披露。
- 误区三：安全港里保留完整出生日期「只精确到年」——月日必须删，只留年份，年份之外的日期元素一个都留不得。
- 误区四：专家认证做完不留档——(b)(1) 明文要求记录方法与结果，无文档的认证在审计里等于没做。
- 误区五：以为去标识化是一劳永逸——接收方手里的外部数据在变，当初的「无合理依据」判断在新数据环境下可能不再成立，专家路线的结论尤其要定期回看（此为审慎实务提示，非条文硬性期限）。

### 七、加州加层：联邦脱钩，不等于加州脱钩

加州单独注明：加州《医疗信息保密法》（CMIA，《民法典》第 56 条起）对医疗服务提供者与健康计划持有医疗信息的披露另有独立约束，一套数据按 HIPAA 完成去标识化，不自动等于它在加州法下可以任意使用与披露——签数据协议、评估州法口径时要把两层分开核。另外，《加州消费者隐私法》（CCPA，经 CPRA 修订）对受 HIPAA 与 CMIA 管辖的 PHI 设有豁免、同时对「去标识化」数据有自己的定义与要求；同一批数据在不同法域下的身份可能不同，交付前逐层确认，不要拿联邦结论一路通行。此节为口径提示，具体条文适用以现行文本与专业意见为准。

来源口径：45 C.F.R. § 164.514 现行条文（eCFR，含 (a) 标准、(b)(1) 专家认证、(b)(2) 安全港 18 类与 20,000 人邮编线、(c) 再识别码、(e) 有限数据集与数据使用协议）；HHS 民权办公室《Guidance Regarding Methods for De-identification of Protected Health Information in Accordance with HIPAA》；加州《民法典》第 56 条起（CMIA）与第 1798.100 条起（CCPA）的豁免与定义口径。

声明：个人学习笔记，不构成医疗建议，也不构成法律意见；全文不涉及药物剂量与频次。

---

## English

Scope: within this repository's HIPAA line (overview, civil money penalties and enforcement, breach notification, access and amendment rights, privacy after death), the question of when data stops being protected health information had no dedicated article. This article covers de-identification and limited data sets under 45 C.F.R. § 164.514, following the current eCFR text and the HHS Office for Civil Rights guidance on de-identification methods. The three candidate topics originally queued for this slot — breach notification, the patient access right and copy fees, and hospital price transparency under Part 180 — were each found on inspection to already have a dedicated article, so this uncovered section was selected instead.

The standard in § 164.514(a) is one sentence: health information that does not identify an individual, and for which there is no reasonable basis to believe it can be used to identify an individual, is not individually identifiable health information. Properly de-identified data is therefore no longer PHI, and its use and disclosure leave the HIPAA authorization framework. But the status is conditional: de-identification must be achieved through one of the two methods the rule prescribes. Deleting names and declaring the job done is the most common error in practice.

Method one is expert certification under § 164.514(b)(1): a person with appropriate knowledge of and experience with generally accepted statistical and scientific principles and methods applies those methods, determines that the risk is very small that the information could be used, alone or in combination with other reasonably available information, by an anticipated recipient to identify an individual, and documents the methods and the results of the analysis. No particular degree or credential is required, but the analysis is recipient-specific — the same data set can pass for one recipient and fail for another — and undocumented certification does not count.

Method two is the Safe Harbor under § 164.514(b)(2): remove all 18 listed identifier types for the individual and for relatives, employers, and household members, and have no actual knowledge that the remaining information could identify someone. The 18 types are: names; geographic subdivisions smaller than a state (with the ZIP rule below); all date elements except year, plus ages over 89 aggregated as 90 or older; telephone numbers; fax numbers; email addresses; Social Security numbers; medical record numbers; health plan beneficiary numbers; account numbers; certificate and license numbers; vehicle identifiers and serial numbers including license plates; device identifiers and serial numbers; web URLs; IP addresses; biometric identifiers including finger and voice prints; full-face photographic and comparable images; and any other unique identifying number, characteristic, or code. The ZIP detail: the first three digits may be kept only if the combined population of the area sharing them, per current Census Bureau data, exceeds 20,000 people; otherwise they become 000. Worked example: an area of 18,500 people falls 20,000 minus 18,500 equals 1,500 short, so the prefix must be changed to 000. Dates keep the year only, and a 92-year-old is recorded as 90 or older, never as 92.

Section 164.514(c) permits a re-identification code: the covered entity may assign a code allowing it to re-identify the data, provided the code is not derived from information about the individual and the re-identification mechanism is not disclosed. Data so re-identified is PHI again.

Section 164.514(e) creates the middle lane, the limited data set. It strips 16 categories of direct identifiers but may retain dates and city, state, and ZIP code. It remains PHI; it may be used or disclosed only for research, public health, or health care operations; and every disclosure requires a data use agreement that sets the permitted uses and users, binds the recipient to safeguards, bars re-identification and contact with individuals, and requires reporting of impermissible uses. No individual authorization is needed, but the agreement is the ticket — handing over a limited data set without one is an impermissible disclosure dressed as de-identification.

Frequent errors: treating a name-deleted file as de-identified when the 18 types were not all removed; treating a limited data set as de-identified data; keeping full dates under Safe Harbor when only the year may stay; obtaining an expert opinion without keeping the documentation § 164.514(b)(1) requires; and treating de-identification as permanent when changes in a recipient's other data holdings can undermine the original no-reasonable-basis judgment over time.

California layer: the Confidentiality of Medical Information Act (Civil Code section 56 et seq.) independently restricts disclosure of medical information held by providers and plans, so a data set that clears HIPAA de-identification is not automatically free for every use under California law. The California Consumer Privacy Act, as amended by the CPRA, exempts PHI governed by HIPAA and the CMIA while imposing its own definition of deidentified data. The layers must be checked separately.

Sources: 45 C.F.R. § 164.514 (eCFR current text); HHS Office for Civil Rights, Guidance Regarding Methods for De-identification of Protected Health Information; California Civil Code sections 56 et seq. and 1798.100 et seq.

*Personal study notes only; not medical advice and not legal advice. This article contains no drug dose or frequency.*

---

## Español (初译待校)

Alcance: dentro de la línea HIPAA de este repositorio (panorama, sanciones civiles y aplicación, notificación de brechas, derechos de acceso y rectificación, privacidad tras el fallecimiento), la pregunta de cuándo unos datos dejan de ser información de salud protegida no tenía artículo propio. Este artículo cubre la desidentificación y los conjuntos de datos limitados según 45 C.F.R. § 164.514, con el texto vigente del eCFR y la guía de métodos de la Oficina de Derechos Civiles del HHS. Los tres temas candidatos previstos para este turno — notificación de brechas, derecho de acceso del paciente y tarifas de copia, y transparencia de precios hospitalarios de la Parte 180 — resultaron tener ya artículo propio al revisarlos, por lo que se eligió esta sección sin cobertura.

La norma de § 164.514(a) cabe en una frase: la información de salud que no identifica a una persona, y respecto de la cual no existe base razonable para creer que puede usarse para identificarla, no es información de salud individualmente identificable. Los datos correctamente desidentificados dejan de ser PHI y su uso y divulgación salen del marco de autorizaciones de HIPAA. Pero el resultado es condicional: hay que llegar a él por uno de los dos métodos que prescribe la regla. Borrar los nombres y dar el trabajo por hecho es el error más frecuente en la práctica.

El primer método es la certificación por experto de § 164.514(b)(1): una persona con conocimientos y experiencia adecuados en principios y métodos estadísticos y científicos generalmente aceptados los aplica, determina que el riesgo de que un destinatario previsto identifique a una persona es muy pequeño, y documenta los métodos y los resultados del análisis. No se exige un título concreto, pero el análisis depende del destinatario — el mismo conjunto puede pasar para uno y fallar para otro — y una certificación sin documentación no cuenta.

El segundo método es el puerto seguro de § 164.514(b)(2): eliminar las 18 clases de identificadores enumeradas, para la persona y para sus familiares, empleadores y miembros del hogar, y no tener conocimiento real de que la información restante pueda identificar a alguien. Las 18 clases son: nombres; subdivisiones geográficas menores que un estado (con la regla del código postal siguiente); todos los elementos de fecha salvo el año, y las edades mayores de 89 agrupadas como 90 o más; números de teléfono; números de fax; direcciones de correo electrónico; números de Seguridad Social; números de historia clínica; números de beneficiario de plan de salud; números de cuenta; números de certificado y licencia; identificadores y números de serie de vehículos, incluidas las placas; identificadores y números de serie de dispositivos; direcciones web (URL); direcciones IP; identificadores biométricos, incluidas huellas dactilares y de voz; imágenes fotográficas de rostro completo e imágenes comparables; y cualquier otro número, característica o código único de identificación. Detalle del código postal: los tres primeros dígitos solo pueden conservarse si la población combinada del área que los comparte, según datos vigentes de la Oficina del Censo, supera las 20.000 personas; en caso contrario pasan a ser 000. Ejemplo: un área de 18.500 personas queda 20.000 menos 18.500 igual a 1.500 por debajo del umbral, así que el prefijo debe cambiarse a 000. De las fechas solo queda el año, y una persona de 92 años se registra como 90 o más, nunca como 92.

La sección 164.514(c) permite un código de reidentificación: la entidad cubierta puede asignar un código para volver a identificar los datos, siempre que el código no se derive de información sobre la persona y el mecanismo de reidentificación no se divulgue. Los datos reidentificados vuelven a ser PHI.

La sección 164.514(e) crea el carril intermedio: el conjunto de datos limitado. Retira 16 categorías de identificadores directos, pero puede conservar fechas y ciudad, estado y código postal. Sigue siendo PHI; solo puede usarse o divulgarse para investigación, salud pública u operaciones de atención de salud; y cada divulgación exige un acuerdo de uso de datos que fije los usos y usuarios permitidos, obligue al destinatario a aplicar salvaguardas, prohíba reidentificar y contactar a las personas, y exija informar de usos no permitidos. No hace falta autorización individual, pero el acuerdo es el billete: entregar un conjunto limitado sin acuerdo es una divulgación no permitida disfrazada de desidentificación.

Errores frecuentes: tratar un archivo sin nombres como desidentificado sin haber eliminado las 18 clases; tratar un conjunto limitado como si fuera dato desidentificado; conservar fechas completas en puerto seguro cuando solo puede quedar el año; obtener la opinión de un experto sin conservar la documentación que exige § 164.514(b)(1); y tratar la desidentificación como permanente cuando los cambios en otros datos del destinatario pueden socavar con el tiempo el juicio original.

Capa de California: la Ley de Confidencialidad de la Información Médica (CMIA, Código Civil, sección 56 y siguientes) restringe de forma independiente la divulgación de información médica en manos de proveedores y planes, de modo que un conjunto que supera la desidentificación de HIPAA no queda automáticamente libre para todo uso bajo la ley californiana. La Ley de Privacidad del Consumidor de California, modificada por la CPRA, exime la PHI regida por HIPAA y la CMIA e impone su propia definición de datos desidentificados. Cada capa debe comprobarse por separado.

Fuentes: 45 C.F.R. § 164.514 (texto vigente en eCFR); Oficina de Derechos Civiles del HHS, guía sobre métodos de desidentificación de PHI; Código Civil de California, secciones 56 y siguientes y 1798.100 y siguientes.

*Notas personales de estudio; no constituyen consejo médico ni jurídico. Este artículo no contiene ninguna dosis ni frecuencia de medicamentos.*

---

## 한국어 (초역 · 初译待校)

범위: 이 저장소의 HIPAA 계열(총론, 민사 벌칙과 집행, 유출 통지, 접근권과 정정권, 사망 후 기록 프라이버시) 안에서 데이터가 언제 보호 대상 건강 정보가 아니게 되는지는 전용 글이 없었습니다. 이 글은 45 C.F.R. § 164.514의 비식별화와 제한 데이터 세트를 다루며, eCFR 현행 본문과 HHS 민권국의 비식별화 방법 안내를 따릅니다. 이번 차례의 후보였던 유출 통지, 환자 접근권과 복사 수수료, 45 C.F.R. Part 180의 병원 가격 투명성은 실사 결과 모두 전용 글이 이미 있어, 비어 있던 이 절을 골랐습니다.

§ 164.514(a)의 기준은 한 문장입니다. 개인을 식별하지 않고, 개인을 식별하는 데 쓰일 수 있다고 믿을 합리적 근거가 없는 건강 정보는 개인 식별 가능 건강 정보가 아닙니다. 제대로 비식별화된 데이터는 더 이상 PHI가 아니며 사용과 공개가 HIPAA의 승인 틀을 벗어납니다. 다만 그 지위는 조건부입니다. 규칙이 정한 두 방법 중 하나로 만들어야 하며, 이름만 지우고 끝났다고 선언하는 것이 실무에서 가장 흔한 오판입니다.

첫째 방법은 § 164.514(b)(1)의 전문가 인증입니다. 일반적으로 받아들여지는 통계적·과학적 원리와 방법에 대한 적절한 지식과 경험을 갖춘 사람이 그 방법을 적용해, 예상 수신자가 단독으로 또는 다른 합리적으로 이용 가능한 정보와 결합해 개인을 식별할 위험이 매우 작다고 판단하고, 사용한 방법과 분석 결과를 문서로 남기는 방식입니다. 특정 학위나 자격은 요구되지 않지만, 분석은 수신자에 따라 달라져 같은 데이터라도 수신자가 바뀌면 결론이 뒤집힐 수 있고, 문서 없는 인증은 인정되지 않습니다.

둘째 방법은 § 164.514(b)(2)의 세이프 하버입니다. 본인과 그 친족, 고용주, 가구 구성원에 대한 열거된 18가지 식별자를 모두 제거하고, 남은 정보가 개인을 식별할 수 있다는 실제 인식이 없어야 합니다. 18가지는 다음과 같습니다: 이름; 주보다 작은 지리적 세분(아래 우편번호 규칙 포함); 연도만 남기는 날짜 요소 전체와 90세 이상으로 묶는 89세 초과 연령; 전화번호; 팩스 번호; 이메일 주소; 사회보장번호; 병력 번호; 건강보험 수혜자 번호; 계좌 번호; 증명서와 면허 번호; 차량 식별자와 일련번호(번호판 포함); 기기 식별자와 일련번호; 웹 주소(URL); IP 주소; 지문과 성문을 포함한 생체 식별자; 얼굴 전체 사진과 그에 준하는 이미지; 그 밖의 모든 고유 식별 번호, 특징, 코드입니다. 우편번호 세부 규칙: 같은 앞 세 자리를 공유하는 지역의 합산 인구가 인구조사국의 현행 공개 데이터로 20,000명을 넘을 때만 앞 세 자리를 남길 수 있고, 아니면 000으로 바꿉니다. 예시: 인구 18,500명 지역은 20,000 빼기 18,500으로 1,500명이 모자라 기준에 못 미치므로 앞자리를 000으로 바꿔야 합니다. 날짜는 연도만 남고, 92세는 92가 아니라 90세 이상으로 기록합니다.

§ 164.514(c)는 재식별 코드를 허용합니다. 대상 기관은 데이터를 다시 개인과 연결할 수 있는 코드를 부여할 수 있되, 코드가 그 개인에 관한 정보에서 도출되어서는 안 되고 재식별 방식이 외부에 알려서도 안 됩니다. 재식별된 정보는 다시 PHI가 됩니다.

§ 164.514(e)는 중간 차선인 제한 데이터 세트를 만듭니다. 직접 식별자 16범주를 제거하지만 날짜와 도시, 주, 우편번호는 남길 수 있습니다. 여전히 PHI이며, 연구, 공중보건, 의료 운영 세 목적에만 쓸 수 있고, 공개할 때마다 허용 용도와 사용자를 정하고, 수신자에게 보호 조치를 지우며, 재식별과 개인 접촉을 금지하고, 부적절한 사용의 보고를 요구하는 데이터 사용 계약이 필요합니다. 개인 승인은 필요 없지만 계약이 입장권이라, 계약 없이 제한 데이터 세트를 넘기는 것은 비식별화로 위장한 위법 공개입니다.

흔한 오류: 18가지를 다 지우지 않고 이름만 지운 파일을 비식별화로 취급하는 것, 제한 데이터 세트를 비식별 데이터처럼 다루는 것, 세이프 하버에서 연도만 남겨야 하는데 전체 날짜를 남기는 것, 전문가 의견을 받고도 § 164.514(b)(1)이 요구하는 문서를 남기지 않는 것, 수신자가 가진 외부 데이터가 바뀌면 원래 판단이 흔들릴 수 있는데 비식별화를 영구적인 것으로 여기는 것입니다.

캘리포니아 층: 의료 정보 비밀 유지법(CMIA, 민법전 제56조 이하)은 제공자와 건강보험이 가진 의료 정보의 공개를 독립적으로 제한하므로, HIPAA 비식별화를 통과한 데이터라도 캘리포니아 법에서 모든 용도가 자동으로 자유로워지지는 않습니다. CPRA로 개정된 캘리포니아 소비자 프라이버시법은 HIPAA와 CMIA가 다스리는 PHI를 면제하면서 비식별 데이터에 대한 자체 정의를 둡니다. 각 층을 따로 확인해야 합니다.

출처: 45 C.F.R. § 164.514(eCFR 현행 본문), HHS 민권국의 PHI 비식별화 방법 안내, 캘리포니아 민법전 제56조 이하와 제1798.100조 이하.

*개인 학습 노트이며 의료 조언도 법률 조언도 아닙니다. 이 글에는 약물 용량과 투여 간격이 없습니다.*

---

## Tiếng Việt (bản dịch sơ bộ · 初译待校)

Phạm vi: trong dòng HIPAA của kho này (tổng quan, phạt tiền dân sự và thực thi, thông báo vi phạm, quyền truy cập và sửa đổi, quyền riêng tư sau khi qua đời), câu hỏi khi nào dữ liệu ngừng là thông tin sức khỏe được bảo vệ chưa có bài riêng. Bài này bàn về khử định danh và tập dữ liệu giới hạn theo 45 C.F.R. § 164.514, dựa trên bản eCFR hiện hành và hướng dẫn về phương pháp khử định danh của Văn phòng Dân quyền thuộc HHS. Ba chủ đề ứng viên dự kiến cho lượt này — thông báo vi phạm, quyền truy cập của bệnh nhân và phí sao chép, minh bạch giá bệnh viện theo Phần 180 — qua kiểm tra đều đã có bài riêng, nên phần còn trống này được chọn thay thế.

Tiêu chuẩn tại § 164.514(a) gói trong một câu: thông tin sức khỏe không định danh một cá nhân, và không có cơ sở hợp lý để tin rằng nó có thể được dùng để định danh cá nhân đó, thì không phải là thông tin sức khỏe có thể định danh cá nhân. Dữ liệu đã khử định danh đúng cách không còn là PHI, và việc sử dụng, tiết lộ nó rời khỏi khung ủy quyền của HIPAA. Nhưng trạng thái này có điều kiện: phải đạt được bằng một trong hai phương pháp mà quy tắc quy định. Xóa tên rồi tuyên bố xong việc là sai lầm phổ biến nhất trong thực tế.

Phương pháp một là chứng nhận của chuyên gia theo § 164.514(b)(1): một người có kiến thức và kinh nghiệm phù hợp về các nguyên tắc và phương pháp thống kê, khoa học được chấp nhận chung sẽ áp dụng các phương pháp đó, xác định rằng nguy cơ thông tin bị người nhận dự kiến dùng, riêng lẻ hoặc kết hợp với thông tin sẵn có hợp lý khác, để định danh một cá nhân là rất nhỏ, đồng thời ghi lại phương pháp và kết quả phân tích thành tài liệu. Không yêu cầu bằng cấp cụ thể nào, nhưng phân tích phụ thuộc vào người nhận — cùng một tập dữ liệu có thể đạt với người nhận này và không đạt với người nhận khác — và chứng nhận không có tài liệu thì không tính.

Phương pháp hai là bến an toàn (Safe Harbor) theo § 164.514(b)(2): loại bỏ toàn bộ 18 loại định danh được liệt kê, đối với cá nhân và đối với thân nhân, người sử dụng lao động và thành viên hộ gia đình của họ, đồng thời không có kiến thức thực tế rằng thông tin còn lại có thể định danh ai đó. Mười tám loại là: họ tên; phân vùng địa lý nhỏ hơn bang (kèm quy tắc mã ZIP dưới đây); mọi yếu tố ngày tháng trừ năm, cùng các độ tuổi trên 89 được gộp thành 90 trở lên; số điện thoại; số fax; địa chỉ email; số An sinh Xã hội; số hồ sơ bệnh án; số người thụ hưởng chương trình sức khỏe; số tài khoản; số chứng chỉ và giấy phép; định danh và số sê-ri của phương tiện, kể cả biển số; định danh và số sê-ri của thiết bị; địa chỉ web (URL); địa chỉ IP; định danh sinh trắc, gồm dấu vân tay và giọng nói; ảnh chụp toàn mặt và hình ảnh tương đương; và mọi số, đặc điểm hay mã định danh duy nhất khác. Chi tiết mã ZIP: ba chữ số đầu chỉ được giữ khi tổng dân số của khu vực dùng chung ba chữ số đó, theo dữ liệu hiện hành của Cục Điều tra Dân số, vượt 20.000 người; nếu không, chúng trở thành 000. Ví dụ: một khu vực 18.500 người thiếu 20.000 trừ 18.500 bằng 1.500 so với ngưỡng, nên tiền tố phải đổi thành 000. Ngày tháng chỉ giữ lại năm, và người 92 tuổi được ghi là 90 trở lên, không bao giờ ghi 92.

Điều 164.514(c) cho phép mã tái định danh: tổ chức được bảo phủ có thể gán một mã để sau này nối lại dữ liệu với cá nhân, với điều kiện mã không được suy ra từ thông tin về cá nhân đó và cơ chế tái định danh không được tiết lộ. Dữ liệu đã tái định danh lại là PHI.

Điều 164.514(e) tạo làn giữa: tập dữ liệu giới hạn. Nó loại bỏ 16 nhóm định danh trực tiếp nhưng có thể giữ ngày tháng và thành phố, bang, mã ZIP. Nó vẫn là PHI; chỉ được dùng hoặc tiết lộ cho nghiên cứu, y tế công cộng hoặc vận hành chăm sóc sức khỏe; và mỗi lần tiết lộ đều cần một thỏa thuận sử dụng dữ liệu quy định mục đích và người dùng được phép, buộc người nhận áp dụng biện pháp bảo vệ, cấm tái định danh và cấm liên hệ với cá nhân, đồng thời yêu cầu báo cáo việc dùng sai. Không cần ủy quyền của từng cá nhân, nhưng thỏa thuận là tấm vé — giao tập dữ liệu giới hạn mà không có thỏa thuận là một lần tiết lộ không được phép đội lốt khử định danh.

Các lỗi thường gặp: coi một tệp đã xóa tên là đã khử định danh khi chưa loại đủ 18 loại; coi tập dữ liệu giới hạn như dữ liệu đã khử định danh; giữ nguyên ngày tháng đầy đủ trong bến an toàn khi chỉ năm được ở lại; xin ý kiến chuyên gia mà không lưu tài liệu mà § 164.514(b)(1) yêu cầu; và coi khử định danh là vĩnh viễn trong khi những thay đổi trong các dữ liệu khác mà người nhận nắm giữ có thể làm suy yếu phán đoán ban đầu theo thời gian.

Lớp California: Đạo luật Bảo mật Thông tin Y tế (CMIA, Bộ luật Dân sự điều 56 trở đi) độc lập hạn chế việc tiết lộ thông tin y tế do nhà cung cấp và chương trình sức khỏe nắm giữ, nên một tập dữ liệu qua được khử định danh HIPAA không tự động tự do cho mọi mục đích theo luật California. Đạo luật Quyền riêng tư Người tiêu dùng California, sửa đổi bởi CPRA, miễn trừ PHI chịu sự điều chỉnh của HIPAA và CMIA đồng thời đặt ra định nghĩa riêng về dữ liệu đã khử định danh. Mỗi lớp phải được kiểm tra riêng.

Nguồn: 45 C.F.R. § 164.514 (bản eCFR hiện hành); Văn phòng Dân quyền HHS, hướng dẫn về phương pháp khử định danh PHI; Bộ luật Dân sự California các điều 56 trở đi và 1798.100 trở đi.

*Ghi chép học tập cá nhân, không phải tư vấn y tế cũng không phải tư vấn pháp lý. Bài này không chứa liều lượng hay tần suất thuốc nào.*

---

## हिन्दी (प्रारंभिक अनुवाद · 初译待校)

दायरा: इस भंडार की HIPAA श्रृंखला (अवलोकन, दीवानी आर्थिक दंड और प्रवर्तन, उल्लंघन अधिसूचना, पहुँच और संशोधन अधिकार, मृत्यु के पश्चात निजता) में यह प्रश्न कि डेटा कब संरक्षित स्वास्थ्य सूचना होना बंद कर देता है, अब तक बिना समर्पित लेख के था। यह लेख 45 C.F.R. § 164.514 के अंतर्गत अ-पहचानीकरण और सीमित डेटा समुच्चयों को लेता है, वर्तमान eCFR पाठ और HHS नागरिक अधिकार कार्यालय के अ-पहचानीकरण विधियों के मार्गदर्शन के अनुसार। इस बारी के तीन प्रत्याशी विषय — उल्लंघन अधिसूचना, रोगी पहुँच अधिकार और प्रतिलिपि शुल्क, तथा भाग 180 के अंतर्गत अस्पताल मूल्य पारदर्शिता — जाँच पर पाया गया कि तीनों पर पहले से समर्पित लेख हैं, इसलिए यह खाली खंड चुना गया।

§ 164.514(a) का मानक एक वाक्य में है: जो स्वास्थ्य सूचना किसी व्यक्ति की पहचान नहीं करती और जिसके बारे में यह मानने का कोई युक्तिसंगत आधार नहीं है कि उससे किसी व्यक्ति की पहचान हो सकती है, वह व्यक्तिगत रूप से पहचान योग्य स्वास्थ्य सूचना नहीं है। ठीक से अ-पहचानीकृत डेटा इसलिए PHI नहीं रहता और उसका उपयोग व प्रकटीकरण HIPAA के प्राधिकरण ढाँचे से बाहर चला जाता है। परंतु यह स्थिति सशर्त है: अ-पहचानीकरण नियम द्वारा निर्धारित दो विधियों में से किसी एक से प्राप्त होना चाहिए। नाम हटाकर काम पूरा घोषित करना व्यवहार में सबसे आम भूल है।

विधि एक है § 164.514(b)(1) के अंतर्गत विशेषज्ञ प्रमाणन: सामान्यतः स्वीकृत सांख्यिकीय और वैज्ञानिक सिद्धांतों व विधियों का उपयुक्त ज्ञान और अनुभव रखने वाला व्यक्ति उन विधियों को लागू करता है, यह निर्धारित करता है कि अपेक्षित प्राप्तकर्ता द्वारा सूचना को अकेले या अन्य युक्तिसंगत रूप से उपलब्ध सूचना के साथ मिलाकर किसी व्यक्ति की पहचान करने का जोखिम बहुत छोटा है, और विधियों तथा विश्लेषण के परिणामों का दस्तावेज़ीकरण करता है। किसी विशेष डिग्री या प्रमाणपत्र की आवश्यकता नहीं है, परंतु विश्लेषण प्राप्तकर्ता-विशिष्ट होता है — वही डेटा समुच्चय एक प्राप्तकर्ता के लिए उत्तीर्ण और दूसरे के लिए अनुत्तीर्ण हो सकता है — और बिना दस्तावेज़ वाला प्रमाणन गिना नहीं जाता।

विधि दो है § 164.514(b)(2) के अंतर्गत सुरक्षित बंदरगाह (Safe Harbor): व्यक्ति के लिए तथा उसके संबंधियों, नियोक्ताओं और घर के सदस्यों के लिए सूचीबद्ध 18 प्रकार के पहचानकर्ता हटाए जाएँ, और शेष सूचना से किसी की पहचान हो सकती है, इसका वास्तविक ज्ञान न हो। अठारह प्रकार हैं: नाम; राज्य से छोटी भौगोलिक उप-इकाइयाँ (नीचे दिए ZIP नियम सहित); वर्ष को छोड़कर सभी तिथि तत्व, तथा 89 से अधिक आयु को 90 या अधिक में समूहित करना; टेलीफ़ोन नंबर; फ़ैक्स नंबर; ईमेल पते; सामाजिक सुरक्षा नंबर; चिकित्सा अभिलेख नंबर; स्वास्थ्य योजना लाभार्थी नंबर; खाता नंबर; प्रमाणपत्र और लाइसेंस नंबर; वाहन पहचानकर्ता और क्रम संख्याएँ, लाइसेंस प्लेट सहित; यंत्र पहचानकर्ता और क्रम संख्याएँ; वेब URL; IP पते; जैवमितीय पहचानकर्ता, अँगुलि-छाप और स्वर-छाप सहित; पूरे चेहरे की तस्वीरें और तुलनीय छवियाँ; और कोई अन्य अद्वितीय पहचान संख्या, विशेषता या कोड। ZIP विवरण: पहले तीन अंक तभी रखे जा सकते हैं जब उन्हें साझा करने वाले क्षेत्र की संयुक्त जनसंख्या, जनगणना ब्यूरो के वर्तमान डेटा के अनुसार, 20,000 से अधिक हो; अन्यथा वे 000 हो जाते हैं। उदाहरण: 18,500 लोगों का क्षेत्र 20,000 ऋण 18,500 बराबर 1,500 से सीमा से नीचे है, इसलिए उपसर्ग 000 करना होगा। तिथियों में केवल वर्ष रहता है, और 92 वर्ष के व्यक्ति को 92 नहीं, 90 या अधिक लिखा जाता है।

धारा 164.514(c) पुनः-पहचान कोड की अनुमति देती है: आवृत इकाई एक कोड दे सकती है जिससे वह डेटा को फिर व्यक्ति से जोड़ सके, बशर्ते कोड उस व्यक्ति के बारे में सूचना से व्युत्पन्न न हो और पुनः-पहचान की प्रक्रिया प्रकट न की जाए। इस प्रकार पुनः पहचाना गया डेटा फिर PHI बन जाता है।

धारा 164.514(e) बीच की गली बनाती है: सीमित डेटा समुच्चय। यह प्रत्यक्ष पहचानकर्ताओं की 16 श्रेणियाँ हटाता है, परंतु तिथियाँ और शहर, राज्य व ZIP रख सकता है। यह PHI बना रहता है; इसका उपयोग या प्रकटीकरण केवल अनुसंधान, लोक स्वास्थ्य या स्वास्थ्य-देखभाल संचालन के लिए हो सकता है; और हर प्रकटीकरण हेतु डेटा उपयोग समझौता चाहिए जो अनुमत उपयोग और उपयोगकर्ता तय करे, प्राप्तकर्ता को सुरक्षा उपायों से बाँधे, पुनः-पहचान और व्यक्तियों से संपर्क पर रोक लगाए, और अननुमत उपयोगों की सूचना माँगे। व्यक्तिगत प्राधिकरण आवश्यक नहीं, परंतु समझौता ही टिकट है — बिना समझौते सीमित डेटा समुच्चय सौंपना अ-पहचानीकरण के भेस में अननुमत प्रकटीकरण है।

आम भूलें: 18 प्रकार पूरी तरह हटाए बिना नाम-रहित फ़ाइल को अ-पहचानीकृत मानना; सीमित डेटा समुच्चय को अ-पहचानीकृत डेटा समझना; सुरक्षित बंदरगाह में केवल वर्ष रहने की जगह पूरी तिथियाँ रखना; विशेषज्ञ की राय लेकर § 164.514(b)(1) द्वारा अपेक्षित दस्तावेज़ न रखना; और अ-पहचानीकरण को स्थायी मानना, जबकि प्राप्तकर्ता के पास मौजूद अन्य डेटा में बदलाव समय के साथ मूल निर्णय को कमज़ोर कर सकता है।

कैलिफ़ोर्निया परत: चिकित्सा सूचना गोपनीयता अधिनियम (CMIA, दीवानी संहिता धारा 56 व आगे) प्रदाताओं और योजनाओं के पास मौजूद चिकित्सा सूचना के प्रकटीकरण को स्वतंत्र रूप से सीमित करता है, इसलिए HIPAA अ-पहचानीकरण पार करने वाला डेटा समुच्चय कैलिफ़ोर्निया विधि में हर उपयोग हेतु स्वतः मुक्त नहीं हो जाता। CPRA द्वारा संशोधित कैलिफ़ोर्निया उपभोक्ता निजता अधिनियम HIPAA और CMIA द्वारा शासित PHI को छूट देता है और अ-पहचानीकृत डेटा की अपनी परिभाषा रखता है। प्रत्येक परत अलग से जाँचनी चाहिए।

स्रोत: 45 C.F.R. § 164.514 (eCFR वर्तमान पाठ); HHS नागरिक अधिकार कार्यालय, PHI के अ-पहचानीकरण की विधियों पर मार्गदर्शन; कैलिफ़ोर्निया दीवानी संहिता धारा 56 व आगे और 1798.100 व आगे।

*केवल व्यक्तिगत अध्ययन-टिप्पणी; चिकित्सा सलाह नहीं और कानूनी सलाह भी नहीं। इस लेख में कोई औषधि-खुराक या आवृत्ति नहीं है।*
