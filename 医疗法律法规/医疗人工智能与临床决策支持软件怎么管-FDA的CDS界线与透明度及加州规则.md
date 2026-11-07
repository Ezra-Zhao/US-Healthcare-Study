# 医疗人工智能与临床决策支持软件怎么管：FDA 的 CDS 界线、透明度与加州规则

> 个人学习笔记，不构成医疗建议，也不构成法律意见。本篇讲的是医疗人工智能与临床决策支持（CDS）软件在美国的监管界线：哪些软件被法律排除在器械定义之外、哪些仍要走 FDA 上市路径、认证健康 IT 的算法透明度要求，以及加州对生成式 AI 患者沟通的规则。条号不确定处只写法律名与年份，不写死；具体产品的定性以 FDA 与州监管机构的现行文本为准。全文不涉及任何药物用量。出现紧急情况请拨打 911。

## 中文主文

### 一、总界线：软件先分「器械」与「非器械」两边

美国对医疗软件的第一刀，切在《联邦食品、药品和化妆品法》（FD&C Act）的器械（device）定义上。2016 年《21 世纪治愈法》（21st Century Cures Act）第 3060 条在 FD&C Act 中加入第 520(o) 条，把若干类软件功能明确排除在 device 定义之外，其中与临床最相关的一类就是满足条件的临床决策支持软件。落在排除侧的软件，不按医疗器械走 FDA 上市审查；落在器械侧的软件，则按风险走既有的器械路径。医疗 AI 产品的名字叫什么不重要，重要的是它的功能、对象和输出方式落在哪一边。

### 二、排除侧的四项判据：§ 520(o) 怎么划 CDS 这条线

按 FD&C Act § 520(o) 的结构与 FDA 于 2022 年发布的《Clinical Decision Support Software》最终指南的解释，一项 CDS 功能要落在非器械一侧，大体要同时满足四项判据：

1. 不处理医学影像、体外诊断信号或生理信号模式本身——它的输入是临床信息与知识，而不是对影像或信号做采集与分析判断；
2. 功能是展示、分析或打印医疗信息，或支持、提供关于预防、诊断、治疗的建议，其形态是把依据与选项摆出来；
3. 面向的是医疗专业人员（health care professional），而不是直接面向患者或照护者下结论；
4. 设计上要让医护人员能够独立审查建议的依据——软件应当交代它依赖的信息、逻辑或来源，使医护人员不是主要依赖软件的输出来做临床决定，而是自己看过依据后判断。

四项里第四项是实务中最常卡住的一条：如果软件只给出一个确定性结论，却不展示依据，医护人员无从独立审查，它在功能上就更像在代替判断，而不是支持判断。FDA 2022 年指南还强调了时间紧迫场景的考量：在分秒必争的场合，医护人员客观上没有条件逐条复核依据，这类输出更容易被当作指令使用，监管定性时会被更严格地看待。指南是 FDA 的解释口径，不改变法条本身；个案定性最终看产品实际功能、预期用途与宣传表述的组合。

### 三、器械侧的路径：510(k)、De Novo、PMA 与 SaMD 框架

落在器械侧的软件，按风险与是否有先例走三条常见路径：与已上市器械实质等同的，走 510(k) 上市前通知；没有合适先例、但风险属低到中等的，走 De Novo 分类路径，获批的同时立起一个新的器械类型；风险最高的，走 PMA 上市前批准，证据要求也最重。分析框架上，国际医疗器械监管者论坛（IMDRF）的 SaMD（Software as a Medical Device）思路是理解这一领域的通用语言：按软件提供的信息对临床决策的重要程度、以及所针对病情的严重程度，给软件分层定级，FDA 的风险分类与审查强度与这一思路大体呼应。给影像下判断的 AI、直接驱动治疗决策的软件，多落在这一侧。

### 四、AI 器械的特殊问题：会「变」的软件与 PCCP

