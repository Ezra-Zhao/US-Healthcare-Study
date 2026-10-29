# FDA 药品与器械审批怎么管：上市路径、510(k) 与 PMA

这篇讲什么：
- 一盒药、一台呼吸机凭什么能卖，不是企业说了算，而是 FDCA 先划线、FDA 按风险分道审批。这篇按「法律底盘 → 药品路径 → 器械路径 → 应急与加速 → 上市后与加州衔接」走，条号钉在每一步上。
- 来源口径：FDCA，21 U.S.C. §§ 301 et seq.；定义 § 321(g)/(h)；IND 21 C.F.R. Part 312；器械报告 21 C.F.R. Part 803；EUA § 564，21 U.S.C. § 360bbb-3；加州 Sherman 法，Cal. Health & Safety Code §§ 109875 et seq.（提纲 §§ 109600 起经核不合，正文按核正条号写）。产品分类与状态以 FDA 当期数据库为准。

---

## 一、法律底盘：FDCA、三个中心与药械的定义线

### 中文

底盘是 1938 年的 FDCA，现编在 21 U.S.C. §§ 301 et seq.，FDA 按产品分工：药品评价与研究中心（CDER）管大多数小分子药，生物制品中心（CBER）管疫苗、血液制品与多数生物制品，器械与放射健康中心（CDRH）管医疗器械。分界看定义：§ 321(g) 的「药」指用于疾病诊断、治愈、缓解、治疗或预防，或意图影响人体结构与功能的物品；§ 321(h) 的「器械」可用于类似目的，但不靠体内化学作用、也不靠被代谢来实现主要作用——这句区别决定许多产品归 CDER 还是 CDRH。审批之外还有执法底盘：§ 331 列禁止行为（如州际运送掺假或错误标识产品），§ 351 定义「掺假」（adulterated，如生产质量不合规），§ 352 定义「错误标识」（misbranded，如标签虚假误导、缺少警示）。

### English

The foundation is the Federal Food, Drug, and Cosmetic Act of 1938, at 21 U.S.C. sections 301 et seq., enforced by FDA product centers: CDER for most small-molecule drugs, CBER for vaccines, blood products, and most biologics, and CDRH for medical devices. Classification turns on the definitions. A drug under section 321(g) is an article intended to diagnose, cure, mitigate, treat, or prevent disease, or to affect the structure or function of the body. A device under section 321(h) may serve similar purposes but does not achieve its primary purpose through chemical action in or on the body and is not dependent on being metabolized — the watershed that sends many products to CDER rather than CDRH. Beyond premarket review, section 331 lists prohibited acts such as shipping adulterated or misbranded products in interstate commerce, section 351 defines adulteration, and section 352 defines misbranding.

### Español (译稿)

La base es la FDCA de 1938, en 21 U.S.C. §§ 301 y ss., aplicada por centros de la FDA: el CDER para la mayoría de los fármacos de molécula pequeña, el CBER para vacunas, productos sanguíneos y la mayoría de los biológicos, y el CDRH para los dispositivos médicos. La clasificación depende de las definiciones. Un medicamento, según el § 321(g), es un artículo destinado a diagnosticar, curar, mitigar, tratar o prevenir enfermedades, o a afectar la estructura o función del cuerpo. Un dispositivo, según el § 321(h), puede perseguir fines parecidos, pero no logra su propósito principal mediante acción química en o sobre el cuerpo ni depende de ser metabolizado; esa frase envía muchos productos al CDER y no al CDRH. Más allá de la revisión previa, el § 331 enumera actos prohibidos, como enviar productos adulterados o mal etiquetados en el comercio interestatal; el § 351 define la adulteración; y el § 352 define el etiquetado indebido, incluidas las afirmaciones falsas o engañosas. (Traducción de estudio, pendiente de revisión nativa.)

### 한국어 (초역·교정 대기)

바탕은 1938년 FDCA로, 21 U.S.C. §§ 301 이하에 편찬되어 있고 FDA가 제품별 센터로 집행합니다. 대부분의 소분자 의약품은 CDER, 백신·혈액제제와 대부분의 생물의약품은 CBER, 의료기기는 CDRH가 맡습니다. 분류는 정의에 달려 있습니다. § 321(g)의 약물은 질병의 진단·치유·완화·치료·예방에 쓰이거나 인체의 구조·기능에 영향을 주도록 의도된 물품입니다. § 321(h)의 기기는 비슷한 목적을 가질 수 있지만 체내·체표의 화학작용으로 주요 목적을 달성하지 않고 대사에 의존하지도 않습니다. 이 문장이 많은 제품을 CDRH가 아닌 CDER로 보내는 분수령이며. 시판 전 심사 너머의 집행 바탕도 있습니다. § 331은 불량하거나 허위표시된 제품의 주간 운송 같은 금지행위를, § 351은 제조 품질 미준수를 포함한 불량의 정의를, § 352는 거짓·오해성 표시를 포함한 허위표시의 정의를 정합니다. (학습용 초역으로, 원어민 교정이 필요합니다.)

### Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

