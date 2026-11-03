# 医疗 AI 与临床决策支持怎么管：FDA 的 CDS 框架、HIPAA 及加州 AB 3030

医院里越来越多软件在“帮医生看病”：有的把指南要点推到屏幕上，有的直接对着影像给出判断，还有聊天机器人替诊所给患者回消息。这些东西到底算不算医疗器械、要不要先过 FDA、患者数据受什么法律管、AI 写给患者的话要不要标注——美国现行规则不是一张总图，而是几条线分别在管。这篇把四条线拆开讲：FDA 的临床决策支持（CDS）划线、ONC 对算法透明度的要求、HIPAA 真正的适用范围，以及加州 AB 3030 对生成式 AI 患者沟通的标注义务。全篇只讲制度信息，不涉及任何药物剂量，具体的软件定性和合规判断要由专业人士结合产品功能确认。

## 中文主文

### 一、起点：治愈法把一部分 CDS 软件移出了“器械”定义

关键条文出在《21 世纪治愈法》（21st Century Cures Act）第 3060 条。它修订了《联邦食品、药品和化妆品法》（FDCA）第 520(o) 条（21 U.S.C. § 360j(o)），把某些软件功能从“器械”（device）的法定定义里排除出去。其中和临床最相关的一类，就是满足特定条件的临床决策支持软件。

被排除的 CDS 大致要同时符合这样的画像：软件面向的是医疗专业人员；它提供的是信息、选项或建议，供医生在诊疗中参考；更要紧的是，它的设计要让医生能够独立审查这些建议背后的依据——比如能看到所依据的数据、指南或逻辑——并且医生不会把它当作主要依赖来做决定。立法的意思很直白：软件只是帮医生把依据摆到台面上、决定仍然实实在在由医生独立作出时，这类功能就不按医疗器械来管。理解这一条，要抓住两个词：“可独立审查依据”和“不作主要依赖”，后面 FDA 的指南也是围着这两点展开的。

### 二、反面清单：哪些软件仍然是器械，要走 FDA 路径

排除不是通行证。同样是给临床出主意的软件，落到下面几种情形，仍然属于器械，要走 FDA 的上市路径（视风险等级走 510(k)、De Novo 或 PMA 等程序）：

第一类，处理医学影像或信号的软件。比如对 CT、病理切片、监护波形等影像或生理信号做分析并给出判断的，立法排除时明确没有把它放进去，这类产品一直是 FDA 器械监管的主场。

第二类，给出单一确定结论、而医生无法独立复核其依据的软件。软件如果只吐出一个“是或不是”的结论，却不展示依据、数据来源或推理路径，医生除了信或不信没有别的抓手，这就不再是“支持决策”，而是实质上在替医生下判断，按器械管。

第三类，时间紧迫场景下使用的软件。在急救、监护报警这类分秒必争的场景里，医生客观上没有时间去逐条复核依据，软件输出事实上会被直接当作行动指令，监管上也按器械对待。

FDA 在 2022 年 9 月发布的《Clinical Decision Support Software》最终指南，就是把上面这条线画细的文件：它逐项解释 FDA 如何理解 520(o) 的排除条件，哪些功能落在排除侧、哪些落在器械侧，并给了不少示例。做产品或采购评估时，这份指南是第一手的划线依据；但要提醒一句，指南是 FDA 的解释口径，不改变法条本身，个案定性最终看产品实际功能与宣传用途的组合。

### 三、ONC 的 HTI-1：不管是不是器械，算法要把来源说清

第二条线来自健康 IT 认证体系。联邦卫生 IT 协调办公室（ONC）的 HTI-1 规则在 45 CFR § 170.315(b)(11) 设立了“决策支持干预”（Decision Support Interventions）认证标准。它的管法和 FDA 不同：不问软件算不算器械，而是要求使用认证健康 IT（比如主流电子病历系统）提供预测性决策支持时，必须公开算法的来源属性——诸如开发方、所用数据的大致构成、 intended use、已知的局限与公平性相关的考量等一组透明度信息，让使用方和采购方能查、能比、能追问。

