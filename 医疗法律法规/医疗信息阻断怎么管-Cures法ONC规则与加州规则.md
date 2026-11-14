# 医疗信息阻断怎么管：21 世纪治愈法、ONC 规则与加州规则

> 个人学习笔记，不构成医疗或法律建议。本文梳理联邦信息阻断（information blocking）规则的适用对象、八项例外与执行口径，并注明与 HIPAA 及加州法的衔接；条文以现行 C.F.R. 与官方指引为准。

## 中文主文

### 一、规则的来历：从「有数据」到「数据要流动」

电子病历普及后，一个老问题变成新问题：数据明明在系统里，却因为机构、厂商或流程上的阻拦，患者与其他医疗方拿不到、用不上。《21 世纪治愈法》（21st Century Cures Act）§ 4004 因此创设了信息阻断规则，法典位置在 42 U.S.C. § 300jj-52；健康信息技术国家协调官办公室（ONC）以规章落地于 45 C.F.R. Part 171。规则的核心定义是：**凡可能干扰、阻止或实质劝退对电子健康信息（EHI）的访问、交换或使用的行为，除非法律要求或落入八项例外之一，即构成信息阻断。**

### 二、谁受管：三类行为体

1. **医疗服务提供者**（health care providers）：医院、诊所、医生等；
2. **认证健康 IT 开发者**（health IT developers of certified health IT）：电子病历厂商等；
3. **健康信息交换组织/网络**（HIE/HIN）：区域健康信息交换等中间层。

EHI 的范围与 HIPAA 的「指定记录集」（designated record set）中的电子受保护健康信息对应（定义见 45 C.F.R. § 171.102），不是机构内部的全部数据，更不是纸质记录本身。

### 三、八项例外：正当理由必须对号入座

Part 171 把不构成信息阻断的情形列成八项例外，每项都有自己的构成要件，用错一项即不成立：

- **防止伤害例外**（§ 171.201）：有合理依据相信放行会造成身体伤害；
- **隐私例外**（§ 171.202）：州法或联邦法要求的前置条件（如特定同意）未满足等情形；
- **安全例外**（§ 171.203）：直接关系到系统与数据安全的措施；
- **不可行例外**（§ 171.204）：不可控事件、无法按要求方式提供等，须按规定书面回应请求方；
- **健康 IT 性能例外**（§ 171.205）：计划内维护等暂时不可用，须符合约定时限；
- **内容与方式例外**（§ 171.301）：无法以请求的方式提供时，按规则的阶梯顺序提供替代方式；
- **费用例外**（§ 171.302）：收费须基于客观统一标准、与成本合理相关，不得按竞争关系差别定价；
- **许可例外**（§ 171.303）：对互操作元素的许可须满足规则列明的条款与时限。

实务要点：例外是「逐项论证」的——机构须能说清自己落入哪一项、该项的每个要件如何满足，而不是笼统声称「出于隐私/安全考虑」。

### 四、执行与后果：三类主体，三种力度

- 对开发者与 HIE/HIN：HHS 监察长办公室（OIG）可处民事罚款（civil money penalties），法定上限为**每起违规最高 100 万美元**（42 U.S.C. § 300jj-52(b) 一带）；
- 对医疗服务提供者：走「适当的不利激励」（appropriate disincentives）路径——通过其参加的联邦项目（如 Medicare 的质量支付安排）落实后果，具体以 CMS 当期规则为准；
- 投诉入口是公开的：患者与同行都可通过 ONC 的信息阻断投诉门户提交线索，ONC 转交 OIG 调查。规则自 2021 年 4 月 5 日起适用（applicability date），覆盖范围此后按规章时间表扩展至全部 EHI。

### 五、与 HIPAA 和加州法的关系

- **与 HIPAA 不冲突、是两层**：HIPAA 给患者访问权（45 C.F.R. § 164.524），信息阻断规则管的是「不得无正当理由阻拦流动」；一家机构完全可能形式上遵守 HIPAA 的披露流程、却因无理由地拖延或设卡而踩信息阻断线。反过来，HIPAA 或州法**要求**限制披露的情形（如更严格的州隐私法），属于规则承认的正当理由范围。
- **加州衔接**：加州患者查阅病历的权利另有州法通道（Health & Safety Code § 123110 的查阅与复制规则），医疗信息保密由《医疗信息保密法》（CMIA, Civil Code § 56 起）管辖，其对某些类别信息的同意要求严于联邦底线——在加州判断「能不能放行」时，须先过 CMIA 与专科同意规则，再看联邦信息阻断的例外是否对得上。