传统器械审查假设产品上市后基本不变，但机器学习软件的卖点恰恰是持续学习与迭代。为这个矛盾准备的工具是预定变更控制计划（Predetermined Change Control Plan, PCCP）：厂商在上市申请时就把将来打算怎么改算法、改动范围到哪里、用什么方法验证改动后的性能，先写成计划随申请一并提交审查；将来在已获批计划范围内的改动，可以按计划实施并留档，而不必每改一版都重新走一遍完整申请。PCCP 不是免审通行证：计划外的改动、超出预定范围的性能变化，仍然要重新与 FDA 打交道。采购方评估 AI 产品时，可以直接问一句：这家厂商有没有 PCCP、覆盖哪些改动——答案能看出对方对持续合规的准备程度。

### 五、透明度线：ONC HTI-1 对决策支持干预的要求

第二条监管线不在 FDA，而在健康 IT 认证体系。联邦卫生 IT 协调办公室（ONC）的 HTI-1 规则在认证标准中加入了「决策支持干预」（decision support interventions）条款（45 C.F.R. § 170.315(b)(11)）：使用认证健康 IT 提供的预测性决策支持时，系统要公开一组算法来源属性，例如干预的名称与开发方、预期用途、开发所用数据的性质、已知的局限与公平性相关考量、以及外部验证情况等，让使用机构能查、能比、能追问。它的逻辑与 FDA 不同：不先问算不算器械，而是先要求黑箱把盖子打开一条缝。医院做采购与上线评审时，这组属性是现成的审查清单。

### 六、数据线：HIPAA 管谁，PHI 与去标识化的边界在哪

医疗 AI 离不开患者数据，但 HIPAA 的适用面比很多人想的窄：它只约束受保主体（covered entity）及其业务伙伴（business associate）经手的受保护健康信息（PHI）。医院部署的 AI 工具处理病历数据，工具厂商通常以业务伙伴身份被 HIPAA 约束，要签业务伙伴协议、落实安全保障；反过来，消费者自己下载、自己输入数据的健康应用，若运营方既不是受保主体也不是业务伙伴，用户数据就不在 HIPAA 管辖内，可能改受 FTC 规则与州隐私法约束。用患者数据训练或验证算法时，常见的合规出口是去标识化（de-identification）：按 HIPAA 的方法去掉规定的标识符、或经专家认证判定再识别风险极低之后，数据不再算 PHI，使用限制随之松动。但去标识化不是把姓名删掉就算数，方法不对，数据在法律上仍是 PHI，这是实务中最常见的误判之一。

### 七、加州规则：AB 3030 的免责声明与 AI 利用审查的监管动向

州层面以加州动作最明确。加州 AB 3030（2024）要求：医疗机构使用生成式 AI 制作涉及患者临床信息的沟通内容时，要附上免责声明，表明内容由生成式 AI 生成，并为患者保留联系真人的通道。该法的着眼点是沟通知情——患者有权知道对面这段话是机器写的还是医护写的。具体条号与执行细则以加州现行法典文本为准，本篇只引用法案名与年份。另一个动向是利用审查（utilization review）环节的 AI：健康计划用算法参与事先授权与医疗必要性审查，近年成为联邦与各州共同的监管议题，加州亦有相应的立法与监管讨论，口径仍在演进，涉及这类系统的机构应以现行法与监管机构当期指引为准，不宜按旧闻行事。

### 八、把几条线合起来：一份简易核对顺序

面对一款医疗 AI 或 CDS 产品，可以依次问五个问题：一，它是否满足 § 520(o) 的四项判据（尤其第四项：医护能否独立审查依据），还是应当按器械走 510(k)、De Novo 或 PMA；二，如果是会持续迭代的 AI 器械，有没有 PCCP、计划覆盖到哪一步；三，它若嵌在认证健康 IT 里，HTI-1 要求的来源属性是否公开齐全；四，数据经手方是不是 HIPAA 的受保主体或业务伙伴、训练数据是否真正完成了去标识化；五，若在加州用生成式 AI 直接与患者沟通临床信息，AB 3030 的免责声明与真人通道是否落实。五问过完，产品的监管轮廓大致就清楚了。