这条线的意义在于补位：有些工具即便落在 FDA 的器械定义之外，也不等于可以做成黑箱。医院在采购和上线评估时，可以依据这组公开属性做内部审查；医生在临床使用时，至少知道这个建议大致是“谁做的、拿什么数据做的、边界在哪”。对患者而言，它不是直接的知情同意规则，而是通过机构采购与治理间接起作用。

### 四、HIPAA 的真实边界：不是一切健康 App 的总法

第三条线最容易被说过头。HIPAA 经常被当成“美国健康隐私总法”，其实它的适用面要窄得多：HIPAA 的隐私与安全规则只约束受保主体（covered entity，如医疗机构、健康计划、医疗信息交换中心）及其业务伙伴（business associate），且只针对这些主体手里的受保护健康信息（protected health information，PHI）。

落到日常场景就是：医院电子病历里的数据、诊所用 AI 工具处理患者病历——只要经手方是受保主体或其业务伙伴，HIPAA 就适用，业务伙伴合同、最小必要、安全 safeguards 这些要求都要跟上。反过来，一个面向消费者的健康 App，如果运营方既不是受保主体也不是业务伙伴，用户自己输入的数据就不在 HIPAA 管辖之内，哪怕内容同样敏感。这类场景可能转而受联邦贸易委员会（FTC）的健康泄露通知规则、州消费者隐私法或州医疗信息法的管辖（加州另有 CMIA 等州法），但不能笼统地说“受 HIPAA 保护”。判断任何一款医疗 AI 产品的数据合规，第一步永远是先问主体身份和数据流向，而不是先背 HIPAA 条款。

### 五、加州 AB 3030：AI 写给患者的话，必须标明并留真人通道

第四条线是州法，管的是沟通环节。加州 AB 3030（2024）针对生成式人工智能在医疗沟通中的使用立了规矩，自 2025 年 1 月 1 日起生效：医疗机构使用生成式 AI 生成与患者的临床信息相关沟通内容时（比如检查结果说明、随访提醒、诊疗相关的消息回复），必须附上免责声明，表明该内容由生成式 AI 生成；同时要给患者留出联系真人的通道，让患者能方便地转到真实工作人员沟通。

这条规则的着眼点不是临床判断本身对不对，而是患者有没有知情：对面这段话是机器写的还是医护写的，患者有权知道，并且有权绕过机器找到人。需要注意它的射程：它管的是“与患者沟通临床信息”的生成内容，不是医院内部所有的 AI 使用；触发点在内容由生成式 AI 生成并发送给患者。具体条号与执行细则以加州现行法典和卫生机构指引为准，本文只引用法案本身 AB 3030 (2024)，不另编条号。

### 六、四条线怎么合起来用：一张简易判断顺序

面对任何一个医疗 AI 或 CDS 产品，可以按这个顺序过一遍：先看功能——它是否让医生能独立审查依据、是否只是辅助而非主要依赖、是否碰影像信号或时间紧迫场景，据此对照 FDCA 第 520(o) 条与 FDA 2022 年指南，判断落在器械侧还是排除侧；再看部署——它是否嵌在认证健康 IT 里提供预测性支持，是的话查 45 CFR § 170.315(b)(11) 要求的来源属性是否公开齐全；然后看数据——经手方是不是 HIPAA 的受保主体或业务伙伴、数据是不是 PHI，决定 HIPAA 是否适用、还要不要叠加州法；最后看沟通——如果在加州用生成式 AI 直接给患者发临床信息，AB 3030 的免责声明和真人联系通道有没有落实。这个顺序走完，一款产品的监管轮廓大致就清楚了。

*本文为个人学习笔记，不构成医疗建议，也不构成法律意见；具体产品的器械定性与合规方案，请咨询 FDA 监管专业人士或医疗法律师。主要来源：《21 世纪治愈法》第 3060 条与 FDCA 第 520(o) 条（21 U.S.C. § 360j(o)）；FDA《Clinical Decision Support Software》最终指南（2022 年 9 月）；ONC HTI-1 规则与 45 CFR § 170.315(b)(11)；HIPAA 隐私与安全规则（45 CFR Part 160、164）关于受保主体与业务伙伴的适用口径；加州 AB 3030 (2024)。具体条文以各机构现行发布为准。*

---

## English