*声明：个人学习笔记，不构成医疗或法律建议。来源：21st Century Cures Act § 4004；42 U.S.C. § 300jj-52；45 C.F.R. Part 171（§§ 171.102、171.201–171.205、171.301–171.303）；45 C.F.R. § 164.524；Cal. Health & Saf. Code § 123110；Cal. Civ. Code § 56 et seq.（CMIA）。*

---

## English

Information blocking law comes from § 4004 of the 21st Century Cures Act, codified at 42 U.S.C. § 300jj-52 and implemented by ONC at 45 C.F.R. Part 171: any practice likely to interfere with access, exchange or use of electronic health information (EHI, defined at § 171.102 by reference to the designated record set) is information blocking unless required by law or covered by one of eight exceptions — preventing harm, privacy, security, infeasibility, health IT performance, content and manner, fees, and licensing (§§ 171.201–171.205, 171.301–171.303) — each with its own conditions that must be met element by element. The rule binds health care providers, developers of certified health IT, and health information exchanges/networks. OIG may impose civil money penalties of up to $1 million per violation on developers and exchanges, while providers face "appropriate disincentives" through federal programs. The rule complements rather than replaces HIPAA's access right (§ 164.524), and in California it must be read alongside patient access under Health & Safety Code § 123110 and confidentiality under the CMIA (Civil Code § 56 et seq.). *Personal study notes only; not medical or legal advice.*

## Español (traducción de estudio, pendiente de revisión nativa)

La norma contra el bloqueo de información proviene de la § 4004 de la 21st Century Cures Act, codificada en 42 U.S.C. § 300jj-52 y desarrollada por la ONC en 45 C.F.R. Parte 171: toda práctica que probablemente interfiera con el acceso, intercambio o uso de información electrónica de salud (EHI, definida en § 171.102 por referencia al conjunto de registros designado) es bloqueo de información, salvo que la ley lo exija o aplique una de ocho excepciones — prevención de daño, privacidad, seguridad, inviabilidad, rendimiento de la tecnología sanitaria, contenido y forma, tarifas y licencias (§§ 171.201–171.205, 171.301–171.303) — cada una con requisitos propios que deben cumplirse elemento por elemento. La norma obliga a proveedores de salud, desarrolladores de tecnología sanitaria certificada y redes de intercambio (HIE/HIN). La OIG puede imponer sanciones civiles de hasta 1 millón de dólares por infracción a desarrolladores e intermediarios, mientras los proveedores enfrentan «desincentivos apropiados» en programas federales. La regla complementa, sin reemplazar, el derecho de acceso de HIPAA (§ 164.524), y en California debe leerse junto al acceso del paciente (Health & Safety Code § 123110) y la confidencialidad de la CMIA (Civil Code § 56 y ss.). *Notas de estudio personales; no es asesoría médica ni legal.*

## 한국어 (초역, 원어민 감수 대기)

정보 차단(information blocking) 규칙은 21st Century Cures Act §4004에서 나왔고 42 U.S.C. §300jj-52에 성문화되었으며 ONC가 45 C.F.R. Part 171로 시행합니다. 전자건강정보(EHI, §171.102에서 지정 기록집합을 기준으로 정의)에 대한 접근·교환·사용을 방해할 가능성이 있는 행위는, 법이 요구하거나 여덟 가지 예외 중 하나에 해당하지 않으면 정보 차단입니다. 예외는 위해 방지, 프라이버시, 보안, 실행 불가, 건강 IT 성능, 내용과 방식, 수수료, 라이선스이며(§§171.201–171.205, 171.301–171.303) 각각의 요건을 요소별로 충족해야 합니다. 적용 대상은 의료 제공자, 인증 건강 IT 개발자, 건강정보교환 조직/네트워크입니다. OIG는 개발자와 교환 조직에 위반 건당 최대 100만 달러의 민사 벌금을 부과할 수 있고, 제공자는 연방 프로그램을 통한 '적절한 불이익'을 받습니다. 이 규칙은 HIPAA 접근권(§164.524)을 대체하지 않고 보완하며, 캘리포니아에서는 환자 열람권(Health & Safety Code §123110)과 CMIA(Civil Code §56 이하)의 비밀유지 규정과 함께 읽어야 합니다. 실무에서 중요한 것은 예외를 항목별로 입증해야 한다는 점입니다. "프라이버시나 보안 때문"이라는 뭉뚱그린 주장은 성립하지 않고, 자신이 어느 예외에 해당하는지, 그 예외의 요건을 하나씩 어떻게 충족하는지를 설명할 수 있어야 합니다. 예를 들어 실행 불가 예외는 요청자에게 규정된 방식으로 서면 답변을 해야 하고, 수수료 예외의 요금은 객관적이고 일률적인 기준에 따라 비용과 합리적으로 연관되어야 하며 경쟁 관계에 따라 다르게 매길 수 없습니다. 이 규칙은 2021년 4월 5일부터 적용되었고, 환자와 동료 의료인은 ONC의 정보 차단 신고 포털을 통해 단서를 제출할 수 있으며 ONC는 이를 OIG에 넘겨 조사하게 합니다.

