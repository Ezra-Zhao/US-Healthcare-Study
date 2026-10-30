# 病历能看能改吗：HIPAA 访问权、修正权与信息阻断规则

> 个人学习笔记，不构成医疗或法律建议。条号以 45 C.F.R. Part 164 与 HHS 官网为准。

## 中文主文

在美国，你的病历法律上「就是你的」吗？答案分两半：纸或文件本身归医疗机构保管，但其中信息你有一组联邦权利——能看、能拿副本、能要求改正、能指定发给第三方。这组权利主要来自 HIPAA 隐私规则（45 C.F.R. Part 164, Subpart E）。

**访问权：30 天内必须给。** § 164.524(a)：个人有权查阅并取得自己在「指定记录集」（designated record set）中的受保护健康信息（PHI）副本。机构一般须在 30 天内提供（§ 164.524(b)(2)），确有困难可书面说明延期一次、不超过 30 天。形式上：机构能以电子方式维护的，须按你要求的电子格式提供（§ 164.524(c)(2)(ii)），比如 PDF 或经患者门户下载。收费有上限：只能收基于人工的合理成本费（reasonable, cost-based fee），HHS 长期立场是纸质与电子副本都不得借此牟利；按页收费对电子记录不成立。

**可以拒绝给的情形很少，且多可复核。** § 164.524(a)(2)–(3) 列举了可拒绝且不可复核（如涉及他人安全、临床试验进行中）与可拒绝但可复核（持牌专业人员判断获取可能危及本人或他人生命安全等）的情形。拒绝必须书面说明理由与复核、投诉路径。

**第三方直送。** § 164.524(c)(3)(ii)：你可以书面明确要求机构把副本直接发给你的指定第三方（如另一位医生、律师或家人）。机构对「患者本人指示的发送」收费同样受成本费上限约束（这一口径经 Ciox Health v. Azar, 435 F. Supp. 3d 30 (D.D.C. 2020) 一案调整：法院撤销了 HHS 把费用上限扩张到第三方记录公司的部分，但患者本人直接索取的上限不变）。

**修正权：能要求改，不保证改成。** § 164.526：你有权要求修正记录集中不准确或不完整的 PHI。机构须在 60 天内答复（可延期 30 天）。机构可以拒绝（例如记录不是它建的、它认为记录准确完整），但必须书面说明理由；你有权提交一份异议声明（statement of disagreement）附入记录，以后披露该记录时一并附上。换句话说：HIPAA 给的是「申请＋留痕」权，不是单方改稿权。

**信息阻断（information blocking）：机构不能无理由拖延电子病历共享。** 《21 世纪治愈法案》§ 4004 落地为 45 C.F.R. Part 171：医疗提供者、健康信息网络与经认证的电子病历厂商，不得实施可能干扰电子健康信息（EHI）访问、交换或使用的行为，除非落入八类法定例外（如隐私保护、防止伤害、不可行等，且每类例外有具体条件）。患者遇到门户迟迟不放检查结果、无理由的拖延，可向 ONC（国家卫生信息技术协调员办公室）提交信息阻断投诉。注意它管的是「阻断行为」，不取代 HIPAA 访问权本身，两条线常并用：一边按 § 164.524 正式索取，一边对拖延投诉。

**加州加层。** 加州《患者访问健康记录法》（Health & Saf. Code §§ 123100 起）给患者查阅与取得副本的权利，且时限更短：查阅一般在 5 个工作日内安排、副本 15 天内提供（§ 123130），收费有法定上限。联邦与州规则并存时，取对患者更有利者。

**实务动作。** 索取时书面注明：记录范围与日期、要的格式（电子 PDF）、依据 § 164.524，并保留提交凭证；30 天未到先书面催告，再向 HHS 民权办公室（OCR）投诉——OCR 投诉是免费且最常用的施压路径。

---

## English

Is your medical record legally "yours" in the United States? The chart itself is kept by the provider, but the HIPAA Privacy Rule (45 C.F.R. Part 164, Subpart E) gives you a set of federal rights over the information: to see it, get a copy, ask for corrections, and direct it to a third party.

**Right of access — within 30 days.** Under § 164.524(a), you may inspect and obtain a copy of your protected health information in a designated record set. The covered entity generally must act within 30 days (§ 164.524(b)(2)), with one written extension of up to 30 more days. If the information is maintained electronically, you may obtain it in the electronic form and format you request (§ 164.524(c)(2)(ii)). Fees are capped at a reasonable, cost-based amount; per-page fees do not apply to electronic records.