U.S. oversight of medical AI runs on separate tracks. Section 3060 of the 21st Century Cures Act amended FDCA Section 520(o) (21 U.S.C. § 360j(o)) to exclude certain clinical decision support (CDS) software functions from the statutory definition of a device.

The exclusion fits software that presents information or options to clinicians, lets the clinician independently review the basis for its recommendations, and is not intended as the primary basis for a decision. Judgment stays visibly with the clinician.

The opposite side remains a regulated device: software processing medical images or signals, software giving a single definitive conclusion whose basis cannot be independently reviewed, and software for time-critical settings. FDA drew this line in its September 2022 final guidance, Clinical Decision Support Software.

Transparency is a second track. ONC's HTI-1 rule, at 45 CFR § 170.315(b)(11) (Decision Support Interventions), requires certified health IT to disclose source attributes of predictive algorithms — who built the tool, on what data, with what limits.

HIPAA is narrower than often assumed: it applies only where protected health information is handled by a covered entity or business associate, not to every health app. In California, AB 3030 (2024), effective January 1, 2025, requires a disclaimer and a way to reach a human when generative AI produces clinical communications to patients.

## Español

La supervisión de la IA médica en EE. UU. avanza por vías separadas. La Sección 3060 de la Ley de Curas del Siglo XXI modificó la Sección 520(o) de la FDCA (21 U.S.C. § 360j(o)) para excluir ciertas funciones de software de apoyo a la decisión clínica (CDS) de la definición legal de dispositivo.

La exclusión encaja con el software que presenta información u opciones a los clínicos, les permite revisar de forma independiente la base de sus recomendaciones y no está pensado como base principal de la decisión. El juicio queda visiblemente en manos del clínico.

El lado contrario sigue regulado como dispositivo: el software que procesa imágenes o señales médicas, el que ofrece una única conclusión definitiva cuya base no puede revisarse por separado, y el destinado a situaciones de urgencia temporal. La FDA trazó la línea en su guía final de septiembre de 2022, Clinical Decision Support Software.

La transparencia es otra vía. La norma HTI-1 de la ONC, en 45 CFR § 170.315(b)(11) sobre Intervenciones de Apoyo a la Decisión, exige revelar los atributos de origen de los algoritmos predictivos: quién lo creó, con qué datos y con qué límites.

HIPAA es más estrecha de lo que suele creerse: solo se aplica cuando una entidad cubierta o un socio comercial maneja información de salud protegida, no a toda aplicación de salud. En California, AB 3030 (2024), vigente desde el 1 de enero de 2025, exige un aviso y contacto con una persona real cuando la IA generativa redacta comunicaciones clínicas a pacientes.

## 한국어（初译待校）

미국에서 의료 AI는 서로 다른 궤도로 감독됩니다. 출발점은 21세기 치유법 제3060조로, FDCA 제520(o)조(21 U.S.C. § 360j(o))를 개정해 일부 임상 의사결정 지원(CDS) 소프트웨어 기능을 법정 '기기' 정의에서 제외했습니다.

제외에 해당하는 것은 임상의에게 정보나 선택지를 제시하고, 임상의가 권고의 근거를 독립적으로 검토할 수 있게 하며, 결정의 주요 근거로 의존하도록 의도되지 않은 소프트웨어입니다. 판단의 주체가 임상의에게 분명히 남아 있는 경우입니다.

반대쪽은 여전히 기기로 규제됩니다. 의료 영상이나 신호를 처리하는 소프트웨어, 임상의가 근거를 독립적으로 검토할 수 없는 단일 확정 결론을 내놓는 소프트웨어, 시간에 쫓기는 상황을 위한 소프트웨어가 여기에 속합니다. 이들은 FDA 시판 경로를 따르며, FDA는 2022년 9월 최종 지침 Clinical Decision Support Software에서 이 경계를 구체화했습니다.

두 번째 궤도는 투명성입니다. ONC의 HTI-1 규칙 45 CFR § 170.315(b)(11)(의사결정 지원 중재)은 인증 건강 IT가 예측 알고리즘의 출처 속성을 공개하도록 요구해, 누가 어떤 데이터로 만들었고 한계가 무엇인지 확인할 수 있게 합니다.