*本文为个人学习笔记，不构成医疗建议，也不构成法律意见。主要来源：FD&C Act § 520(o)（由 21st Century Cures Act § 3060 加入）；FDA《Clinical Decision Support Software》最终指南（2022 年）；ONC HTI-1 规则与 45 C.F.R. § 170.315(b)(11)；HIPAA 隐私与安全规则关于受保主体、业务伙伴与去标识化的口径；加州 AB 3030 (2024)。具体条文以各机构现行发布为准。*

## English

> Personal study notes, not medical advice and not legal advice. In an emergency, call 911. This article maps the U.S. regulatory lines for medical AI and clinical decision support (CDS) software. It discusses no drug amounts.

**The statutory line.** Section 3060 of the 21st Century Cures Act added Section 520(o) to the FD&C Act, excluding certain software functions from the definition of a device. For CDS, FDA's September 2022 final guidance, *Clinical Decision Support Software*, reads the exclusion around four criteria: the software does not acquire, process, or analyze a medical image, an in vitro diagnostic signal, or a physiological signal pattern; it displays, analyzes, or prints medical information or provides supporting recommendations about prevention, diagnosis, or treatment; it is intended for health care professionals rather than giving conclusions directly to patients or caregivers; and it is designed so that the professional can independently review the basis for its recommendations — the software discloses the information, logic, or sources it relies on, so the clinician judges the basis instead of primarily relying on the output. Software that outputs a single definitive answer with no reviewable basis, or that is meant for time-critical decisions where review is unrealistic, tends to fall on the device side.

**Device pathways and changing algorithms.** Software on the device side follows the familiar routes: 510(k) premarket notification where a predicate exists, the De Novo pathway for novel low-to-moderate-risk types, and PMA for the highest-risk products. The IMDRF's SaMD (Software as a Medical Device) framework — grading software by the significance of the information it provides and the seriousness of the condition — is the common vocabulary behind this risk layering. For learning systems, the Predetermined Change Control Plan (PCCP) is the key tool: the manufacturer submits, up front, what algorithm changes it anticipates, how far they may go, and how each change will be validated; changes inside an authorized plan can then be made under the plan instead of a fresh full submission each time, while changes outside the plan still require FDA engagement.

**Transparency and data.** ONC's HTI-1 rule, at 45 C.F.R. § 170.315(b)(11), requires certified health IT to disclose source attributes for predictive decision support interventions — developer, intended use, the nature of development data, known limitations and fairness considerations, and validation — whether or not the tool is a device. HIPAA reaches only covered entities and their business associates handling protected health information; de-identified data, removed under HIPAA's specified methods or certified by an expert, is no longer PHI, but deleting names alone does not de-identify. In California, AB 3030 (2024) requires a disclaimer and a human contact route when generative AI produces clinical communications to patients, and AI in utilization review remains an evolving area of state and federal oversight — check current law before relying on any summary.

## Español (traducción de estudio)

> Notas personales de estudio; no constituyen asesoría médica ni legal. En una emergencia, llame al 911. Este artículo traza las líneas regulatorias estadounidenses para la IA médica y el software de apoyo a la decisión clínica (CDS). No menciona cantidades de medicamentos.