Nền tảng là FDCA năm 1938, tại 21 U.S.C. §§ 301 trở đi, do FDA thực thi qua các trung tâm: CDER đối với hầu hết thuốc phân tử nhỏ, CBER đối với vắc-xin, chế phẩm máu và đa số chế phẩm sinh học, và CDRH đối với thiết bị y tế. Việc phân loại xoay quanh định nghĩa. Thuốc theo § 321(g) là vật phẩm nhằm chẩn đoán, chữa khỏi, làm giảm, điều trị hoặc phòng bệnh, hoặc nhằm tác động tới cấu trúc hay chức năng cơ thể. Thiết bị theo § 321(h) có thể phục vụ mục đích tương tự nhưng không đạt mục đích chính bằng tác dụng hóa học trong hoặc trên cơ thể và không phụ thuộc vào việc bị chuyển hóa; câu đó khiến nhiều sản phẩm đi về CDER thay vì CDRH. Ngoài xét duyệt trước khi bán, § 331 liệt kê hành vi bị cấm như vận chuyển sản phẩm bị pha tạp hoặc ghi nhãn sai trong thương mại liên bang; § 351 định nghĩa pha tạp, bao gồm sản xuất không tuân thủ; và § 352 định nghĩa ghi nhãn sai, bao gồm nhãn giả dối, gây hiểu lầm. (Bản dịch học tập sơ bộ, chờ người bản ngữ hiệu đính.)

### हिन्दी (प्रारंभिक अनुवाद, समीक्षा लंबित)

आधार 1938 का FDCA है, जो 21 U.S.C. §§ 301 आगे में है और FDA उत्पाद-केंद्रों से लागू करता है: अधिकांश लघु-अणु दवाओं के लिए CDER, टीकों, रक्त उत्पादों व अधिकांश जैविक उत्पादों के लिए CBER, और चिकित्सा उपकरणों के लिए CDRH. वर्गीकरण परिभाषाओं पर टिका है. § 321(g) की दवा वह वस्तु है जो रोग के निदान, उपचार, शमन, चिकित्सा या रोकथाम के लिए, या शरीर की संरचना या कार्य को प्रभावित करने के लिए आशयित हो. § 321(h) का उपकरण समान उद्देश्यों के लिए हो सकता है, किंतु अपना मुख्य उद्देश्य शरीर में या पर रासायनिक क्रिया से प्राप्त नहीं करता और चयापचय पर निर्भर नहीं होता — यही विभाजन-रेखा कई उत्पादों को CDRH के बजाय CDER भेजती है. बाज़ार-पूर्व समीक्षा के परे, § 331 निषिद्ध कृत्य गिनाता है जैसे अपमिश्रित या मिथ्या-चिह्नित उत्पादों को अंतर्राज्यीय वाणिज्य में भेजना; § 351 अपमिश्रण की परिभाषा देता है, जिसमें अनुपालनहीन निर्माण भी है; और § 352 मिथ्या-चिह्नन की परिभाषा देता है, जिसमें झूठा या भ्रामक लेबल भी है. (अध्ययन हेतु प्रारंभिक अनुवाद, मूलभाषी समीक्षा लंबित है।)

---

## 二、药品路径：从 IND 三期临床到 NDA、ANDA 与 505(b)(2)

### 中文

新药第一次在美国人身上试验，先过研究用新药申请（IND），依据 § 505(i)，21 U.S.C. § 355(i)，细则在 21 C.F.R. Part 312：申办方交临床前数据与方案，FDA 在 30 天内不叫停（clinical hold）才能启动。临床通常分三期：一期小样本看安全与剂量，二期看初步疗效与副作用，三期大样本随机对照确证。确证后走新药申请（NDA），依据 § 505(b)，21 U.S.C. § 355(b)，FDA 判断药是否安全、在标注用途下是否有效、生产是否可控。仿制药走简略申请（ANDA），依据 § 505(j)：不重做完整临床，而是证明与参比药药学等效、生物等效（bioequivalence）。这条通道是 1984 年 Hatch-Waxman 法搭的交换：仿制药可搭原研数据之桥，原研可获专利期恢复等补偿；第一个成功挑战专利并获批的首仿药可享 180 天市场独占期，但有触发与丧失条件，不能写成无条件垄断。介于两者之间还有 § 505(b)(2)：部分依赖已发表文献或他人已批药数据、自有部分补桥接研究。

### English

A new drug's first test in people requires an Investigational New Drug application (IND) under section 505(i), 21 U.S.C. section 355(i), at 21 C.F.R. Part 312: the sponsor files preclinical data and a protocol, and the study may proceed if FDA imposes no clinical hold within 30 days. Development usually runs in three phases — phase 1 for safety and dose, phase 2 for early efficacy and side effects, phase 3 for large randomized confirmation. Confirmation leads to a New Drug Application (NDA) under section 505(b), 21 U.S.C. section 355(b), where FDA asks whether the drug is safe, effective for its labeled use, and made under control. Generics use the Abbreviated NDA (ANDA) under section 505(j), showing pharmaceutical equivalence and bioequivalence to the reference drug instead of repeating full trials. That bridge was built by the Hatch-Waxman Act of 1984: generics may rely on the innovator record, innovators receive patent-term restoration, and the first generic to successfully challenge a patent and win approval may earn 180 days of market exclusivity, subject to triggering and forfeiture rules. Section 505(b)(2) sits in between, relying in part on published literature or another approved drug plus bridging studies.