*개인 학습 노트이며 의학·법률 자문이 아닙니다.*

## Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

Quy định về chặn thông tin (information blocking) xuất phát từ § 4004 của Đạo luật Chữa trị Thế kỷ 21 (21st Century Cures Act), được hệ thống hóa tại 42 U.S.C. § 300jj-52 và do ONC triển khai tại 45 C.F.R. Phần 171: mọi hành vi có khả năng cản trở việc truy cập, trao đổi hoặc sử dụng thông tin sức khỏe điện tử (EHI, định nghĩa tại § 171.102 theo tập hồ sơ chỉ định) đều là chặn thông tin, trừ khi luật yêu cầu hoặc thuộc một trong tám ngoại lệ — ngăn ngừa tổn hại, quyền riêng tư, an ninh, không khả thi, hiệu năng công nghệ thông tin y tế, nội dung và cách thức, phí, và cấp phép (§§ 171.201–171.205, 171.301–171.303) — mỗi ngoại lệ có điều kiện riêng phải đáp ứng từng yếu tố. Quy định ràng buộc nhà cung cấp dịch vụ y tế, nhà phát triển công nghệ thông tin y tế được chứng nhận và các tổ chức/mạng trao đổi thông tin y tế. OIG có thể phạt tiền dân sự tới 1 triệu đô la mỗi vi phạm đối với nhà phát triển và tổ chức trao đổi, còn nhà cung cấp chịu «biện pháp răn đe thích hợp» qua các chương trình liên bang. Quy định này bổ sung chứ không thay thế quyền truy cập của HIPAA (§ 164.524), và tại California phải đọc cùng quyền truy cập của bệnh nhân (Health & Safety Code § 123110) và bảo mật theo CMIA (Civil Code § 56 trở đi). Điểm then chốt trong thực hành là các ngoại lệ phải được lập luận theo từng hạng mục: nói chung chung "vì quyền riêng tư hay an ninh" là không đủ; tổ chức phải chỉ rõ mình rơi vào ngoại lệ nào và từng điều kiện của ngoại lệ đó được đáp ứng ra sao. Ví dụ, ngoại lệ không khả thi đòi hỏi phải trả lời bằng văn bản cho bên yêu cầu theo cách quy định; ngoại lệ về phí yêu cầu mức phí dựa trên tiêu chuẩn khách quan, thống nhất, liên quan hợp lý đến chi phí, và không được định giá khác nhau theo quan hệ cạnh tranh. Quy định này áp dụng từ ngày 5 tháng 4 năm 2021; bệnh nhân và đồng nghiệp đều có thể gửi đầu mối qua cổng khiếu nại chặn thông tin của ONC, và ONC chuyển cho OIG điều tra.

*Ghi chú học tập cá nhân, không phải tư vấn y tế hay pháp lý.*

## हिन्दी (प्रारंभिक अनुवाद, मूल-भाषी समीक्षा लंबित)