**La línea legal.** La Sección 3060 de la Ley de Curas del Siglo XXI añadió la Sección 520(o) a la FD&C Act, excluyendo ciertas funciones de software de la definición de dispositivo. Para el CDS, la guía final de la FDA de septiembre de 2022, *Clinical Decision Support Software*, ordena la exclusión en torno a cuatro criterios: el software no adquiere, procesa ni analiza una imagen médica, una señal de diagnóstico in vitro ni un patrón de señal fisiológica; muestra, analiza o imprime información médica, o aporta recomendaciones de apoyo sobre prevención, diagnóstico o tratamiento; está destinado a profesionales de la salud y no a dar conclusiones directas a pacientes o cuidadores; y está diseñado para que el profesional pueda revisar de forma independiente la base de sus recomendaciones — el software revela la información, la lógica o las fuentes que usa, de modo que el clínico juzga la base en lugar de depender principalmente del resultado. El software que ofrece una única respuesta definitiva sin base revisable, o pensado para decisiones urgentes donde la revisión no es realista, tiende a caer del lado del dispositivo.

**Vías de dispositivo y algoritmos cambiantes.** El software del lado del dispositivo sigue las rutas conocidas: notificación previa 510(k) cuando existe un precedente, la vía De Novo para tipos nuevos de riesgo bajo a moderado, y PMA para los productos de mayor riesgo. El marco SaMD (software como dispositivo médico) del IMDRF — que gradúa el software según la importancia de la información que aporta y la gravedad de la condición — es el vocabulario común de esta clasificación por riesgo. Para sistemas que aprenden, la herramienta clave es el Plan de Control de Cambios Predeterminado (PCCP): el fabricante presenta por anticipado qué cambios del algoritmo prevé, hasta dónde pueden llegar y cómo se validará cada uno; los cambios dentro de un plan autorizado pueden hacerse bajo ese plan en vez de una nueva presentación completa cada vez, mientras que los cambios fuera del plan siguen requiriendo trato con la FDA.

**Transparencia y datos.** La norma HTI-1 de la ONC, en 45 C.F.R. § 170.315(b)(11), exige que la IT de salud certificada revele los atributos de origen de las intervenciones predictivas de apoyo a la decisión — desarrollador, uso previsto, naturaleza de los datos de desarrollo, limitaciones conocidas y consideraciones de equidad, y validación — sea o no el producto un dispositivo. HIPAA solo alcanza a las entidades cubiertas y sus socios comerciales que manejan información de salud protegida; los datos desidentificados según los métodos que fija HIPAA, o certificados por un experto, ya no son PHI, pero borrar nombres por sí solo no desidentifica. En California, AB 3030 (2024) exige un aviso y una vía de contacto con una persona real cuando la IA generativa produce comunicaciones clínicas a pacientes, y el uso de IA en la revisión de utilización sigue siendo un ámbito en evolución de la supervisión estatal y federal: consulte la ley vigente antes de fiarse de cualquier resumen.

## 한국어 (초역, 원어민 감수 대기)

> 개인 학습 노트이며 의료·법률 자문이 아닙니다. 응급 시 911에 전화하십시오. 이 글은 의료 AI와 임상 의사결정 지원(CDS) 소프트웨어에 대한 미국의 규제 경계를 정리하며, 약물 용량은 다루지 않습니다.

**법정 경계.** 21세기 치유법 제3060조는 FD&C Act에 제520(o)조를 더해 일부 소프트웨어 기능을 기기 정의에서 제외했습니다. CDS에 대해 FDA의 2022년 9월 최종 지침 *Clinical Decision Support Software*는 제외를 네 가지 기준을 중심으로 읽습니다. 소프트웨어가 의료 영상, 체외진단 신호, 생리 신호 패턴 자체를 취득·처리·분석하지 않을 것; 의료 정보를 표시·분석·출력하거나 예방·진단·치료에 대한 지원적 권고를 제공할 것; 환자나 돌봄 제공자에게 직접 결론을 내리는 것이 아니라 의료 전문가를 대상으로 할 것; 그리고 전문가가 권고의 근거를 독립적으로 검토할 수 있도록 설계될 것 — 소프트웨어가 의존하는 정보와 논리, 출처를 밝혀 임상의가 출력에 주로 의존하지 않고 근거를 보고 판단하게 하는 것입니다. 검토할 근거 없이 하나의 확정 결론만 내는 소프트웨어나, 검토가 현실적으로 어려운 시간 긴박 상황에서 쓰이는 소프트웨어는 기기 쪽으로 기우는 경향이 있습니다.