### Español (译稿)

La primera prueba de un fármaco nuevo en personas exige la solicitud IND del § 505(i), 21 U.S.C. § 355(i), en 21 C.F.R. Part 312: el promotor presenta datos preclínicos y un protocolo, y el estudio puede avanzar si la FDA no lo suspende (clinical hold) en 30 días. El desarrollo suele correr en tres fases — fase 1 de seguridad y dosis, fase 2 de eficacia preliminar y efectos adversos, fase 3 de confirmación aleatorizada y amplia. La confirmación lleva a la NDA del § 505(b), 21 U.S.C. § 355(b), donde la FDA valora si el fármaco es seguro, eficaz para el uso etiquetado y fabricado bajo control. Los genéricos usan la ANDA del § 505(j), demostrando equivalencia farmacéutica y bioequivalencia frente al fármaco de referencia en lugar de repetir los ensayos. Ese puente lo construyó la Ley Hatch-Waxman de 1984: el genérico puede apoyarse en el expediente del innovador, el innovador recibe restauración del plazo de patente, y el primer genérico que impugna con éxito una patente y logra aprobación puede obtener 180 días de exclusividad, sujetos a reglas de activación y pérdida. El § 505(b)(2) queda en medio, apoyándose en parte en literatura publicada o en otro fármaco aprobado, con estudios puente propios. (Traducción de estudio, pendiente de revisión nativa.)

### 한국어 (초역·교정 대기)

신약을 사람에게 처음 시험하려면 § 505(i), 21 U.S.C. § 355(i)에 근거하고 21 C.F.R. Part 312로 시행되는 IND가 필요합니다. 스폰서가 전임상 자료와 계획서를 내고 FDA가 30일 안에 임상보류(clinical hold)를 걸지 않으면 시작할 수 있습니다. 개발은 보통 3단계입니다. 1상은 안전성과 용량, 2상은 초기 유효성과 부작용, 3상은 대규모 무작위 확증입니다. 확증 뒤에는 § 505(b), 21 U.S.C. § 355(b)의 NDA로 가며, FDA는 약이 안전한지, 표시 용도에 유효한지, 통제 아래 제조되는지를 봅니다. 제네릭은 § 505(j)의 ANDA를 써서 전체 임상을 반복하는 대신 대조약과의 약학적 동등성과 생물학적 동등성을 보입니다. 이 다리는 1984년 Hatch-Waxman법이 만든 교환으로, 제네릭은 오리지널 자료에 기대고 오리지널은 특허기간 회복을 받으며, 특허 도전에 성공해 처음 승인된 제네릭은 180일 시장독점권을 얻을 수 있으나 개시·상실 요건이 따릅니다. 그 사이에는 § 505(b)(2)가 있어, 발표 문헌이나 타 승인약 자료에 일부 기대고 자체 가교 연구를 더합니다. (학습용 초역으로, 원어민 교정이 필요합니다.)

### Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

Lần thử đầu tiên của thuốc mới trên người cần hồ sơ IND theo § 505(i), 21 U.S.C. § 355(i), tại 21 C.F.R. Part 312: nhà tài trợ nộp dữ liệu tiền lâm sàng và đề cương, và nghiên cứu có thể tiến hành nếu FDA không ra lệnh tạm dừng lâm sàng (clinical hold) trong 30 ngày. Phát triển thường chạy ba giai đoạn — giai đoạn 1 về an toàn và liều, giai đoạn 2 về hiệu quả sơ bộ và tác dụng phụ, giai đoạn 3 là xác nhận ngẫu nhiên quy mô lớn. Sau xác nhận là NDA theo § 505(b), 21 U.S.C. § 355(b), nơi FDA xét thuốc có an toàn, hiệu quả cho công dụng ghi nhãn và được sản xuất dưới kiểm soát hay không. Thuốc generic dùng ANDA theo § 505(j), chứng minh tương đương dược học và tương đương sinh học với thuốc tham chiếu thay vì lặp lại toàn bộ thử nghiệm. Cây cầu đó do Đạo luật Hatch-Waxman năm 1984 dựng nên: generic dựa vào hồ sơ của nhà sáng chế, nhà sáng chế nhận khôi phục thời hạn bằng sáng chế, và generic đầu tiên thách thức thành công bằng sáng chế và được duyệt có thể nhận 180 ngày độc quyền thị trường, với quy tắc kích hoạt và mất quyền đi kèm. § 505(b)(2) nằm ở giữa, dựa một phần vào tài liệu đã công bố hoặc thuốc khác đã duyệt, cộng nghiên cứu bắc cầu. (Bản dịch học tập sơ bộ, chờ người bản ngữ hiệu đính.)

### हिन्दी (प्रारंभिक अनुवाद, समीक्षा लंबित)