सूचना-अवरोध (information blocking) नियम 21st Century Cures Act की § 4004 से आया है, जो 42 U.S.C. § 300jj-52 में संहिताबद्ध है और ONC द्वारा 45 C.F.R. Part 171 में लागू है: इलेक्ट्रॉनिक स्वास्थ्य सूचना (EHI, § 171.102 में designated record set के संदर्भ से परिभाषित) की पहुँच, आदान-प्रदान या उपयोग में बाधा डालने वाला कोई भी व्यवहार सूचना-अवरोध है, जब तक कानून उसे आवश्यक न करे या आठ अपवादों में से कोई लागू न हो — हानि रोकथाम, गोपनीयता, सुरक्षा, अव्यवहार्यता, स्वास्थ्य IT प्रदर्शन, सामग्री व तरीका, शुल्क और लाइसेंसिंग (§§ 171.201–171.205, 171.301–171.303) — प्रत्येक की अपनी शर्तें तत्व-दर-तत्व पूरी करनी होती हैं। नियम स्वास्थ्य सेवा प्रदाताओं, प्रमाणित स्वास्थ्य IT डेवलपर्स और स्वास्थ्य सूचना विनिमय संगठनों/नेटवर्कों पर लागू है। OIG डेवलपर्स व विनिमय संगठनों पर प्रति उल्लंघन अधिकतम 1 मिलियन डॉलर तक नागरिक जुर्माना लगा सकता है, जबकि प्रदाताओं को संघीय कार्यक्रमों के माध्यम से 'उचित प्रतिरोध' मिलता है। यह नियम HIPAA के पहुँच अधिकार (§ 164.524) का पूरक है, प्रतिस्थापन नहीं, और California में इसे रोगी पहुँच (Health & Safety Code § 123110) व CMIA (Civil Code § 56 व आगे) की गोपनीयता के साथ पढ़ना चाहिए। व्यवहार में महत्वपूर्ण बात यह है कि अपवादों को तत्व-दर-तत्व सिद्ध करना होता है: "गोपनीयता या सुरक्षा के कारण" जैसा सामान्य दावा पर्याप्त नहीं; संस्थान को बताना होगा कि वह किस अपवाद में आता है और उस अपवाद की हर शर्त कैसे पूरी होती है। उदाहरण के लिए, अव्यवहार्यता अपवाद में अनुरोधकर्ता को निर्धारित तरीके से लिखित उत्तर देना होता है, और शुल्क अपवाद में शुल्क वस्तुनिष्ठ व एकसमान मानदंडों पर आधारित, लागत से युक्तिसंगत रूप से जुड़ा होना चाहिए तथा प्रतिस्पर्धा के आधार पर अलग नहीं रखा जा सकता। यह नियम 5 अप्रैल 2021 से लागू है; रोगी और सहयोगी ONC के सूचना-अवरोध शिकायत portal के माध्यम से शिकायत भेज सकते हैं, जिसे ONC जाँच के लिए OIG को भेजता है।

*व्यक्तिगत अध्ययन नोट; चिकित्सा या कानूनी सलाह नहीं।*


## 补译增量（2026-11-13 15:55 轮）

### 한국어 (초역, 初译待校)

보충 세부사항 두 가지. 첫째, 집행의 세 갈래입니다. 개발자와 건강정보교환조직/네트워크(HIE/HIN)에 대해서는 HHS 감사관실(OIG)이 건당 최고 100만 달러까지의 민사 벌금(civil money penalties)을 부과할 수 있습니다(42 U.S.C. § 300jj-52 일대). 의료 제공자는 벌금 트랙이 아니라 '적절한 불이익(appropriate disincentives)' 트랙으로, Medicare 품질 지급 같은 연방 프로그램 참여를 통해 결과가 닿으며 구체 내용은 CMS 현행 규칙을 따릅니다. 규칙의 적용 개시일은 2021년 4월 5일이고, 적용 범위는 그 후 규칙 일정에 따라 전체 전자건강정보(EHI)로 넓어졌습니다. 둘째, HIPAA와의 이층 관계와 캘리포니아 순서입니다. 기관이 HIPAA 공개 절차를 형식적으로 지켰더라도 이유 없는 지연이나 장벽으로 흐름을 막으면 정보 차단을 구성할 수 있습니다. 반대로 HIPAA나 주법이 공개 제한을 요구하는 경우는 정당한 사유로 인정됩니다. 캘리포니아에서는 환자의 기록 열람권에 Health and Safety Code § 123110의 주법 경로가 따로 있고, 의료정보 비밀은 CMIA(Civil Code § 56 이하)가 관할하며 일부 정보 범주의 동의 요건이 연방 하한보다 엄격합니다. 따라서 캘리포니아에서 공개 가능 여부를 판단할 때는 먼저 CMIA와 개별 동의 규칙을 통과한 뒤, 연방 정보 차단 예외가 맞는지를 대조합니다.

### Tiếng Việt (bản dịch, 初译待校)