**기기 경로와 변하는 알고리즘.** 기기 쪽 소프트웨어는 익숙한 경로를 따릅니다. 선행 제품이 있으면 510(k) 시판 전 신고, 새롭고 위험이 낮거나 중간인 유형은 De Novo 경로, 최고 위험 제품은 PMA입니다. IMDRF의 SaMD(의료기기로서의 소프트웨어) 틀 — 제공하는 정보의 중요성과 대상 질환의 심각성으로 소프트웨어를 등급화하는 방식 — 이 이 위험 계층화의 공통 언어입니다. 학습하는 시스템에서는 사전 결정 변경 관리 계획(PCCP)이 핵심 도구입니다. 제조사가 알고리즘을 어떻게, 어디까지 바꿀 계획인지와 각 변경을 어떻게 검증할지를 처음 신청에 미리 제출하고, 승인된 계획 안의 변경은 매번 새 전체 신청 없이 계획대로 실시할 수 있으며, 계획 밖의 변경은 여전히 FDA와의 절차가 필요합니다.

**투명성과 데이터.** ONC의 HTI-1 규칙 45 C.F.R. § 170.315(b)(11)은 인증 건강 IT가 예측형 의사결정 지원 개입의 출처 속성 — 개발 주체, 의도된 용도, 개발 데이터의 성격, 알려진 한계와 공정성 고려, 검증 현황 — 을 기기 해당 여부와 무관하게 공개하도록 요구합니다. HIPAA는 보호 대상 건강 정보를 다루는 적용 대상 기관과 그 업무 제휴자에게만 미칩니다. HIPAA가 정한 방법으로 비식별화되거나 전문가 인증을 받은 데이터는 더 이상 PHI가 아니지만, 이름만 지우는 것으로는 비식별화가 되지 않습니다. 캘리포니아에서는 AB 3030 (2024)이 생성형 AI가 환자에게 임상 커뮤니케이션을 만들 때 고지와 실제 담당자에게 닿을 경로를 요구하고, 이용 심사에 쓰이는 AI는 주와 연방 감독이 계속 움직이는 영역이므로 어떤 요약도 현행법을 확인한 뒤에 신뢰해야 합니다.

보충하면, 투명성 축은 FDA가 아니라 ONC의 건강 IT 인증 체계에도 있다. HTI-1 규칙이 신설한 decision support interventions 기준(45 C.F.R. § 170.315(b)(11))은 인증 건강 IT가 제공하는 예측형 결정 지원에 대해 개입의 이름과 개발자, 의도된 용도, 개발 데이터의 성격, 알려진 한계와 공정성 고려, 외부 검증 여부 같은 출처 속성을 공개하도록 요구한다. 또 기계학습 소프트웨어의 변경 문제에는 사전결정 변경관리계획(PCCP)이 답으로 준비되어 있다. 제조사가 신청 단계에서 알고리즘을 어떻게, 어디까지 바꿀지와 변경 후 성능 검증 방법을 계획으로 제출해 승인을 받아 두면, 계획 범위 안의 변경은 매번 전체 신청을 다시 하지 않고 계획대로 실시하고 기록할 수 있다. 계획 밖 변경은 여전히 FDA와 새로 상대해야 한다.
## Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

> Ghi chú học tập cá nhân, không phải tư vấn y tế hay pháp lý. Trường hợp khẩn cấp, hãy gọi 911. Bài này vạch các ranh giới quản lý của Hoa Kỳ đối với AI y tế và phần mềm hỗ trợ quyết định lâm sàng (CDS), và không đề cập lượng thuốc nào.