नई दवा की मनुष्यों पर पहली जाँच के लिए § 505(i), 21 U.S.C. § 355(i), के तहत IND चाहिए, जो 21 C.F.R. Part 312 में है: प्रायोजक पूर्व-नैदानिक आँकड़े व प्रोटोकॉल देता है, और यदि FDA 30 दिनों में clinical hold न लगाए तो अध्ययन शुरू हो सकता है. विकास सामान्यतः तीन चरणों में चलता है — चरण 1 सुरक्षा व ख़ुराक, चरण 2 प्रारंभिक प्रभावकारिता व दुष्प्रभाव, चरण 3 बड़ा यादृच्छिक पुष्टिकरण. पुष्टि के बाद § 505(b), 21 U.S.C. § 355(b), के तहत NDA आता है, जहाँ FDA देखता है कि दवा सुरक्षित है, लेबल किए उपयोग के लिए प्रभावी है और नियंत्रण में बनती है या नहीं. जेनेरिक § 505(j) के ANDA का उपयोग करते हैं और पूरे परीक्षण दोहराने के बजाय संदर्भ दवा से औषधीय समानता व जैव-समतुल्यता दिखाते हैं. यह सेतु 1984 के Hatch-Waxman अधिनियम ने बनाया: जेनेरिक नवप्रवर्तक के अभिलेख पर निर्भर रह सकता है, नवप्रवर्तक को पेटेंट-अवधि पुनर्स्थापना मिलती है, और पेटेंट को सफलतापूर्वक चुनौती देकर स्वीकृति पाने वाला पहला जेनेरिक 180 दिनों की बाज़ार-अनन्यता पा सकता है, जो सक्रियण व ज़ब्ती नियमों के अधीन है. बीच में § 505(b)(2) है, जो आंशिक रूप से प्रकाशित साहित्य या अन्य स्वीकृत दवा पर निर्भर करता है और अपने सेतु-अध्ययन जोड़ता है. (अध्ययन हेतु प्रारंभिक अनुवाद, मूलभाषी समीक्षा लंबित है।)

---

## 三、器械路径：按风险分三类，510(k)、De Novo 与 PMA 三条道

### 中文

器械先按风险分级，依据 § 513，21 U.S.C. § 360c：I 类低风险，受一般控制、不少豁免上市前通知；II 类中风险，需特殊控制，通常走 510(k)；III 类高风险，支撑生命或风险不合理时走最严路径。510(k) 本身在 § 510(k)，21 U.S.C. § 360(k)，是上市前通知，核心标准是实质等同（substantial equivalence，定义在 § 513(i)）：与已合法上市的谓词器械（predicate）预期用途相同，技术特征相同，或不同但不提出新的安全有效性问题且证明一样安全有效——其结果叫「放行」（clearance），不是「批准」。全新、低到中风险又无谓词的器械走 De Novo，依据 § 513(f)(2)，FDA 直接为它新建分类，III 类等高风险产品走上市前批准（PMA），依据 § 515，21 U.S.C. § 360e，标准是「合理保证安全有效」（reasonable assurance of safety and effectiveness）。

### English

Devices are first graded by risk under section 513, 21 U.S.C. section 360c: Class I low risk, under general controls and often exempt from premarket notification; Class II moderate risk, requiring special controls and usually a 510(k); Class III high risk, such as implantable pacemakers, where the device sustains life or presents unreasonable risk. The 510(k) itself sits in section 510(k), 21 U.S.C. section 360(k): a premarket notification whose test is substantial equivalence, defined in section 513(i) — the same intended use as a legally marketed predicate, and either the same technological characteristics or different ones that raise no new safety or effectiveness questions and are shown to be as safe and effective. Its outcome is clearance, not approval. A novel low-to-moderate-risk device with no predicate uses De Novo under section 513(f)(2); FDA creates a new classification. Class III and similar high-risk products need Premarket Approval (PMA) under section 515, 21 U.S.C. section 360e, showing reasonable assurance of safety and effectiveness.

### Español (译稿)

Los dispositivos se gradúan primero por riesgo según el § 513, 21 U.S.C. § 360c: clase I de riesgo bajo, con controles generales y a menudo exenta de notificación previa; clase II de riesgo moderado, con controles especiales y normalmente un 510(k); clase III de riesgo alto, cuando el dispositivo sostiene la vida o presenta un riesgo no razonable. El 510(k) está en el propio § 510(k), 21 U.S.C. § 360(k): una notificación previa cuyo criterio es la equivalencia sustancial, definida en el § 513(i) — mismo uso previsto que un predicado legalmente comercializado, y mismas características tecnológicas, o distintas que no planteen nuevas preguntas de seguridad y eficacia y se demuestren tan seguras y eficaces. Su resultado es clearance, no aprobación. Un dispositivo nuevo de riesgo bajo a moderado y sin predicado usa De Novo, § 513(f)(2); la FDA crea una clasificación nueva. La clase III y productos parecidos exigen PMA según el § 515, 21 U.S.C. § 360e, demostrando garantía razonable de seguridad y eficacia. (Traducción de estudio, pendiente de revisión nativa.)

### 한국어 (초역·교정 대기)