HIPAA는 흔히 생각하는 것보다 좁습니다. 보호 대상 건강 정보를 적용 대상 기관이나 업무 제휴자가 취급할 때만 적용되며, 모든 건강 앱을 포괄하는 법은 아닙니다. 캘리포니아에서는 AB 3030 (2024)이 2025년 1월 1일부터 시행되어, 의료기관이 생성형 AI로 환자에게 임상 정보 관련 내용을 보낼 때 고지와 실제 담당자에게 연락할 경로를 요구합니다.

보충하면, HTI-1의 출처 속성(source attributes)은 추상적 투명성 구호가 아니라 열거된 항목 목록이라는 점을 분명히 해야 합니다. 예측형 의사결정 지원 개입에는 개입의 이름과 개발 주체, 의도된 용도, 학습·개발에 쓰인 데이터의 성격, 알려진 한계와 공정성 관련 고려, 업데이트 방식처럼 사용자가 실제로 대조할 수 있는 속성들이 공개 대상에 포함됩니다. 그래서 조달 심사에서는 벤더의 마케팅 문구가 아니라 이 속성표가 채워져 있는지가 첫 번째 확인 지점이 됩니다. HIPAA 적용 판단도 순서를 고정해 두면 실수가 줄어듭니다. 먼저 데이터가 PHI인지, 다음으로 그 데이터를 다루는 주체가 보장 대상 기관이나 업무 파트너인지, 마지막으로 그 사용·공개가 치료·지불·운영 같은 허용 목적에 들어가는지를 봅니다. 세 단계 중 어느 하나라도 어긋나면 HIPAA의 결론이 달라집니다. AB 3030에 대해서는 적용 범위를 과장하지 않는 것이 중요합니다. 이 법은 생성형 AI가 작성한 환자 대상 임상 커뮤니케이션을 겨냥한 표시·연결 의무이지, 의료기관 내부의 모든 AI 활용에 대한 전면 허가제가 아닙니다. 다만 같은 논리 — 환자가 기계가 쓴 글인지 알 권리와 사람에게 닿을 통로 — 는 다른 주의 입법에서도 반복되고 있어, 다주 운영 기관은 캘리포니아 기준을 사실상 하한선으로 삼는 경향이 있습니다.

## Tiếng Việt（初译待校）

Việc giám sát AI y tế tại Hoa Kỳ đi theo nhiều tuyến riêng. Mục 3060 của Đạo luật Chữa trị Thế kỷ 21 đã sửa đổi Mục 520(o) của FDCA (21 U.S.C. § 360j(o)) để loại trừ một số chức năng phần mềm hỗ trợ quyết định lâm sàng (CDS) khỏi định nghĩa pháp lý về thiết bị.

Loại trừ này áp dụng cho phần mềm trình bày thông tin hoặc lựa chọn cho bác sĩ, cho phép bác sĩ độc lập xem xét cơ sở của khuyến nghị, và không được dự định là cơ sở chính cho quyết định. Phán đoán vẫn rõ ràng thuộc về bác sĩ.

Phía ngược lại vẫn bị quản lý như thiết bị: phần mềm xử lý hình ảnh hoặc tín hiệu y tế, phần mềm đưa ra một kết luận dứt khoát duy nhất mà bác sĩ không thể độc lập kiểm chứng cơ sở, và phần mềm cho tình huống khẩn cấp về thời gian. FDA đã vạch rõ ranh giới này trong hướng dẫn cuối cùng tháng 9 năm 2022, Clinical Decision Support Software.

Minh bạch là tuyến thứ hai. Quy tắc HTI-1 của ONC, tại 45 CFR § 170.315(b)(11) về Can thiệp Hỗ trợ Quyết định, yêu cầu công nghệ thông tin y tế được chứng nhận phải công bố thuộc tính nguồn của thuật toán dự đoán: ai xây dựng, trên dữ liệu nào, với giới hạn gì.

HIPAA hẹp hơn nhiều người tưởng: chỉ áp dụng khi thông tin sức khỏe được bảo vệ do một thực thể thuộc diện điều chỉnh hoặc đối tác kinh doanh xử lý, không phải luật chung cho mọi ứng dụng sức khỏe. Tại California, AB 3030 (2024), hiệu lực từ ngày 1 tháng 1 năm 2025, yêu cầu tuyên bố miễn trừ và kênh liên hệ với người thật khi AI tạo sinh soạn nội dung lâm sàng gửi bệnh nhân.