**Ranh giới luật định.** Mục 3060 của Đạo luật Chữa trị Thế kỷ 21 đã bổ sung Mục 520(o) vào FD&C Act, loại trừ một số chức năng phần mềm khỏi định nghĩa thiết bị. Với CDS, hướng dẫn cuối cùng tháng 9 năm 2022 của FDA, *Clinical Decision Support Software*, đọc điều khoản loại trừ quanh bốn tiêu chí: phần mềm không thu thập, xử lý hay phân tích hình ảnh y tế, tín hiệu chẩn đoán in vitro hay mẫu tín hiệu sinh lý; nó hiển thị, phân tích hoặc in thông tin y tế, hoặc đưa ra khuyến nghị hỗ trợ về phòng ngừa, chẩn đoán, điều trị; nó hướng tới chuyên gia y tế chứ không đưa kết luận trực tiếp cho bệnh nhân hay người chăm sóc; và nó được thiết kế để chuyên gia có thể độc lập xem xét cơ sở của khuyến nghị — phần mềm công khai thông tin, lôgic hay nguồn mà nó dựa vào, để bác sĩ phán đoán trên cơ sở đó thay vì chủ yếu dựa vào kết quả đầu ra. Phần mềm chỉ đưa một đáp án dứt khoát duy nhất mà không có cơ sở để kiểm chứng, hoặc dùng cho quyết định gấp về thời gian nơi việc xem lại không thực tế, có xu hướng rơi về phía thiết bị.

**Lộ trình thiết bị và thuật toán thay đổi.** Phần mềm ở phía thiết bị đi theo các lộ trình quen thuộc: thông báo tiền thị trường 510(k) khi có tiền lệ, lộ trình De Novo cho loại hình mới có rủi ro thấp tới trung bình, và PMA cho sản phẩm rủi ro cao nhất. Khung SaMD (phần mềm như thiết bị y tế) của IMDRF — xếp hạng phần mềm theo mức quan trọng của thông tin nó cung cấp và mức nghiêm trọng của bệnh trạng — là ngôn ngữ chung của cách phân tầng rủi ro này. Với hệ thống có khả năng học, công cụ then chốt là Kế hoạch Kiểm soát Thay đổi Định trước (PCCP): nhà sản xuất nộp ngay từ đầu việc mình dự kiến thay đổi thuật toán ra sao, tới mức nào, và mỗi thay đổi sẽ được thẩm định thế nào; thay đổi nằm trong kế hoạch đã được chấp thuận có thể thực hiện theo kế hoạch thay vì nộp lại toàn bộ hồ sơ mỗi lần, còn thay đổi ngoài kế hoạch vẫn phải làm việc với FDA.

**Minh bạch và dữ liệu.** Quy tắc HTI-1 của ONC, tại 45 C.F.R. § 170.315(b)(11), yêu cầu công nghệ thông tin y tế được chứng nhận phải công bố thuộc tính nguồn của các can thiệp hỗ trợ quyết định mang tính dự đoán — bên phát triển, mục đích sử dụng, tính chất của dữ liệu phát triển, các giới hạn đã biết và cân nhắc về công bằng, cùng việc thẩm định — bất kể công cụ đó có phải là thiết bị hay không. HIPAA chỉ chạm tới các thực thể thuộc diện điều chỉnh và đối tác kinh doanh của chúng khi xử lý thông tin sức khỏe được bảo vệ; dữ liệu đã khử định danh theo các phương pháp HIPAA quy định hoặc được chuyên gia chứng nhận thì không còn là PHI, nhưng chỉ xóa tên thôi thì chưa khử định danh. Tại California, AB 3030 (2024) yêu cầu tuyên bố miễn trừ và một kênh liên hệ với người thật khi AI tạo sinh soạn nội dung giao tiếp lâm sàng gửi bệnh nhân, và AI trong khâu thẩm định sử dụng dịch vụ (utilization review) vẫn là lĩnh vực giám sát đang biến động ở cấp bang và liên bang — hãy kiểm tra luật hiện hành trước khi tin vào bất kỳ bản tóm tắt nào.