기기는 먼저 § 513, 21 U.S.C. § 360c에 따라 위험도로 나뉩니다. I등급은 저위험으로 일반 통제를 받고 통지가 면제되는 경우가 많고, II등급은 중위험으로 특별 통제와 보통 510(k)가 필요하며, III등급은 이식형 심박조율기 같은 고위험입니다. 510(k) 자체는 § 510(k), 21 U.S.C. § 360(k)에 있는 시판 전 통지이며, 기준은 § 513(i)가 정의한 실질적 동등성입니다. 합법적으로 시판된 비교기기(predicate)와 용도가 같고, 기술적 특성이 같거나, 다르더라도 안전성·유효성에 새로운 문제를 제기하지 않으며 그만큼 안전하고 유효함을 보여야 합니다. 결과는 승인이 아니라 허가(clearance)입니다. 비교기기가 없는 신규 저·중위험 기기는 § 513(f)(2)의 De Novo를 써서 FDA가 새 분류를 만듭니다. III등급 등 고위험 제품은 § 515, 21 U.S.C. § 360e의 PMA가 필요하고, 보통 임상 자료와 함께 안전성·유효성에 대한 합리적 보증을 보여야 합니다. (학습용 초역으로, 원어민 교정이 필요합니다.)

### Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

Thiết bị trước hết được phân cấp theo rủi ro theo § 513, 21 U.S.C. § 360c: Loại I rủi ro thấp, chịu kiểm soát chung và thường được miễn thông báo; Loại II rủi ro trung bình, đòi hỏi kiểm soát đặc biệt và thường đi qua 510(k); Loại III rủi ro cao, như máy tạo nhịp cấy ghép, khi thiết bị duy trì sự sống hoặc tạo rủi ro không hợp lý. Bản thân 510(k) nằm ở § 510(k), 21 U.S.C. § 360(k): một thông báo trước khi bán mà tiêu chuẩn là tương đương đáng kể, định nghĩa tại § 513(i) — cùng công dụng dự kiến với một tiền lệ đã bán hợp pháp, và đặc tính công nghệ giống hệt, hoặc khác nhưng không đặt ra câu hỏi mới về an toàn và hiệu quả và được chứng minh an toàn, hiệu quả như tiền lệ. Kết quả của nó gọi là clearance, không phải approval. Một thiết bị mới, rủi ro thấp tới trung bình và không có tiền lệ thì dùng De Novo theo § 513(f)(2); FDA tạo phân loại mới. Loại III và các sản phẩm tương tự cần PMA theo § 515, 21 U.S.C. § 360e, chứng minh bảo đảm hợp lý về an toàn và hiệu quả. (Bản dịch học tập sơ bộ, chờ người bản ngữ hiệu đính.)

### हिन्दी (प्रारंभिक अनुवाद, समीक्षा लंबित)

उपकरण पहले § 513, 21 U.S.C. § 360c, के तहत जोखिम से वर्गीकृत होते हैं: वर्ग I निम्न जोखिम, सामान्य नियंत्रणों में और अक्सर सूचना से मुक्त; वर्ग II मध्यम जोखिम, जिनमें विशेष नियंत्रण और सामान्यतः 510(k) चाहिए; वर्ग III उच्च जोखिम, जैसे आरोप्य पेसमेकर. 510(k) स्वयं § 510(k), 21 U.S.C. § 360(k), में है: यह बाज़ार-पूर्व सूचना है जिसका मानक § 513(i) में परिभाषित सारभूत समानता है — कानूनी रूप से बिके predicate जैसा ही आशयित उपयोग, और या तो समान तकनीकी विशेषताएँ, या भिन्न विशेषताएँ जो सुरक्षा व प्रभावकारिता के नए प्रश्न न उठाएँ और उतनी ही सुरक्षित व प्रभावी सिद्ध हों. इसका परिणाम approval नहीं, clearance कहलाता है. कोई नया निम्न-मध्यम जोखिम उपकरण जिसका कोई predicate न हो, § 513(f)(2) के De Novo का प्रयोग करता है; FDA नया वर्गीकरण बनाती है. वर्ग III व समान उत्पादों को § 515, 21 U.S.C. § 360e, के तहत PMA चाहिए, जिसमें सुरक्षा व प्रभावकारिता का युक्तियुक्त आश्वासन सामान्यतः नैदानिक आँकड़ों से दिखाना होता है. (अध्ययन हेतु प्रारंभिक अनुवाद, मूलभाषी समीक्षा लंबित है।)

---

## 四、应急与加速通道：EUA 不是正式批准，加速项目也不是免检

### 中文

紧急状态下有一条窄门：紧急使用授权（EUA），依据 § 564，21 U.S.C. § 360bbb-3。卫生与公众服务部部长先发紧急声明，FDA 再判断病原体可致严重或危及生命的疾病、综合证据显示产品「可能有效」（may be effective）、获益超过风险、且无足够可得的已批准替代品。may be effective 的门槛低于正式批准的「有效」，EUA 是绑定紧急状态的临时授权，可被撤销，不等于 NDA 或 PMA 批准。非紧急情形另有加速带：药品的快速通道（Fast Track）、突破性疗法，器械的突破性器械计划（Breakthrough Devices Program），换的是更早更密的沟通与滚动、优先审评，不是删掉安全有效标准。

### English

Emergencies open a narrow door: Emergency Use Authorization (EUA) under section 564, 21 U.S.C. section 360bbb-3. The Secretary of Health and Human Services first issues an emergency declaration; FDA then asks whether the agent can cause a serious or life-threatening disease, whether the evidence shows the product may be effective, whether benefits outweigh risks, and whether no adequate, approved, and available alternative exists. May be effective is a lower bar than full approval, and an EUA is temporary and revocable — not an NDA or PMA approval. Outside emergencies, Fast Track and Breakthrough Therapy for drugs and the Breakthrough Devices Program for devices offer earlier interaction and rolling or priority review: speed, not lower standards.