**Denials are narrow.** Section 164.524(a)(2)–(3) lists unreviewable and reviewable grounds for denial (for example, a licensed professional's judgment that access could endanger life or safety). Any denial must be written, with reasons and complaint routes.

**Directing a copy to a third party.** Under § 164.524(c)(3)(ii), you may direct the entity in writing to transmit a copy to a person or entity you designate. After Ciox Health v. Azar, 435 F. Supp. 3d 30 (D.D.C. 2020), the rate cap no longer extends to records sent to third-party companies at a company's request, but the cap for an individual's own request is unchanged.

**Right to amend — a right to ask, not to dictate.** Under § 164.526, you may request amendment of inaccurate or incomplete PHI; the entity must respond within 60 days (one 30-day extension) and may deny, but must explain in writing, and you may file a statement of disagreement that travels with the record.

**Information blocking.** Section 4004 of the 21st Century Cures Act, implemented at 45 C.F.R. Part 171, prohibits providers, health information networks, and certified EHR developers from practices likely to interfere with access, exchange, or use of electronic health information, unless one of eight regulatory exceptions applies. Complaints go to ONC.

**California overlay.** The Patient Access to Health Records Act (Health & Saf. Code §§ 123100 et seq.) is faster: inspection generally within 5 working days and copies within 15 days (§ 123130), with statutory fee caps. Where state law is more protective, it controls.

*Personal study notes only; not medical or legal advice.*

---

## Español (初译待校)

¿Su historial médico es legalmente «suyo» en Estados Unidos? El documento lo custodia el proveedor, pero la Regla de Privacidad de HIPAA (45 C.F.R. Parte 164, Subparte E) le otorga derechos federales sobre la información: verla, obtener copia, pedir correcciones y dirigirla a un tercero.

**Acceso: en 30 días.** Según § 164.524(a), usted puede inspeccionar y obtener copia de su información de salud protegida en un conjunto de registros designado. La entidad debe responder en 30 días (§ 164.524(b)(2)), con una prórroga escrita de hasta 30 días más. Si la información se mantiene electrónicamente, puede obtenerla en el formato electrónico solicitado (§ 164.524(c)(2)(ii)). La tarifa está limitada a un costo razonable basado en el trabajo real; no caben cargos por página en registros electrónicos.

**Denegaciones limitadas.** § 164.524(a)(2)–(3) enumera motivos denegables con y sin revisión (por ejemplo, juicio de un profesional con licencia de que el acceso pondría en peligro la vida o la seguridad). Toda denegación debe ser escrita y fundamentada.

**Envío a un tercero.** Según § 164.524(c)(3)(ii), puede ordenar por escrito que la copia se envíe a la persona o entidad que designe. Tras Ciox Health v. Azar, 435 F. Supp. 3d 30 (D.D.C. 2020), el tope tarifario ya no se extiende a envíos pedidos por empresas terceros, pero se mantiene para la solicitud del propio individuo.

**Corrección: derecho a pedir, no a imponer.** Según § 164.526, puede solicitar la corrección de información inexacta o incompleta; la entidad responde en 60 días (con una prórroga de 30) y puede denegar, pero debe explicarlo por escrito, y usted puede presentar una declaración de desacuerdo que acompañará al registro.

**Bloqueo de información.** La sección 4004 de la Ley de Curas del Siglo XXI, en 45 C.F.R. Parte 171, prohíbe a proveedores, redes de información y desarrolladores de historiales electrónicos prácticas que interfieran con el acceso, intercambio o uso de información electrónica de salud, salvo ocho excepciones reglamentarias. Las quejas van a la ONC.

**California.** La ley estatal de acceso del paciente (Health & Saf. Code §§ 123100 y ss.) es más rápida: inspección en 5 días laborables y copias en 15 días (§ 123130), con tarifas máximas legales.

*Notas personales de estudio; no constituyen asesoría médica ni legal.*

---

## 한국어 (초역, 교정 대기)

미국에서 진료기록은 법적으로 '내 것'일까요? 차트 자체는 의료기관이 보관하지만, HIPAA 프라이버시 규칙(45 C.F.R. Part 164, Subpart E)은 정보에 대한 연방 권리를 줍니다: 열람, 사본 취득, 정정 요청, 제3자 지정 전송이 그것입니다.

**접근권 — 30일 이내.** § 164.524(a)에 따라 지정 기록집합(designated record set)에 있는 본인의 보호대상 건강정보(PHI)를 열람하고 사본을 받을 수 있습니다. 기관은 원칙적으로 30일 이내 조치해야 하며(§ 164.524(b)(2)) 서면으로 한 번, 최대 30일 연장할 수 있습니다. 전자적으로 보관되는 정보는 요청한 전자 형식으로 받을 수 있습니다(§ 164.524(c)(2)(ii)). 수수료는 합리적인 실비 기준으로 제한되며 전자 기록에 페이지당 요금은 적용되지 않습니다.

**거부 사유는 좁습니다.** § 164.524(a)(2)–(3)는 심사가능/불가능한 거부 사유를 열거합니다(예: 면허 전문직이 접근 시 생명·안전이 위태롭다고 판단한 경우). 거부는 이유와 함께 서면 통지되어야 합니다.

**제3자 직접 전송.** § 164.524(c)(3)(ii)에 따라 사본을 지정한 제3자에게 직접 보내도록 서면 지시할 수 있습니다. Ciox Health v. Azar, 435 F. Supp. 3d 30 (D.D.C. 2020) 이후 기업이 요청한 제3자 전송에는 수수료 상한이 확장 적용되지 않지만, 본인 요청에 대한 상한은 그대로입니다.

**정정권 — 요구할 권리이지 일방적으로 고칠 권리는 아닙니다.** § 164.526에 따라 부정확·불완전한 정보의 정정을 요청할 수 있고, 기관은 60일 이내 답해야 하며(30일 연장 가능) 거부 시 서면 사유를 밝혀야 하고, 본인은 이의 진술서(statement of disagreement)를 기록에 첨부할 수 있습니다.

**정보 차단(information blocking).** 21세기 치유법(Cures Act) § 4004를 시행한 45 C.F.R. Part 171은 의료제공자·건강정보네트워크·인증 EHR 업체가 전자 건강정보의 접근·교환·사용을 방해할 수 있는 행위를 금지하며, 8가지 법정 예외만 인정합니다. 신고는 ONC에 합니다.

**캘리포니아 상층 규정.** 환자 열람법(Health & Saf. Code §§ 123100 이하)은 더 빠릅니다: 열람은 통상 5영업일 이내, 사본은 15일 이내 제공(§ 123130), 수수료 법정 상한 적용.

*개인 학습 노트이며 의료·법률 자문이 아닙니다.*

---

## Tiếng Việt (bản dịch sơ bộ, chờ hiệu đính)

Tại Hoa Kỳ, hồ sơ bệnh án có hợp pháp là "của bạn" không? Bản hồ sơ do cơ sở y tế lưu giữ, nhưng Quy tắc Bảo mật HIPAA (45 C.F.R. Part 164, Subpart E) trao cho bạn các quyền liên bang đối với thông tin: xem, lấy bản sao, yêu cầu sửa và chỉ định gửi cho bên thứ ba.

**Quyền truy cập — trong 30 ngày.** Theo § 164.524(a), bạn được xem và nhận bản sao thông tin sức khỏe được bảo vệ của mình trong tập hồ sơ chỉ định. Cơ sở y tế thường phải thực hiện trong 30 ngày (§ 164.524(b)(2)), được gia hạn bằng văn bản một lần tối đa 30 ngày. Nếu thông tin được lưu điện tử, bạn được nhận theo định dạng điện tử yêu cầu (§ 164.524(c)(2)(ii)). Phí bị giới hạn ở mức hợp lý theo chi phí thực tế; phí theo trang không áp dụng cho hồ sơ điện tử.

**Từ chối rất hạn chế.** § 164.524(a)(2)–(3) liệt kê các căn cứ từ chối có thể và không thể xét lại (ví dụ: chuyên gia có giấy phép phán đoán việc truy cập có thể gây nguy hiểm đến tính mạng hoặc an toàn). Mọi từ chối phải bằng văn bản kèm lý do.

**Gửi thẳng cho bên thứ ba.** Theo § 164.524(c)(3)(ii), bạn có thể chỉ thị bằng văn bản để gửi bản sao cho người hoặc tổ chức bạn chỉ định. Sau vụ Ciox Health v. Azar, 435 F. Supp. 3d 30 (D.D.C. 2020), mức trần phí không còn mở rộng sang các lần gửi do công ty bên thứ ba yêu cầu, nhưng trần cho yêu cầu của chính cá nhân không đổi.

**Quyền sửa — quyền yêu cầu, không phải quyền áp đặt.** Theo § 164.526, bạn có thể yêu cầu sửa thông tin không chính xác hoặc không đầy đủ; cơ sở phải trả lời trong 60 ngày (gia hạn một lần 30 ngày) và nếu từ chối phải giải thích bằng văn bản; bạn có quyền nộp tuyên bố không đồng ý để đính kèm hồ sơ.

**Chặn thông tin (information blocking).** Điều 4004 của Đạo luật Cures Thế kỷ 21, được thi hành tại 45 C.F.R. Part 171, cấm nhà cung cấp, mạng thông tin y tế và nhà phát triển EHR có hành vi cản trở việc truy cập, trao đổi hoặc sử dụng thông tin sức khỏe điện tử, trừ tám ngoại lệ theo quy định. Khiếu nại gửi tới ONC.

**Lớp quy định California.** Đạo luật Truy cập Hồ sơ Sức khỏe của Bệnh nhân (Health & Saf. Code §§ 123100 trở đi) nhanh hơn: xem hồ sơ thường trong 5 ngày làm việc và bản sao trong 15 ngày (§ 123130), có trần phí theo luật.

*Ghi chú học tập cá nhân, không phải tư vấn y tế hay pháp lý.*

---

## हिन्दी (प्रारंभिक अनुवाद, समीक्षा लंबित)

संयुक्त राज्य में क्या आपका चिकित्सा रिकॉर्ड कानूनी रूप से "आपका" है? चार्ट प्रदाता के पास रहता है, लेकिन HIPAA गोपनीयता नियम (45 C.F.R. Part 164, Subpart E) आपको जानकारी पर संघीय अधिकार देता है: देखना, प्रति लेना, सुधार माँगना और किसी तीसरे पक्ष को भिजवाना।

**पहुँच का अधिकार — 30 दिनों के भीतर।** § 164.524(a) के अंतर्गत आप निर्दिष्ट रिकॉर्ड सेट में अपनी संरक्षित स्वास्थ्य जानकारी देख सकते हैं और उसकी प्रति पा सकते हैं। संस्था को सामान्यतः 30 दिनों के भीतर कार्रवाई करनी होती है (§ 164.524(b)(2)), लिखित रूप से एक बार 30 दिनों तक की वृद्धि संभव है। इलेक्ट्रॉनिक रूप से रखी जानकारी माँगे गए इलेक्ट्रॉनिक प्रारूप में मिल सकती है (§ 164.524(c)(2)(ii))। शुल्क उचित, लागत-आधारित राशि तक सीमित है; इलेक्ट्रॉनिक रिकॉर्ड पर प्रति-पृष्ठ शुल्क लागू नहीं होता।

**इंकार के आधार संकीर्ण हैं।** § 164.524(a)(2)–(3) समीक्षा योग्य और अयोग्य इंकार आधारों को सूचीबद्ध करता है (जैसे लाइसेंसधारी पेशेवर का यह निर्णय कि पहुँच से जीवन या सुरक्षा ख़तरे में पड़ सकती है)। हर इंकार लिखित कारणों सहित होना चाहिए।

**तीसरे पक्ष को सीधा भेजना।** § 164.524(c)(3)(ii) के अनुसार आप लिखित निर्देश देकर प्रति अपने निर्दिष्ट व्यक्ति या संस्था को भिजवा सकते हैं। Ciox Health v. Azar, 435 F. Supp. 3d 30 (D.D.C. 2020) के बाद शुल्क-सीमा तीसरी-पक्ष कंपनियों के अनुरोधों पर विस्तारित नहीं होती, परंतु व्यक्ति के अपने अनुरोध पर सीमा अपरिवर्तित है।

**संशोधन का अधिकार — माँगने का अधिकार है, थोपने का नहीं।** § 164.526 के अंतर्गत ग़लत या अधूरी जानकारी के संशोधन का अनुरोध किया जा सकता है; संस्था को 60 दिनों में उत्तर देना होता है (एक बार 30 दिन की वृद्धि) और इंकार पर लिखित कारण देना होता है; आप असहमति का कथन (statement of disagreement) रिकॉर्ड के साथ संलग्न कर सकते हैं।

**जानकारी अवरोधन (information blocking)।** 21st Century Cures Act की धारा 4004, जिसे 45 C.F.R. Part 171 में लागू किया गया, प्रदाताओं, स्वास्थ्य सूचना नेटवर्कों और प्रमाणित EHR डेवलपर्स को इलेक्ट्रॉनिक स्वास्थ्य जानकारी की पहुँच, विनिमय या उपयोग में बाधा डालने वाले आचरण से रोकती है, आठ नियामक अपवादों को छोड़कर। शिकायत ONC को जाती है।

**California की अतिरिक्त परत।** Patient Access to Health Records Act (Health & Saf. Code §§ 123100 और आगे) तेज़ है: निरीक्षण सामान्यतः 5 कार्यदिवसों में और प्रतियाँ 15 दिनों में (§ 123130), वैधानिक शुल्क-सीमा सहित।

*केवल व्यक्तिगत अध्ययन नोट; यह चिकित्सीय या कानूनी सलाह नहीं है।*