Hai chi tiết bổ sung. Thứ nhất, ba nhánh thực thi. Đối với nhà phát triển và tổ chức/mạng lưới trao đổi thông tin y tế (HIE/HIN), Văn phòng Tổng thanh tra HHS (OIG) có thể áp tiền phạt dân sự (civil money penalties) tối đa 1 triệu đô la cho mỗi vi phạm (quanh 42 U.S.C. § 300jj-52). Đối với nhà cung cấp dịch vụ y tế, con đường là "biện pháp răn đe thích hợp" (appropriate disincentives) — hậu quả đến qua các chương trình liên bang mà họ tham gia, như cơ chế chi trả theo chất lượng của Medicare, với chi tiết theo quy định CMS hiện hành. Ngày bắt đầu áp dụng của quy tắc là 5 tháng 4 năm 2021, và phạm vi áp dụng sau đó mở rộng theo lịch trình quy định tới toàn bộ thông tin sức khỏe điện tử (EHI). Thứ hai, quan hệ hai tầng với HIPAA và thứ tự xét tại California. Một tổ chức có thể tuân thủ hình thức quy trình tiết lộ của HIPAA nhưng vẫn cấu thành chặn thông tin nếu trì hoãn hoặc dựng rào cản vô lý đối với dòng chảy dữ liệu; ngược lại, trường hợp HIPAA hoặc luật bang yêu cầu hạn chế tiết lộ thì thuộc phạm vi lý do chính đáng được quy tắc thừa nhận. Tại California, quyền xem hồ sơ của bệnh nhân còn có kênh luật bang tại Health and Safety Code § 123110, còn bảo mật thông tin y tế do CMIA (Civil Code § 56 trở đi) điều chỉnh, với yêu cầu đồng ý cho một số nhóm thông tin nghiêm ngặt hơn mức sàn liên bang. Vì vậy, khi xét "có được phép tiết lộ hay không" tại California, phải qua CMIA và các quy tắc đồng ý chuyên biệt trước, rồi mới đối chiếu ngoại lệ chặn thông tin của liên bang.

### हिन्दी (प्रारंभिक अनुवाद, 初译待校)

दो पूरक विवरण। पहला, प्रवर्तन की तीन धाराएँ। डेवलपर्स और स्वास्थ्य सूचना विनिमय संगठनों/नेटवर्कों (HIE/HIN) पर HHS महानिरीक्षक कार्यालय (OIG) प्रति उल्लंघन अधिकतम 1 मिलियन डॉलर तक नागरिक जुर्माना (civil money penalties) लगा सकता है (42 U.S.C. § 300jj-52 के आसपास)। स्वास्थ्य सेवा प्रदाताओं पर जुर्माना-पथ नहीं, 'उचित प्रतिरोध' (appropriate disincentives) पथ लागू होता है — परिणाम उन संघीय कार्यक्रमों के माध्यम से पहुँचता है जिनमें वे भाग लेते हैं, जैसे Medicare गुणवत्ता-भुगतान व्यवस्था, जिसका विवरण CMS के वर्तमान नियमों से तय होता है। नियम की प्रयोज्यता तिथि 5 अप्रैल 2021 है और उसके बाद दायरा नियम-अनुसूची अनुसार संपूर्ण इलेक्ट्रॉनिक स्वास्थ्य सूचना (EHI) तक फैला। दूसरा, HIPAA के साथ द्विस्तरीय संबंध और कैलिफ़ोर्निया क्रम। कोई संस्था HIPAA प्रकटीकरण प्रक्रिया का औपचारिक पालन करते हुए भी यदि अनुचित देरी या अवरोध से डेटा-प्रवाह रोके तो सूचना-अवरोध बन सकता है; इसके विपरीत, जहाँ HIPAA या राज्य-विधि प्रकटीकरण सीमित करने को कहे, वह नियम द्वारा मान्यता प्राप्त उचित कारण है। कैलिफ़ोर्निया में रोगी के अभिलेख-दर्शन अधिकार का अलग राज्य-मार्ग Health and Safety Code § 123110 है, और चिकित्सा सूचना गोपनीयता CMIA (Civil Code § 56 व आगे) के अधीन है, जिसकी कुछ सूचना-श्रेणियों की सहमति-आवश्यकताएँ संघीय न्यूनतम से कठोर हैं। अतः कैलिफ़ोर्निया में 'प्रकट किया जा सकता है या नहीं' तय करते समय पहले CMIA व विशेष सहमति नियमों से गुज़रें, फिर संघीय सूचना-अवरोध अपवाद का मिलान करें।