### Español (译稿)

Las emergencias abren una puerta estrecha: la EUA del § 564, 21 U.S.C. § 360bbb-3. El Secretario de Salud y Servicios Humanos emite primero la declaración de emergencia; luego la FDA valora si el agente puede causar una enfermedad grave o mortal, si la evidencia muestra que el producto puede ser eficaz (may be effective), si los beneficios superan los riesgos y si no hay una alternativa adecuada, aprobada y disponible. May be effective es un listón más bajo que la aprobación plena, y una EUA es temporal y revocable, no una aprobación NDA ni PMA. Fuera de emergencias, Fast Track y Breakthrough Therapy en fármacos y el Breakthrough Devices Program en dispositivos ofrecen interacción más temprana y revisión continua o prioritaria: velocidad, no estándares más bajos. (Traducción de estudio, pendiente de revisión nativa.)

### 한국어 (초역·교정 대기)

비상사태에서는 § 564, 21 U.S.C. § 360bbb-3의 긴급사용승인(EUA)이라는 좁은 문이 열립니다. 먼저 보건복지부 장관이 비상 선언을 내고, FDA는 병원이 심각한 질병을 일으킬 수 있는지, 제품이 효과가 있을 수 있는지(may be effective), 이익이 위험을 초과하는지, 적절한 승인 대안이 없는지를 판단합니다. may be effective는 정식 승인보다 낮은 문턱이며, EUA는 임시적이고 철회 가능해 NDA나 PMA 승인이 아닙니다. 비상이 아닌 경우 약의 Fast Track·Breakthrough Therapy와 기기의 Breakthrough Devices Program은 이른 소통과 순차·우선 심사를 제공할 뿐, 기준을 낮추지 않습니다. (학습용 초역으로, 원어민 교정이 필요합니다.)

### Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

Khẩn cấp mở ra một cửa hẹp: EUA theo § 564, 21 U.S.C. § 360bbb-3. Bộ trưởng Bộ Y tế và Dịch vụ Nhân sinh ban hành tuyên bố khẩn cấp trước; FDA sau đó xét tác nhân có thể gây bệnh nghiêm trọng hoặc đe dọa tính mạng không, bằng chứng có cho thấy sản phẩm có thể có hiệu quả (may be effective) không, lợi ích có vượt rủi ro không, và có giải pháp thay thế phù hợp, đã duyệt và sẵn có hay không. May be effective là ngưỡng thấp hơn phê duyệt đầy đủ, và EUA là tạm thời, có thể thu hồi, không phải phê duyệt NDA hay PMA. Ngoài khẩn cấp, Fast Track và Breakthrough Therapy cho thuốc và Breakthrough Devices Program cho thiết bị mang lại tương tác sớm hơn và xét duyệt cuốn chiếu hoặc ưu tiên: tốc độ, không phải tiêu chuẩn thấp hơn. (Bản dịch học tập sơ bộ, chờ người bản ngữ hiệu đính.)

### हिन्दी (प्रारंभिक अनुवाद, समीक्षा लंबित)

आपात में § 564, 21 U.S.C. § 360bbb-3, के तहत EUA का संकरा द्वार खुलता है. पहले स्वास्थ्य सचिव आपात घोषणा जारी करता है; फिर FDA देखता है कि कारक गंभीर या जानलेवा रोग कर सकता है या नहीं, उत्पाद प्रभावी हो सकता है (may be effective) या नहीं, लाभ जोखिमों से अधिक हैं या नहीं, और कोई पर्याप्त स्वीकृत विकल्प नहीं है या नहीं. May be effective पूर्ण स्वीकृति से निम्न स्तर है, और EUA अस्थायी व निरस्त-योग्य है, NDA या PMA स्वीकृति नहीं. आपात से बाहर दवाओं के Fast Track व Breakthrough Therapy और उपकरणों का Breakthrough Devices Program पहले संपर्क और rolling या priority review देते हैं: गति, निम्न मानक नहीं. (अध्ययन हेतु प्रारंभिक अनुवाद, मूलभाषी समीक्षा लंबित है।)

---

## 五、上市后监管：不良事件报告、召回的自愿与强制之分、加州衔接

### 中文

批准不是终点。上市后各方通过 MedWatch 报告不良事件，企业义务更硬：器械制造商与进口商按 MDR（21 C.F.R. Part 803）报告器械相关的死亡、严重伤害与可报告故障，制造商一般在获悉后 30 个日历日内提交、某些需立即补救的情形为 5 个工作日；使用机构向 FDA 或制造商报告死亡与严重伤害。报告是信号，不等于已证明因果。召回分自愿与强制：绝大多数由企业在 21 C.F.R. Part 7 下自愿发起；FDA 对一般药品没有普遍的强制召回权，药品召回通常靠企业配合、辅以扣押与禁令，特定品类的法定授权除外。食品则不同，FSMA 加入的 § 423 给了强制召回权。器械有明文强制通道：§ 518(e)，21 U.S.C. § 360h(e)，与 21 C.F.R. Part 810——FDA 认定器械有合理可能造成严重不良后果或死亡时，可命停止分销与通知、给予听证机会，再命召回。加州方面，在州内生产药品或器械还须按 Sherman 法（Health & Safety Code §§ 109875 et seq.）向 CDPH Food and Drug Branch 领制造许可并接受检查；