Bổ sung: trục minh bạch không chỉ nằm ở FDA mà còn ở hệ thống chứng nhận health IT của ONC. Tiêu chuẩn decision support interventions do quy tắc HTI-1 bổ sung (45 C.F.R. § 170.315(b)(11)) yêu cầu, đối với hỗ trợ quyết định dự đoán do health IT được chứng nhận cung cấp, phải công bố một bộ thuộc tính nguồn gốc thuật toán như tên và nhà phát triển của can thiệp, mục đích dự kiến, bản chất dữ liệu phát triển, các giới hạn đã biết và cân nhắc công bằng, cùng tình trạng kiểm chứng bên ngoài. Với bài toán phần mềm học máy liên tục thay đổi, công cụ tương ứng là kế hoạch kiểm soát thay đổi định trước (PCCP): nhà sản xuất nộp kèm hồ sơ kế hoạch sẽ thay đổi thuật toán thế nào, đến đâu, và kiểm chứng hiệu năng sau thay đổi ra sao; thay đổi trong phạm vi kế hoạch đã duyệt có thể thực hiện theo kế hoạch kèm lưu hồ sơ mà không phải nộp lại toàn bộ hồ sơ, còn thay đổi ngoài kế hoạch vẫn phải làm việc lại với FDA.
## हिन्दी (प्रारंभिक अनुवाद, समीक्षा लंबित)

> यह व्यक्तिगत अध्ययन नोट है, चिकित्सा या कानूनी सलाह नहीं। आपात स्थिति में 911 पर कॉल करें। यह लेख चिकित्सा AI और नैदानिक निर्णय समर्थन (CDS) सॉफ़्टवेयर की अमेरिकी नियामक सीमाओं को रखता है, और किसी दवा की मात्रा का उल्लेख नहीं करता।

**वैधानिक रेखा।** 21वीं सदी उपचार अधिनियम की धारा 3060 ने FD&C Act में धारा 520(o) जोड़ी, जिसने कुछ सॉफ़्टवेयर कार्यों को उपकरण की परिभाषा से बाहर किया। CDS के लिए FDA का सितंबर 2022 का अंतिम मार्गदर्शन, *Clinical Decision Support Software*, इस छूट को चार मानदंडों के आसपास पढ़ता है: सॉफ़्टवेयर चिकित्सा छवि, in vitro नैदानिक संकेत या शारीरिक संकेत-पैटर्न का स्वयं अधिग्रहण, प्रसंस्करण या विश्लेषण न करे; वह चिकित्सा जानकारी प्रदर्शित, विश्लेषित या मुद्रित करे, या रोकथाम, निदान, उपचार पर सहायक सिफ़ारिशें दे; वह स्वास्थ्य पेशेवरों के लिए हो, रोगियों या देखभालकर्ताओं को सीधे निष्कर्ष देने के लिए नहीं; और वह इस प्रकार बना हो कि पेशेवर उसकी सिफ़ारिशों के आधार की स्वतंत्र समीक्षा कर सके — सॉफ़्टवेयर वह जानकारी, तर्क या स्रोत खोलता है जिन पर वह टिका है, ताकि चिकित्सक परिणाम पर मुख्य रूप से निर्भर हुए बिना आधार को स्वयं परखे। जो सॉफ़्टवेयर बिना समीक्षा-योग्य आधार के एकमात्र निश्चित उत्तर देता है, या समय-दबाव वाले निर्णयों के लिए है जहाँ समीक्षा अव्यावहारिक है, वह उपकरण पक्ष की ओर झुकता है।