Bổ sung: cần nói rõ các thuộc tính nguồn (source attributes) của HTI-1 là một danh mục liệt kê cụ thể, không phải khẩu hiệu minh bạch trừu tượng. Với các can thiệp hỗ trợ quyết định mang tính dự đoán, đối tượng phải công bố gồm tên và bên phát triển của can thiệp, mục đích sử dụng dự kiến, tính chất của dữ liệu dùng để phát triển, các giới hạn đã biết và cân nhắc liên quan công bằng, cùng cách thức cập nhật — những thuộc tính mà người dùng thật sự đối chiếu được. Vì vậy khi thẩm định mua sắm, điểm kiểm tra đầu tiên là bảng thuộc tính này đã được điền hay chưa, chứ không phải câu chữ tiếp thị của nhà cung cấp. Phán đoán áp dụng HIPAA cũng nên cố định thứ tự để giảm sai sót: trước hết dữ liệu có phải PHI không, tiếp đó chủ thể xử lý dữ liệu có phải tổ chức được bao phủ hay đối tác kinh doanh không, cuối cùng việc sử dụng, tiết lộ đó có thuộc mục đích được phép như điều trị, thanh toán, vận hành không — lệch một trong ba bước là kết luận HIPAA thay đổi. Với AB 3030, điều quan trọng là không phóng đại phạm vi: luật này nhắm tới nghĩa vụ ghi nhãn và giữ đường liên hệ tới người thật đối với nội dung giao tiếp lâm sàng với bệnh nhân do AI tạo sinh viết ra, chứ không phải chế độ cấp phép toàn diện cho mọi ứng dụng AI nội bộ của cơ sở y tế. Tuy vậy cùng một lôgic — bệnh nhân có quyền biết đoạn văn do máy viết và có đường tới gặp người thật — đang lặp lại trong lập pháp của các bang khác, nên cơ sở hoạt động đa bang có xu hướng lấy chuẩn California làm sàn tối thiểu trên thực tế.

## हिन्दी（初译待校）

अमेरिका में चिकित्सा AI की निगरानी अलग-अलग धाराओं में चलती है। 21वीं सदी उपचार अधिनियम की धारा 3060 ने FDCA धारा 520(o) (21 U.S.C. § 360j(o)) में संशोधन कर कुछ नैदानिक निर्णय समर्थन (CDS) सॉफ़्टवेयर कार्यों को 'उपकरण' की वैधानिक परिभाषा से बाहर किया।

यह छूट उस सॉफ़्टवेयर पर लागू होती है जो चिकित्सकों को जानकारी या विकल्प देता है, उन्हें अपनी सिफ़ारिशों के आधार की स्वतंत्र समीक्षा करने देता है, और निर्णय का मुख्य आधार बनने के लिए नहीं बना है। निर्णय स्पष्ट रूप से चिकित्सक के पास रहता है।

विपरीत पक्ष उपकरण के रूप में ही विनियमित रहता है: चिकित्सा छवियों या संकेतों को संसाधित करने वाला सॉफ़्टवेयर, ऐसा सॉफ़्टवेयर जो एकमात्र निश्चित निष्कर्ष देता है और चिकित्सक उसके आधार की स्वतंत्र जाँच नहीं कर सकता, तथा समय-संवेदनशील स्थितियों का सॉफ़्टवेयर। FDA ने सितंबर 2022 के अंतिम मार्गदर्शन Clinical Decision Support Software में यह रेखा खींची।

पारदर्शिता दूसरी धारा है। ONC का HTI-1 नियम, 45 CFR § 170.315(b)(11) (Decision Support Interventions), प्रमाणित स्वास्थ्य IT से भविष्यवाणी एल्गोरिदम के स्रोत गुणों का खुलासा माँगता है — किसने बनाया, किस डेटा पर, किन सीमाओं के साथ।

HIPAA अक्सर समझे जाने से संकरा है: यह केवल तब लागू होता है जब संरक्षित स्वास्थ्य जानकारी किसी कवर की गई संस्था या व्यावसायिक सहयोगी के पास हो, हर स्वास्थ्य ऐप के लिए सामान्य कानून नहीं है। कैलिफ़ोर्निया में AB 3030 (2024), 1 जनवरी 2025 से प्रभावी, जनरेटिव AI से रोगियों के लिए नैदानिक संचार बनने पर अस्वीकरण और वास्तविक व्यक्ति से संपर्क का रास्ता अनिवार्य करता है।