### English

Approval is not the end. Adverse events are reported through MedWatch, and firm duties are stricter: device manufacturers and importers report device-related deaths, serious injuries, and reportable malfunctions under MDR, 21 C.F.R. Part 803 — generally within 30 calendar days for manufacturers, and 5 work days for certain events needing remedial action — while user facilities report deaths and serious injuries to FDA or the manufacturer. A report is a signal, not proof of causation. Most recalls are firm-initiated voluntarily under 21 C.F.R. Part 7. FDA has no general mandatory recall authority over ordinary drugs, where recalls usually depend on firm cooperation backed by seizure and injunction, apart from specific authorities for particular categories. For foods, section 423, added by FSMA, does grant mandatory authority. For devices, section 518(e), 21 U.S.C. section 360h(e), and 21 C.F.R. Part 810 allow FDA, on finding a reasonable probability of serious adverse consequences or death, to order distribution stopped and notice given, allow a hearing, and then order a recall. In California, in-state manufacturing also requires a license from the CDPH Food and Drug Branch under the Sherman Law, Health & Safety Code sections 109875 et seq., plus inspection.

### Español (译稿)

La aprobación no es el final. Los eventos adversos se informan por MedWatch, y los deberes de la empresa son más estrictos: fabricantes e importadores de dispositivos informan muertes, lesiones graves y fallos notificables conforme al MDR, 21 C.F.R. Part 803 — en general en 30 días naturales para el fabricante, y en 5 días laborables para ciertos eventos que exigen acción correctiva — mientras los centros usuarios informan muertes y lesiones graves a la FDA o al fabricante. Un informe es una señal, no prueba de causalidad. La mayoría de los retiros son voluntarios, iniciados por la empresa bajo 21 C.F.R. Part 7. La FDA no tiene una facultad general de retiro obligatorio sobre los medicamentos ordinarios, donde el retiro suele depender de la cooperación de la empresa respaldada por incautación y órdenes judiciales, salvo autoridades específicas. Para los alimentos, el § 423, añadido por la FSMA, sí concede facultad obligatoria. Para los dispositivos, el § 518(e), 21 U.S.C. § 360h(e), y 21 C.F.R. Part 810 permiten a la FDA, hallada una probabilidad razonable de consecuencias graves o muerte, ordenar el cese de la distribución y la notificación, dar audiencia y después ordenar el retiro. En California, fabricar en el estado exige además licencia de la Food and Drug Branch del CDPH conforme a la Ley Sherman, Health & Safety Code §§ 109875 y ss., más inspección. (Traducción de estudio, pendiente de revisión nativa.)

### 한국어 (초역·교정 대기)

승인은 끝이 아닙니다. 이상사례는 MedWatch로 보고되며 기업 의무가 더 엄격합니다. 기기 제조업자와 수입업자는 MDR(21 C.F.R. Part 803)에 따라 기기 관련 사망, 중대한 상해, 보고 대상 오작동을 보고하는데, 제조업자는 원칙적으로 30일 이내, 즉각 시정이 필요한 일부 사건은 5영업일 이내이며, 사용 기관은 사망과 중대한 상해를 FDA나 제조업자에게 보고합니다. 보고는 신호일 뿐 인과관계의 증명은 아닙니다. 대부분 리콜은 21 C.F.R. Part 7 아래 기업이 자발적으로 시작합니다. FDA는 일반 의약품에 대한 보편적 강제 리콜 권한이 없어, 의약품 리콜은 보통 압류·금지명령으로 뒷받침되는 기업 협조에 의존하고, 특정 범주의 개별 권한은 별개입니다. 식품에는 FSMA가 추가한 § 423이 강제 권한을 줍니다. 기기에는 § 518(e), 21 U.S.C. § 360h(e)와 21 C.F.R. Part 810이 있어, 심각한 위해나 사망의 합리적 가능성이 있으면 FDA는 유통 중단과 통지를 명하고 청문 기회를 준 뒤 리콜을 명할 수 있습니다. 캘리포니아에서 주 내 제조를 하려면 Sherman법(Health & Safety Code §§ 109875 이하)에 따라 CDPH Food and Drug Branch의 면허와 검사도 필요합니다. (학습용 초역으로, 원어민 교정이 필요합니다.)

### Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