**उपकरण मार्ग और बदलते एल्गोरिदम।** उपकरण पक्ष का सॉफ़्टवेयर परिचित मार्गों से जाता है: पूर्ववर्ती उत्पाद हो तो 510(k) पूर्व-बाज़ार अधिसूचना, नए कम-से-मध्यम जोखिम प्रकारों के लिए De Novo मार्ग, और उच्चतम जोखिम उत्पादों के लिए PMA। IMDRF का SaMD (चिकित्सा उपकरण के रूप में सॉफ़्टवेयर) ढाँचा — सॉफ़्टवेयर को उसके द्वारा दी गई जानकारी के महत्व और लक्षित अवस्था की गंभीरता से श्रेणीबद्ध करना — इस जोखिम-स्तरीकरण की साझा भाषा है। सीखने वाले तंत्रों के लिए मुख्य उपकरण है पूर्वनिर्धारित परिवर्तन नियंत्रण योजना (PCCP): निर्माता शुरुआत में ही बता देता है कि वह एल्गोरिदम में क्या बदलाव करेगा, कहाँ तक जाएगा, और प्रत्येक बदलाव का सत्यापन कैसे होगा; स्वीकृत योजना के भीतर के बदलाव योजना के तहत किए जा सकते हैं, हर बार नए पूर्ण आवेदन के बिना, जबकि योजना के बाहर के बदलावों पर FDA से फिर प्रक्रिया करनी होगी।

**पारदर्शिता और डेटा।** ONC का HTI-1 नियम, 45 C.F.R. § 170.315(b)(11) पर, प्रमाणित स्वास्थ्य IT से भविष्यवाणी-आधारित निर्णय समर्थन हस्तक्षेपों के स्रोत गुणों — विकासकर्ता, इच्छित उपयोग, विकास डेटा का स्वरूप, ज्ञात सीमाएँ व निष्पक्षता संबंधी विचार, और सत्यापन — का प्रकटीकरण माँगता है, चाहे वह उपकरण हो या न हो। HIPAA केवल covered entities और उनके business associates तक पहुँचता है जब वे संरक्षित स्वास्थ्य जानकारी संभालते हैं; HIPAA की निर्दिष्ट विधियों से de-identify किया गया या विशेषज्ञ-प्रमाणित डेटा अब PHI नहीं रहता, किंतु केवल नाम हटाना de-identification नहीं है। California में AB 3030 (2024) generative AI द्वारा रोगियों के लिए नैदानिक संचार बनने पर अस्वीकरण और मानव-संपर्क मार्ग अनिवार्य करता है, और utilization review में AI राज्य व संघीय निगरानी का विकसित होता क्षेत्र बना हुआ है — किसी भी सारांश पर भरोसा करने से पहले वर्तमान कानून जाँचें।

पूरक: पारदर्शिता की धुरी केवल FDA में नहीं, ONC की health IT प्रमाणन प्रणाली में भी है। HTI-1 नियम द्वारा जोड़ा गया decision support interventions मानक (45 C.F.R. § 170.315(b)(11)) प्रमाणित health IT द्वारा दी जाने वाली भविष्यवाणी-आधारित निर्णय सहायता के लिए एल्गोरिदम स्रोत गुणों का एक समूह प्रकट — हस्तक्षेप का नाम व विकासकर्ता, इच्छित उपयोग, विकास डेटा की प्रकृति, ज्ञात सीमाएँ व निष्पक्षता विचार, और बाहरी सत्यापन की स्थिति — प्रकट करने को कहता है। मशीन-लर्निंग सॉफ़्टवेयर के बदलते रहने की समस्या के लिए उत्तर पूर्वनिर्धारित परिवर्तन नियंत्रण योजना (PCCP) है: निर्माता आवेदन के साथ ही योजना जमा करता है कि एल्गोरिदम कैसे और कहाँ तक बदलेगा और बदलाव के बाद प्रदर्शन कैसे सत्यापित होगा; स्वीकृत योजना की सीमा के भीतर के बदलाव योजना अनुसार लागू कर दस्तावेज़ित किए जा सकते हैं, हर बार पूरा आवेदन दोबारा दिए बिना, जबकि योजना-बाहरी बदलावों पर FDA से फिर से निपटना होगा।