---

पूरक: स्पष्ट करें कि HTI-1 के source attributes कोई अमूर्त पारदर्शिता नारा नहीं, बल्कि एक गिनी हुई सूची है। पूर्वानुमानात्मक निर्णय समर्थन हस्तक्षेपों के लिए जिन गुणों का प्रकटीकरण अपेक्षित है उनमें हस्तक्षेप का नाम व विकासकर्ता, इच्छित उपयोग, विकास में प्रयुक्त डेटा का स्वरूप, ज्ञात सीमाएँ व निष्पक्षता संबंधी विचार, और अद्यतन का तरीका शामिल हैं — ऐसे गुण जिन्हें उपयोगकर्ता वास्तव में तुलना कर सके। इसलिए खरीद मूल्यांकन में पहला जाँच बिंदु विक्रेता के विपणन वाक्य नहीं, बल्कि यह गुण-तालिका भरी है या नहीं, यही होता है। HIPAA लागू होने का निर्णय भी एक निश्चित क्रम से करें तो गलतियाँ घटती हैं: पहले देखें कि डेटा PHI है या नहीं, फिर कि उसे संभालने वाला पक्ष covered entity या business associate है या नहीं, और अंत में कि वह उपयोग या प्रकटीकरण उपचार, भुगतान, संचालन जैसे अनुमत उद्देश्यों में आता है या नहीं — तीनों में से कोई एक चरण भटके तो HIPAA का निष्कर्ष बदल जाता है। AB 3030 के बारे में दायरा बढ़ाकर न बताना महत्वपूर्ण है: यह कानून generative AI द्वारा लिखे गए रोगी-उन्मुख नैदानिक संचार पर लेबल व मानव-संपर्क मार्ग का दायित्व रखता है, अस्पताल के सभी आंतरिक AI उपयोगों पर कोई व्यापक लाइसेंस व्यवस्था नहीं है। फिर भी यही तर्क — रोगी को यह जानने का अधिकार कि पाठ मशीन ने लिखा है और मनुष्य तक पहुँचने का मार्ग — अन्य राज्यों के विधायन में भी दोहराया जा रहा है, इसलिए बहु-राज्य संस्थान व्यवहार में California मानक को न्यूनतम आधार मानने लगे हैं।

## 六语集中声明区（补译追加，正文未改动）

中文：本文为个人学习笔记，不构成医疗建议，也不构成法律或专业建议；具体事项请以主管部门、发证机构与现行官方文本为准，紧急情况请拨打 911。

English: These are personal study notes, not medical advice and not legal or professional advice. For specific matters, follow the competent authority, the issuing body, and current official texts. In an emergency, call 911.

Español: Estas son notas personales de estudio; no constituyen asesoría médica, legal ni profesional. Para asuntos concretos, siga a la autoridad competente, al organismo emisor y los textos oficiales vigentes. En una emergencia, llame al 911.

한국어 (초역, 원어민 감수 대기): 본 글은 개인 학습 노트이며 의료 자문이나 법률·전문 자문이 아닙니다. 구체적인 사항은 관할 기관, 발급 기관과 현행 공식 문언을 따르십시오. 응급 시 911에 전화하십시오.

Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính): Đây là ghi chú học tập cá nhân, không phải tư vấn y tế, pháp lý hay chuyên môn. Với vấn đề cụ thể, hãy theo cơ quan có thẩm quyền, cơ quan cấp chứng chỉ và văn bản chính thức hiện hành. Trường hợp khẩn cấp, hãy gọi 911.

हिन्दी (प्रारंभिक अनुवाद, मूल-भाषी समीक्षा लंबित): यह व्यक्तिगत अध्ययन नोट है और चिकित्सा, कानूनी या पेशेवर सलाह नहीं है। विशिष्ट मामलों के लिए सक्षम प्राधिकरण, जारी करने वाले निकाय और वर्तमान आधिकारिक पाठों का पालन करें। आपात स्थिति में 911 पर कॉल करें।