Phê duyệt không phải điểm kết thúc. Biến cố bất lợi được báo cáo qua MedWatch, và nghĩa vụ của doanh nghiệp chặt hơn: nhà sản xuất và nhà nhập khẩu thiết bị báo cáo tử vong, tổn thương nghiêm trọng và trục trặc phải báo cáo theo MDR, 21 C.F.R. Part 803 — thường trong 30 ngày lịch đối với nhà sản xuất, và 5 ngày làm việc đối với một số sự kiện cần khắc phục ngay — trong khi cơ sở sử dụng báo cáo tử vong và tổn thương nghiêm trọng cho FDA hoặc nhà sản xuất. Một báo cáo là tín hiệu, không phải bằng chứng nhân quả. Đa số thu hồi do doanh nghiệp tự khởi xướng theo 21 C.F.R. Part 7. FDA không có thẩm quyền thu hồi bắt buộc chung đối với thuốc thông thường, nơi thu hồi thường dựa vào hợp tác của doanh nghiệp, được hỗ trợ bởi tịch thu và lệnh cấm, ngoài thẩm quyền riêng cho từng nhóm. Với thực phẩm, § 423 do FSMA bổ sung có trao thẩm quyền bắt buộc. Với thiết bị, § 518(e), 21 U.S.C. § 360h(e), và 21 C.F.R. Part 810 cho phép FDA, khi thấy khả năng hợp lý gây hậu quả nghiêm trọng hoặc tử vong, ra lệnh ngừng phân phối và thông báo, cho cơ hội điều trần, rồi ra lệnh thu hồi. Ở California, sản xuất trong bang còn cần giấy phép của Food and Drug Branch thuộc CDPH theo Luật Sherman, Health & Safety Code §§ 109875 trở đi, cộng thanh tra. (Bản dịch học tập sơ bộ, chờ người bản ngữ hiệu đính.)

### हिन्दी (प्रारंभिक अनुवाद, समीक्षा लंबित)

स्वीकृति अंत नहीं है. प्रतिकूल घटनाएँ MedWatch से रिपोर्ट होती हैं, और कंपनी के कर्तव्य अधिक कड़े हैं: उपकरण निर्माता व आयातक MDR, 21 C.F.R. Part 803, के तहत उपकरण-संबंधी मृत्यु, गंभीर चोट व रिपोर्ट-योग्य ख़राबियाँ रिपोर्ट करते हैं — निर्माताओं के लिए सामान्यतः 30 कैलेंडर दिनों में, और कुछ घटनाओं में 5 कार्य-दिवसों में — जबकि उपयोगकर्ता सुविधाएँ मृत्यु व गंभीर चोट FDA या निर्माता को रिपोर्ट करती हैं. रिपोर्ट एक संकेत है, कारणता का प्रमाण नहीं. अधिकांश रिकॉल 21 C.F.R. Part 7 के तहत कंपनी स्वयं शुरू करती है. FDA के पास साधारण दवाओं पर सामान्य अनिवार्य रिकॉल अधिकार नहीं है, वहाँ रिकॉल सामान्यतः कंपनी के सहयोग पर निर्भर रहता है, जिसे ज़ब्ती व निषेधाज्ञा का समर्थन मिलता है, विशिष्ट श्रेणियों के अधिकार अलग हैं. खाद्य पदार्थों के लिए FSMA द्वारा जोड़ा गया § 423 अनिवार्य अधिकार देता है. उपकरणों के लिए § 518(e), 21 U.S.C. § 360h(e), व 21 C.F.R. Part 810 स्पष्ट मार्ग देते हैं: गंभीर परिणाम या मृत्यु की युक्तियुक्त संभावना मिलने पर FDA वितरण रोकने व सूचना का आदेश दे सकता है, सुनवाई का अवसर दे सकता है, और फिर रिकॉल का आदेश दे सकता है. California में राज्य के भीतर निर्माण के लिए Sherman Law, Health & Safety Code §§ 109875 आगे, के तहत CDPH Food and Drug Branch से लाइसेंस और निरीक्षण भी चाहिए. (अध्ययन हेतु प्रारंभिक अनुवाद, मूलभाषी समीक्षा लंबित है।)

---

## 参考依据

- FDCA, 21 U.S.C. §§ 301 et seq.；定义 § 321(g)/(h)；禁止行为 § 331；掺假 § 351；错误标识 § 352
- 药品：§ 505(i) IND（21 U.S.C. § 355(i)；21 C.F.R. Part 312）、§ 505(b) NDA、§ 505(j) ANDA、§ 505(b)(2)；Drug Price Competition and Patent Term Restoration Act of 1984（Hatch-Waxman），含 180 天首仿独占框架（§ 505(j)(5)(B)(iv) 一带）
- 器械：§ 513 分级与 § 513(i) 实质等同（21 U.S.C. § 360c）、§ 510(k) 上市前通知（21 U.S.C. § 360(k)）、§ 513(f)(2) De Novo、§ 515 PMA（21 U.S.C. § 360e）
- 应急：§ 564 EUA（21 U.S.C. § 360bbb-3）；加速项目见 FDA 当期说明
- 上市后：21 C.F.R. Part 803（MDR）、21 C.F.R. Part 7（自愿召回）；器械强制召回 § 518(e)（21 U.S.C. § 360h(e)；21 C.F.R. Part 810）；食品强制召回 § 423（21 U.S.C. § 350l，FSMA 加入）
- 加州：Sherman Food, Drug, and Cosmetic Law, Cal. Health & Safety Code §§ 109875 et seq.（Division 104, Part 5，约 §§ 109875–111929.5）。说明：提纲 §§ 109600 et seq. 经核不合现行编纂，正文按核正条号写。

## 免责声明

本篇为个人学习笔记，不构成法律或医疗建议。具体产品请以 FDA 当期决定与法规原文为准；涉及自身用药与器械的问题，请咨询持牌医师或药师。
