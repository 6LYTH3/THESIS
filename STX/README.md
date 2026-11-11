# STX — Seagate Technology Holdings plc

**Sector:** Technology / Data Storage / HDD
**Last updated:** 2026-11-11
**Currency:** USD; B = พันล้านดอลลาร์, M = ล้านดอลลาร์
**Reference price:** $501.62 ราคาปิด 2026-11-10 เวลา 16:00 EST ไม่ใช่ราคาสด [5]
**View:** Avoid new buying at the reference price / รอส่วนเผื่อความปลอดภัย

**HTML report:** [เปิดรายงานพร้อมกราฟและ interactive DCF](report.html) — รองรับมือถือ เปิดแบบ offline และพิมพ์เป็น PDF; ใช้ข้อมูลและสมมติฐาน research pass เดิม

> บทวิเคราะห์อิสระภาษาไทย จัดโครงสร้างคล้ายรายงาน fundamental equity research ของ Morningstar ไม่ใช่รายงาน ราคาเป้าหมาย หรือ rating ของ Morningstar ตัวเลขอนาคตทั้งหมดที่ไม่ได้ระบุว่าเป็น guidance คือสมมติฐานของผู้วิเคราะห์

## Summary

Seagate ออกแบบและผลิตอุปกรณ์จัดเก็บข้อมูล โดยกำไรและการเติบโตหลักมาจาก HDD ความจุสูงสำหรับ cloud และ enterprise ไม่ใช่ฮาร์ดดิสก์คอมพิวเตอร์ส่วนบุคคลอย่างที่ภาพจำเดิมอาจทำให้เข้าใจ เทคโนโลยี HAMR/Mozaic ช่วยเพิ่มข้อมูลต่อแผ่นดิสก์ ลดต้นทุนต่อ TB และเพิ่มประสิทธิภาพพื้นที่กับพลังงานของลูกค้า จึงเป็นความได้เปรียบทางวิศวกรรมที่มีคุณค่าจริง อย่างไรก็ตาม รายได้และ margin ล่าสุดได้รับแรงหนุนมากจากราคาขายและภาวะอุปทานตึงตัว ซึ่งไม่ควรถูกตีความเป็นกำไรปกติถาวร ผมประเมิน moat แบบ **Narrow — มีข้อได้เปรียบแต่ไม่ไร้เทียมทาน**, uncertainty **High**, capital allocation **Standard / mixed** และ DCF กรณีฐานประมาณ **$365 ต่อหุ้น** เทียบราคาปิดอ้างอิง $501.62 จึงยังไม่น่าสนใจสำหรับการซื้อใหม่แบบเน้นมูลค่า เว้นแต่เชื่อว่ารายได้หรือความสามารถทำกำไรระยะยาวจะดีกว่ากรณีฐานอย่างมีนัยสำคัญ

### Analyst dashboard — ความเห็นของรายงานนี้ ไม่ใช่ Morningstar ratings

| หัวข้อ | ข้อสรุป |
| --- | --- |
| Business quality | เทคโนโลยีและตำแหน่งตลาดดีขึ้น แต่ยังเป็นผู้ผลิต hardware วัฏจักร |
| Economic moat | Narrow; ต้นทุน/know-how, qualification และ scale |
| Moat trajectory | HAMR ช่วยเสริม แต่คู่แข่งกำลังตามมา; ยังไม่ยืนยันว่ากว้างขึ้นอย่างถาวร |
| Uncertainty | High; ราคา/TB, hyperscaler demand, yield, SSD substitution |
| Capital allocation | Standard / mixed; ลดหนี้ดี แต่ต้องพิสูจน์วินัย buyback และ compliance |
| Fair value, base DCF | ประมาณ $365; ไม่ใช่เป้าหมายราคา 12 เดือน |
| Bear / bull DCF | ประมาณ $183 / $642; ไม่ใช่ขอบเขตขาดทุนสูงสุด/กำไรสูงสุด |
| Price / base fair value | ประมาณ 1.38 เท่า |
| Margin-of-safety zone | ประมาณ $255–$275 หากพื้นฐานและ fair value ไม่เปลี่ยน |

## Business & Financials

### 1. Seagate ทำอะไร และลูกค้าจ่ายเงินซื้ออะไร

HDD เก็บข้อมูลเป็นสัญญาณแม่เหล็กบนจานหมุน ส่วน SSD ใช้ NAND flash ไม่มีจานหมุน ลูกค้า Seagate ไม่ได้ต้องการแค่จำนวนไดรฟ์ แต่ต้องการ **ความจุที่เชื่อถือได้ในต้นทุนตลอดอายุใช้งานที่ต่ำ** ซึ่งรวมราคาไดรฟ์ พลังงาน rack ระบบเครือข่าย การซ่อมบำรุง และความเสี่ยงข้อมูลสูญหาย [1]

| ตลาด | สินค้า/การใช้งาน | เศรษฐศาสตร์และความสำคัญ |
| --- | --- | --- |
| Data Center | Nearline HDD ความจุสูง, enterprise storage systems; object storage, backup, archive, content delivery, data lake | 81% ของรายได้ Q1 FY27 และประมาณ 90% ของ EB ส่งมอบ; เครื่องยนต์หลักของ thesis [2][3] |
| Edge / IoT | NAS, surveillance, personal/external storage, gaming/creative workflows | 19% ของรายได้ Q1 FY27; รายได้ $784M ตาม call; ไม่ควรสมมติว่าเป็น recurring software [3] |

ชื่อผลิตภัณฑ์ที่พบได้ เช่น Exos สำหรับ enterprise, IronWolf สำหรับ NAS, SkyHawk สำหรับ surveillance และ Seagate/LaCie สำหรับผู้ใช้ทั่วไป แต่การประเมินมูลค่ารอบนี้ไม่ได้ตั้ง premium ให้แต่ละแบรนด์แยกกัน เพราะงบไม่ได้เปิดกำไรระดับแบรนด์ให้ตรวจสอบ

FY2026 ช่องทาง OEM คิดเป็น 81% ของรายได้, distributors 13%, retailers 6%; ลูกค้ารายหนึ่งคิดเป็น 14% ของรายได้ทั้งปี [1] อย่าสับสน OEM 81% กับ Data Center 80% ในปีเดียวกัน: เป็นคนละมิติของการแบ่งรายได้ อีกทั้งบริษัทมีหนึ่ง reportable segment; Data Center/Edge เป็น end-market disclosures ไม่ใช่งบกำไรแยก segment [1][2]

**รายได้ส่วนใหญ่เป็นการขาย hardware ไม่ใช่ subscription:** ความต้องการซื้อซ้ำมีอยู่ แต่ปริมาณและราคาอาจผันผวน ลูกค้ารายใหญ่ใช้เวลาทดสอบสินค้าและวางแผนร่วมกับบริษัท แต่ยังมีอำนาจต่อรองและใช้ผู้ขายหลายรายได้ บริษัทจดทะเบียนในไอร์แลนด์ สำนักงานบริหารหลักอยู่สิงคโปร์ และมีการผลิต/ห่วงโซ่อุปทานข้ามประเทศ รวมถึงไทย ไม่ควรมองเป็นธุรกิจสหรัฐล้วน [1]

### 2. HDD อยู่ตรงไหนในยุค AI และจะถูก SSD แทนหรือไม่

Storage มีหลายชั้น ไม่ใช่ผู้ชนะรายเดียวกินทั้งหมด:

- **DRAM/HBM:** ข้อมูลที่ต้องเข้าถึงเร็วมากใกล้การประมวลผล; ไม่ใช่ตลาดที่ HDD แข่งขันโดยตรง
- **SSD:** เหมาะกับ latency ต่ำ, random access และ workload ที่ความเร็วสำคัญกว่า acquisition cost ต่อ TB
- **HDD:** เหมาะกับข้อมูลจำนวนมากที่ต้อง online/nearline ในราคาต่อ TB ต่ำ เช่น data lake, backup, video และ historical datasets
- **Tape:** เหมาะกับ archive บางประเภทที่ยอมรอเข้าถึงข้อมูลได้; เป็นอีกทางเลือก ไม่ใช่มีเพียง HDD กับ SSD

AI ช่วยเพิ่มข้อมูลสำหรับ training, checkpoints, outputs, logs, provenance และการเก็บข้อมูลกลับมาใช้ซ้ำ แต่ **ข้อมูลที่สร้างขึ้นทั้งหมดไม่เท่ากับข้อมูลที่เก็บถาวร และไม่เท่ากับรายได้ Seagate** ต้องผ่าน retention rate, compression/deduplication, replication, storage tier และ market share ก่อน บริษัทไม่ได้เปิดเผยรายได้ AI แยกจาก cloud ทั่วไป จึงไม่ควรสร้างตัวเลขสัดส่วน AI ขึ้นเอง

HBM/DRAM/SSD เป็นชั้นที่เกี่ยวข้องกับ hot KV cache โดยตรงมากกว่า HDD ประโยชน์ต่อ Seagate จาก inference/agents จึงเป็นการสะสม persistent data และ storage tiering ทางอ้อม ไม่ใช่สมมติว่า HDD จะเข้าไปแทนหน่วยความจำความเร็วสูง

**ความเห็น:** SSD แทน HDD ได้บาง workload และเคยทำไปแล้วใน client PC แต่ไม่ได้แปลว่าจะแทน bulk nearline storage ทั้งหมดทันที ต้องเทียบ total cost of ownership และต้นทุน NAND ต่อบิตด้วย รายงานนี้ไม่กำหนดอัตรา HDD/SSD cost ratio ตายตัว เพราะขึ้นกับรุ่น workload และวัฏจักร NAND

### 3. กลไกรายได้: ปริมาณข้อมูล × ราคาต่อ TB

สำหรับ nearline โดยย่อ:

`Revenue ≈ exabytes shipped × 1,000,000 TB/EB × realized price/TB`

ส่วนรายได้รวมยังมีสินค้าประเภทอื่น จึงใช้ revenue รวม / EB รวมเป็นเพียง **blended proxy** ไม่ใช่ราคา nearline ที่บริษัทประกาศ:

- Q1 FY27: $4.233B / 220 EB ≈ **$19.24/TB**
- Q1 FY26: $2.629B / 182 EB ≈ **$14.45/TB**
- proxy เพิ่มประมาณ **33% YoY** ขณะที่ EB รวมเพิ่มประมาณ **21%**; ผลคูณอธิบายการเติบโตรายได้ราว 61% แต่ยังแยก pure pricing ออกจาก mix ไม่ได้ [2]
- เมื่อเทียบ Q4 FY26 รายได้เพิ่มประมาณ 16.6% แต่ EB รวมเพิ่มจาก 218 เป็น 220 หรือ **0.9%**; nearline เพิ่ม 195 เป็น 198 หรือ **1.54%** ตาม 10-Q ข้อขัดแย้งเดิมที่แหล่งรองรายงาน 1–2% จึงคลี่คลายได้ว่าเกิดจากฐาน/การปัดเศษ [2]

**ข้อสรุป:** ผลงานล่าสุดไม่ใช่แค่ขายข้อมูลได้มากขึ้น การขึ้นราคา/เปลี่ยน product mix มีบทบาทใหญ่มาก หากสองอย่างนี้กลับทิศ กำไรอาจลดเร็วกว่าปริมาณ EB

### 4. HAMR/Mozaic: เทคโนโลยีที่เปลี่ยน economics

HAMR ย่อจาก heat-assisted magnetic recording ใช้ความร้อนจากเลเซอร์ที่จุดเล็กมากช่วยเขียนข้อมูลบนสื่อแม่เหล็กความหนาแน่นสูง ช่วยแก้ข้อจำกัดการทำบิตให้เล็กลงโดยยังรักษาเสถียรภาพข้อมูล Mozaic เป็นแพลตฟอร์มของ Seagate ที่รวม media, heads, photonics, controller และกระบวนการผลิต ไม่ใช่เพียงเพิ่มแผ่นจานเข้าไปในกล่อง [1][4]

ตัวอย่างเชิงกลไก ไม่ใช่ต้นทุนจริงบริษัท: หากไดรฟ์ราคาโรงงาน $300 เก็บได้ 30TB ต้นทุนคือ $10/TB ถ้าเพิ่มเป็น 40TB โดยต้นทุนไดรฟ์ยัง $300 จะเหลือ $7.50/TB หรือลด 25% แต่หาก BOM/yield ทำให้ต้นทุนเพิ่มเป็น $360 จะเหลือ $9/TB หรือลดเพียง 10% **ความจุสูงขึ้นไม่ได้รับประกัน cost-down ตามทฤษฎีทั้งหมด**

สถานะตามเอกสาร/คำชี้แจงที่ตรวจสอบ:

- มีนาคม 2026 บริษัทประกาศ Mozaic 4+ สูงสุด 44TB ผ่าน qualification และอยู่ในการผลิตกับ hyperscaler สองราย [4]
- ใน call ตุลาคม 2026 ผู้บริหารยังคาด HAMR ประมาณ 50% ของ nearline EB shipment run rate เมื่อออกจาก CY2026; Mozaic 4 ราวครึ่งหนึ่งของ HAMR ส่วนนี้ **เป็นเป้าหมาย ไม่ใช่ผลสำเร็จที่ยืนยันแล้ว** [3]
- Mozaic 5 ความจุ 50TB+ ตั้งเป้าเริ่มส่งสินค้าเพื่อ customer qualification ปลาย CY2027 ไม่ใช่รับรู้รายได้ mass production เต็มปีตั้งแต่ต้น 2027 [3]
- สาธิต 8TB/disk ในห้องแล็บตาม call; ไม่ใช่สินค้าที่ผลิตจำนวนมากแล้ว [3]
- ผู้บริหารระบุว่า transition มี manufacturing cycle time ยาวขึ้น และ external component costs ขึ้นมาหักล้าง internal cost-down บางส่วน จึงต้องดู yield, scrap, warranty และ cash flow ควบคู่ [3]

### 5. Economic moat — ทำไมผมให้ Narrow ไม่ใช่ Wide

เกณฑ์ที่ใช้คือความน่าจะเป็นที่จะรักษาผลตอบแทนต่อเงินลงทุนสูงกว่าต้นทุนเงินทุนได้นาน ไม่ใช่ดู margin สูงเพียงไตรมาสเดียว

| แหล่งความได้เปรียบ | หลักฐาน/เหตุผล | สิ่งที่จำกัด moat |
| --- | --- | --- |
| Cost advantage | Areal density, ผลิต heads/media เอง, platform reuse และ manufacturing learning | ต้องพิสูจน์ด้วยต้นทุน/TB และ yield จริง; คู่แข่งลดช่องว่างได้ |
| Intangible assets | HAMR engineering know-how, IP, reliability และกระบวนการผลิตที่ซับซ้อน | สิทธิบัตรไม่ใช่ผูกขาด storage; ยังมี alternative architectures |
| Switching costs | Qualification, firmware/system validation และความเสี่ยงเปลี่ยนผู้ขาย | Hyperscaler มีทีมวิศวกรรมและ multi-source; ไม่ใช่ lock-in แบบ enterprise software |
| Efficient scale | ผู้ผลิต HDD หลักมี Seagate, Western Digital และ Toshiba; entrant ใหม่ทำได้ยาก | มีผู้ขายน้อยไม่ได้รับประกันว่าจะไม่แข่งราคา หรือเพิ่ม EB supply มากเกินไป |
| Network effect | ไม่พบเหตุผลเพียงพอให้เครดิต | HDD ของลูกค้ารายหนึ่งไม่ได้ดีขึ้นเพียงเพราะคนอื่นใช้มากขึ้น |

**ข้อโต้แย้งสำคัญ:** WDC รายงาน non-GAAP gross margin Q1 FY27 ราว 58.1% เทียบ STX 57.8% ดังนั้นความเป็นผู้นำ HAMR ยังไม่เท่ากับมี gross margin เหนือคู่แข่งทุกช่วง [6] WDC ระบุเป้าหมายส่ง first-gen HAMR ปริมาณมากใน CY1H2027 และเริ่ม qualification ของ second-gen 5TB/platter ใน CY2H2027 เป็นแผนผู้บริหาร ไม่ใช่การันตี แต่ก็เพียงพอที่จะไม่ให้ monopoly premium กับ Seagate [6]

Toshiba เป็น supply risk ที่ต้องติดตาม แต่รายงานนี้ไม่ใช้ข่าวแผนเพิ่มกำลังผลิตเป็นหลักฐานว่าเกิด oversupply แน่นอน การนับไดรฟ์อย่างเดียวก็ไม่พอ เพราะ supply ในหน่วย EB เพิ่มจาก density ได้แม้ unit capacity คงเดิม

**คำตัดสิน:** Narrow moat จากต้นทุน/วิศวกรรม/qualification เป็นข้อสรุปที่สมเหตุผลกว่า Wide moat แบบบริษัท platform ที่รักษา pricing power ได้โดยไม่ต้องลงทุนแข่งขันเทคโนโลยีต่อเนื่อง หากข้อมูล cost advantage เสื่อมลงถาวร ก็อาจต้องปรับเป็น no moat

### 6. งบการเงิน: ฟื้นตัวจริง แต่ห้ามลืมฐานวัฏจักร

ตัวเลข GAAP จาก 10-K; FCF = operating cash flow − capex [1]

| USD B ยกเว้น EPS/margin | FY2024 | FY2025 | FY2026 |
| --- | ---: | ---: | ---: |
| Revenue | 6.551 | 9.097 | 12.195 |
| Gross margin คำนวณจากงบ | 23.4% | 35.2% | 45.6% |
| Operating income | 0.452 | 1.890 | 4.094 |
| Operating margin | 6.9% | 20.8% | 33.6% |
| Net income | 0.335 | 1.469 | 3.184 |
| Diluted EPS | $1.58 | $6.77 | $13.90 |
| Operating cash flow | 0.918 | 1.083 | 3.674 |
| Capex | 0.254 | 0.265 | 0.569 |
| FCF | 0.664 | 0.818 | 3.105 |

FY2026 มี 53 สัปดาห์ เทียบ FY2025/24 ที่ 52 สัปดาห์ จึงไม่ใช่ calendar comparison ที่เท่ากันทุกประการ ทั้ง FY2024 net income ยังได้ประโยชน์จาก business divestiture gain $313M และ swap termination gain $104M ก่อนภาษี ไม่ควรใช้ EPS อย่างเดียวตัดสิน earnings quality [1]

#### Q1 FY2027 — สิ้นสุด 2 ตุลาคม 2026

| ตัวชี้วัด | ผลประกอบการ |
| --- | ---: |
| Revenue | $4.233B; +61.0% YoY |
| Gross margin | GAAP 57.3%; non-GAAP 57.8% |
| Operating margin | GAAP 48.8%; non-GAAP 50.7% |
| Net income | GAAP $1.761B |
| Diluted EPS | GAAP $7.59; non-GAAP $7.68 |
| Operating cash flow / capex / FCF | $1.690B / $0.211B / $1.479B |
| FCF margin | 34.9% |
| Nearline / total shipments | 198 / 220 EB |
| Unrestricted cash / carrying debt | $1.258B / $2.351B ณ วันสิ้นไตรมาส |
| Quarterly dividend ล่าสุดที่ประกาศ | $0.76 หรือ $3.04 annualized |

ที่มา [2][7] Guidance Q2 FY27 คือ revenue **$4.8B ±$0.1B**, non-GAAP EPS **$9.20 ±$0.20** ไม่ใช่ guidance ทั้งปี ตัวเลข Q2 revenue midpoint เทียบ $2.825B ปีก่อนคิดเป็นเติบโตราว 70% ไม่ใช่ 7% ที่ปรากฏใน transcript บางช่วง [3][7]

#### Earnings quality — ประเด็นที่ซ่อนอยู่หลัง EPS

1. **GAAP ใกล้ adjusted ไม่ได้หมายความว่าไม่มี adjustments:** Q1 มีการบวกกลับ SBC-related $77M, debt losses $44M และรายการอื่น แต่หัก income-tax adjustments $107M จึงหักล้างกันจน EPS ต่างเพียง $0.09 อัตราภาษี GAAP ราว 11.2% ต่ำกว่า non-GAAP projected FY27 rate 15.5%; DCF ใช้ normalized 17% [7]
2. **FCF ไม่ใช่กำไรบนกระดาษล้วน:** Q1 สร้างเงินสดจริงแม้ receivables ใช้เงิน $283M และ inventory ใช้เงิน $129M แต่ accrued expenses/tax/warranty ช่วยเงินสด $272M จังหวะรายการเหล่านี้กลับทิศได้ [2]
3. **Inventory ต้องพิสูจน์:** สินค้าคงคลัง $1.700B เทียบ $1.571B ไตรมาสก่อน; ส่วนใหญ่เป็น work-in-process $1.156B ผู้บริหารบอกว่าเตรียมสินค้าเพื่อ qualification และ inventory days เพิ่ม 83 → 97 วัน ต้องเห็นเปลี่ยนเป็น shipment/เงินสดจริง ไม่ใช่ถือเป็นคำอธิบายที่ปิดความเสี่ยงได้แล้ว [2][3]
4. **Capex มากกว่า D&A:** Q1 $211M เทียบ $76M; FY26 $569M เทียบ $276M การใช้ EBITDA แทน owner cash flow จึงไม่เหมาะ [1][2]
5. **SBC เป็นต้นทุนผู้ถือหุ้น:** cash-flow SBC Q1 $63M ต่างจาก SBC-related adjustments $77M เพราะนิยามต่างกัน DCF เก็บ SBC เป็น expense ผ่าน margin และไม่บวกกลับ จึงไม่คิดประโยชน์ซ้ำ [2][7]
6. **Restricted cash ไม่ใช่เงินเหลือให้ผู้ถือหุ้น:** Q1 มี restricted cash $112M รวม escrow คดีหลักทรัพย์ $105M เงินที่ย้ายไป escrow ไม่ได้ลด CFO จากการเป็น internal cash transfer แต่ลดสภาพคล่องที่ใช้ได้ ไม่ควรตีความ reported FCF ว่าแจกจ่ายได้ทั้งหมด [2]

#### งบดุลและผลตอบแทนต่อเงินลงทุน

บริษัทชำระหนี้ principal ประมาณ $1.2B ใน Q1 และอีก $750M หลังสิ้นไตรมาส จน principal เหลือราว $1.6B [7] **ไม่ควรนำหนี้หลังไตรมาสไปหัก cash สิ้นไตรมาสแล้วเรียกว่า net debt ล่าสุด** เพราะการคืนหนี้ใช้ cash และระหว่างนั้นมีการดำเนินธุรกิจ รายงานใช้ balance-sheet bridge วันเดียวกัน และไม่เรียก Seagate ว่า debt-free

ROIC ปัจจุบันดูสูงมากเพราะกำไรเพิ่มเร็วและฐานทุนบัญชีค่อนข้างเล็ก แต่เครื่องจักรมี accumulated depreciation สูง และ R&D ถูกบันทึกเป็นค่าใช้จ่าย ทั้ง historical buybacks/convertibles ก็ทำให้ ROE และ book equity ตีความยาก จึงไม่ใช้ headline ROIC เป็นข้อพิสูจน์ moat ระยะยาวโดยลำพัง

### 7. Management และ capital allocation

- CEO Dave Mosley และ CFO Gianluca Romano ให้น้ำหนัก density, build-to-order และ profitability มากกว่าชิงส่วนแบ่งด้วย unit expansion; เป็นแนวทางที่เหมาะกับอุตสาหกรรมนี้ แต่ควรประเมินจาก cash return ตลอดวัฏจักร [3]
- การลดหนี้ช่วงกระแสเงินสดแข็งแรงลดความเสี่ยงจริง ดีกว่านำเงินทั้งหมดไป buyback ในช่วง peak valuation
- Q1 ซื้อหุ้นคืน $400M และจ่ายปันผล $168M; ณ call วงเงิน buyback คงเหลือ $4.4B และตั้งใจเพิ่ม buyback ตั้งแต่ CY2027 แต่ authorization ไม่ใช่สัญญาว่าจะซื้อครบ [3]
- จำนวนหุ้นปลาย Q1 ราว 230M เทียบ 227M สิ้น FY26 และ diluted average เพิ่ม YoY แม้ซื้อคืน จึงต้องดู net share count รวม conversions/employee awards ไม่ใช่ดู buyback headline อย่างเดียว [2]
- BIS settlement ปี 2023 จำนวน $300M สะท้อน compliance risk ที่เกิดขึ้นจริง ไม่ใช่ความเสี่ยงสมมติ ยังมี balance คงค้าง $105M ณ Q1 FY27 และมีภาระ audit; คดีหลักทรัพย์อีกกรณีมีบริษัทออก $105M เข้าบัญชี escrow แล้ว โดย final approval hearing กำหนด 17 พ.ย. 2026 ณ วันที่รายงานยังไม่เกิดขึ้น [2][8]

**Standard / mixed:** ให้เครดิต deleveraging แต่ยังไม่ให้ premium rating จนเห็น buyback ต่ำกว่ามูลค่าเหมาะสมอย่างสม่ำเสมอและการควบคุม compliance ที่ดี ไม่มีการประเมิน compensation alignment อย่างเต็มรูปแบบจาก proxy ในรอบนี้

## Bull case

- **Structural density gains:** HAMR เพิ่ม EB โดยไม่ต้องเพิ่มไดรฟ์ตามสัดส่วน ส่งผลให้ capex 4–6% ของรายได้รองรับการเติบโตได้ตามเป้าผู้บริหาร [3]
- **Demand duration ยาวกว่าวัฏจักรเดิม:** cloud retention, enterprise datasets, inference outputs และ agent/physical AI อาจขยายฐานข้อมูลที่ต้องเก็บต่อเนื่องหลังจบการซื้อ GPU ระยะแรก
- **สัญญายาวช่วย planning:** ตาม call ส่วนใหญ่ของ nearline supply ถูกจัดสรรถึง CY2028 และบาง agreement ถึง CY2030; configuration/pricing ของ CY2027 ระบุไว้ แต่ CY2028 ยังต้อง finalize จึงให้เครดิต visibility ไม่ใช่ตีเป็น guaranteed backlog ทั้งหมด [3]
- **Operating leverage และเงินสด:** ฐาน R&D/SG&A ไม่ต้องโตตามรายได้ทุกดอลลาร์ หาก pricing ยังดี กำไรและเงินสดต่อหุ้นอาจโตแรง พร้อมลดความเสี่ยงหนี้
- **Bull valuation ยังสูงกว่าราคาอ้างอิง:** DCF ประมาณ $642 หากรายได้ถึง $43B ในปีที่สิบและ terminal operating margin ยัง 44% เป็นไปได้แต่ต้องอาศัย structural profitability ที่แข็งแกร่งมาก

## Bear case

| ความเสี่ยง | กลไกกระทบมูลค่า | สิ่งที่ต้องติดตาม |
| --- | --- | --- |
| ราคากลับสู่ปกติ | Revenue/TB กับ margin ลดพร้อมกัน; P/E ดูถูกก่อน EPS ถูกปรับลง | Realized price/TB, price-cost spread, contract resets |
| Hyperscaler digestion | ลูกค้าเลื่อนรับมอบ/ลดการลงทุน/ต่อรอง terms | EB growth, pushouts, customer plans, inventory |
| HAMR execution | Yield, scrap, reliability และ qualification ใช้เวลา/เงินมากกว่าคาด | Warranty, WIP, capex, cost/TB, actual customer ramp |
| Supply เพิ่มจากคู่แข่ง | Density gain เพิ่ม EB supply ได้แม้ไม่เปิดโรงงานใหม่ | WDC/Toshiba output และ capacity roadmap ที่ทำได้จริง |
| SSD/Tape substitution | มูลค่าการประหยัดด้วย HDD ลดลงในบาง workload | Relative TCO และ NAND price/cost trends |
| Customer concentration | ลูกค้ารายใหญ่รายเดียวมีผล disproportionate | FY26 รายหนึ่ง 14%; diversification และ contract quality |
| Trade/compliance/supply chain | ขายบางตลาดไม่ได้ ต้นทุนสูงขึ้น หรือส่วนประกอบขาด | Export controls, audits, tariffs, production continuity |

ปัจจัย electricity/data-center permitting และ AI policy เป็น demand risk ที่ควรทำ sensitivity แต่รายงานนี้ **ไม่สมมติว่าข่าวการเมืองเท่ากับกฎหมายที่บังคับใช้แล้ว** หรืออ้างว่าเป็นสาเหตุราคาหุ้นทุกครั้ง

**Stress test ง่าย ๆ:** ที่รายได้ $19B หาก operating margin ลด 5 percentage points จะเสีย EBIT $0.95B; หลังภาษี 17% คิดเป็นราว **$3.38 ต่อ diluted share** ก่อนผลต้นทุนเงินทุน ส่วน margin ลด 10 จุดมีผลราว $6.77 ต่อหุ้น จึงอ่อนไหวกว่าที่ forward P/E ต่ำบอก

## Valuation

### 1. ตลาดกำลังจ่ายเท่าไร

ใช้ราคา $501.62 [5], จำนวนหุ้นสิ้นไตรมาสแบบปัดเศษ 230M: market cap ประกอบการคำนวณประมาณ **$115.4B** ไม่ใช่ live market cap (10-Q ระบุหุ้น 229.561M ณ 26 ต.ค.; DCF ใช้ diluted 233M เพื่อระวัง dilution)

| วิธีดู | ตัวตั้ง | ผล ณ ราคาอ้างอิง |
| --- | --- | ---: |
| Trailing GAAP P/E | EPS FY26 $13.90 − Q1 FY26 $2.43 + Q1 FY27 $7.59 ≈ $19.06 | 26.3x |
| Q1 adjusted annualized P/E | $7.68 × 4 = $30.72; ไม่ใช่ annual forecast | 16.3x |
| Q2 guide annualized P/E | $9.20 × 4 = $36.80; ไม่ใช่ normalized EPS | 13.6x |
| TTM FCF yield | $3.105B − $0.427B + $1.479B = $4.157B / market cap | 3.6% |
| Q1 annualized FCF yield | $1.479B × 4 / market cap; ไม่ใช่ forecast | 5.1% |
| Dividend yield | $3.04 annualized / price; ไม่รับประกันคงเดิม | 0.61% |

**13.6x ของกำไรช่วงแข็งแรงไม่ได้แปลว่า margin of safety สูง** ถ้ากำไร normalize ต่ำลง ตัวหารจะหายไป ส่วน dividend yield ต่ำเกินเป็นแกนหลักของผลตอบแทน

### 2. DCF กรณีฐาน — ประมาณ $365 ต่อหุ้น

รายละเอียดสมมติฐานทุกปีและวิธีคำนวณอยู่ใน [valuation-2026-11-11.md](valuation-2026-11-11.md) ใช้ FCFF, discount rate 10.5%, terminal growth 2.5%, normalized tax 17%, capex 5% ของ revenue, D&A 2%, incremental operating working capital 10% ของรายได้ที่เพิ่มขึ้น และ diluted shares 233M

ปีโมเดลเป็น **12 เดือนข้างหน้าแบบ rolling จากวันประเมิน** ไม่ใช่ FY2027 ที่มี Q1 เกิดขึ้นไปแล้ว ใช้ year-end discounting เพื่อไม่เอา cash flow ในอดีตมาคิดมูลค่าซ้ำ

| USD B | ปี 1 | ปี 2 | ปี 3 | ปี 5 | ปี 10 |
| --- | ---: | ---: | ---: | ---: | ---: |
| Revenue | 19.0 | 21.0 | 22.5 | 25.2 | 30.5 |
| Operating margin หลังต้นทุน SBC | 48% | 47% | 45% | 42% | 37% |
| FCFF | 6.85 | 7.36 | 7.58 | 7.91 | 8.35 |

รายได้ปีแรกใกล้ Q2 guide annualized $19.2B แต่ margin ต่ำกว่า near-term adjusted guidance เพราะใช้ normalized economic expenses/เผื่อวงจร ต่อจากนั้นให้รายได้โตประมาณ 5.4% CAGR ระหว่างปี 1–10 แต่ margin ค่อย ๆ ลด ไม่ได้สมมติว่า HDD หายไป และ **terminal margin 37% ยังสูงกว่า FY26 GAAP 33.6%** จึงไม่ใช่กรณีที่มองธุรกิจกลับไปตกต่ำแบบเดิมทั้งหมด

ประมาณการ PV ของ FCFF สิบปี **$46.43B** + PV terminal value **$39.55B** = enterprise value **$85.97B** หัก carrying debt $2.351B บวก unrestricted cash $1.258B และหัก BIS claim $0.105B เหลือ equity value ประมาณ **$84.77B** / 233M ≈ **$364** ปัด fair value เป็น **$365**

Terminal value ราว 46% ของ EV; โครงสร้าง reinvestment ใน terminal implies incremental ROIC ราว 24% สูงกว่า WACC มาก เป็นสมมติฐานที่ให้เครดิต moat อยู่แล้ว ไม่ใช่บังคับ returns ลดเท่าต้นทุนทุนเต็มรูปแบบ หาก moat หายและต้องลงทุนเพิ่ม fair value อาจต่ำกว่านี้

### 3. Bear / base / bull — intrinsic values วันนี้ ไม่ใช่ trading targets

| Scenario | Revenue ปี 1 → 10 | Operating margin ปี 1 → 10 | WACC / terminal g | Fair value | ต่างจาก $501.62 |
| --- | --- | --- | --- | ---: | ---: |
| Bear: price/demand reset | $17B → $24B; ปี 2 ลดเป็น $16B | 40% → 32%; ปี 2–3 30% | 12% / 2% | ~$183 | -64% |
| Base: growth + margin normalization | $19B → $30.5B | 48% → 37% | 10.5% / 2.5% | ~$365 | -27% |
| Bull: structural scarcity/density win | $21B → $43B | 52% → 44% | 10% / 3% | ~$642 | +28% |

ไม่กำหนด probability เทียม ๆ และไม่เรียกช่วงนี้ว่า statistical confidence interval ในทุกกรณียังให้ธุรกิจสร้างกำไรระยะยาว จึงไม่รวม extreme disruption/recall scenario ที่แย่กว่านี้ได้

### 4. Sensitivity — เปลี่ยนแค่ WACC กับ terminal growth

USD ต่อหุ้น; ใช้ operating forecast ฐานเดิมทั้งหมด:

| WACC \ terminal growth | 2.0% | 2.5% | 3.0% |
| --- | ---: | ---: | ---: |
| 9.0% | 430 | 447 | 468 |
| 10.5% | 353 | 364 | 376 |
| 12.0% | 300 | 307 | 314 |

WACC 10.5% เป็น required-return assumption ไม่ใช่ค่าตลาดที่วัดได้แม่นยำ: สมมติ risk-free 4.0% + beta 1.3 × equity risk premium 5.0% ≈ cost of equity 10.5%; debt weight ปัจจุบันต่ำ จึง WACC ใกล้ cost of equity ไม่อ้างว่านี่คือ Treasury yield/beta ล่าสุดที่ตรวจสอบแล้ว

### 5. Reverse DCF — ต้องเชื่ออะไรจึงจะรองรับ $501.62

ตรึงอย่างอื่นตามฐานและเปลี่ยนทีละปัจจัย โมเดลต้องการประมาณ:

1. **รายได้ทั้งเส้นสูงขึ้น 37%:** ปีแรก ~$26.1B และปีที่สิบ ~$41.9B แทน $19B/$30.5B โดย scale ฐาน working capital ก่อนเริ่มโมเดลด้วย เป็น algebraic sensitivity ไม่ใช่ forecast ที่สอดคล้อง guidance ปัจจุบันทุกไตรมาส; หรือ
2. **Operating margin ทุกปีสูงขึ้นราว 13.3 percentage points:** ปีแรก ~61.3%, terminal ~50.3%; เป็นตัวอย่างสมมติฐานที่หนักมากเมื่อไม่เพิ่มรายได้; หรือ
3. **WACC ประมาณ 8.3%** แทน 10.5% ซึ่งต้องยอมรับผลตอบแทนที่ต้องการต่ำกว่าสำหรับธุรกิจที่ผมจัด uncertainty สูง

ตลาดจริงอาจสะท้อนส่วนผสมของรายได้ margin และ discount rate ไม่ใช่ตัวเลือกใดเพียงตัวเดียว ประเด็นคือราคา $502 ต้องการกำไรที่คงอยู่ยาวกว่าแค่ beat งบถัดไป

### 6. P/E cross-check และทำไมต่างจากบทวิเคราะห์เดิม

ถ้าเชื่อ normalized adjusted EPS $35–$40 และยอมจ่าย 14–16x จะได้ $490–$640 เหมือนแนวคิดใน research pass ก่อนหน้า แต่ **multiple นี้ซ่อนสมมติฐานว่ากำไร/FCF จะยืนหรือโตได้นาน** DCF ที่ให้ margin normalize และหัก reinvestment จึงให้มูลค่าต่ำกว่า ไม่ควรเฉลี่ยสองวิธีเพียงเพื่อให้ได้ราคาใกล้ตลาด

รอบ 6 พ.ย. มอง conditionally attractive แถว $459 จาก run-rate EPS และ scenario multiples; รอบนี้เปลี่ยนเป็นไม่ซื้อใหม่ที่ $502 เพราะ (1) ราคาอ้างอิงสูงขึ้นราว 9%, (2) เปลี่ยน anchor เป็น cash-flow duration ตลอดวัฏจักร และ (3) ตรวจสอบ contract pricing/working capital/normalized tax ชัดขึ้น **นี่เป็นการเปลี่ยนวิธีประเมินและข้อสรุป ไม่ใช่การอ้างว่ามี profit warning ใหม่** เก็บรายงานเดิมไว้ใน [research-2026-11-06.md](research-2026-11-06.md)

## Conclusion

**Avoid new buying near $502 / รอดูราคาและความทนทานของกำไร:** Seagate เป็นผู้ผลิต storage ที่มีเทคโนโลยีจริงและฐานะการเงินดีขึ้น แต่ราคาหุ้นยังต้องการความเชื่อมั่นสูงต่อกำไรระยะยาว ภายใต้ DCF ฐาน $365 มี downside ประมาณ 27% และผมต้องการส่วนเผื่อ 25–30% จาก fair value สำหรับ uncertainty ระดับนี้ จึงได้โซนพิจารณาราว **$255–$275** โดยไม่ใช่การคาดการณ์ว่าราคาต้องลงมาถึง และต้องประเมินพื้นฐานใหม่เมื่อถึงราคา

หากถืออยู่ การตัดสินใจต้องอิง expected return จากราคาวันนี้และสัดส่วนความเสี่ยง ไม่ใช่ต้นทุนซื้อเดิมหรือหวังกลับ high เดิม นักลงทุนเชิง growth ที่เชื่อ bull case อาจยอมจ่ายสูงกว่าผม แต่ควรระบุให้ชัดว่ากำลังเดิมพันกับ margin และ cash-flow duration ที่ดีกว่าฐาน ไม่ใช่อ้างเพียง P/E ต่ำ

### สิ่งที่จะทำให้เพิ่ม/ลด fair value

| หลักฐาน | ผลต่อ thesis |
| --- | --- |
| Q2 ทำได้ revenue $4.7–$4.9B, adjusted EPS $9.00–$9.40 พร้อม EB เร่งจริง | ยืนยันการส่งมอบระยะสั้น แต่ไม่เพียงพอให้ขึ้น terminal margin ทันที |
| HAMR run rate/qualifications ถึงเป้า และ cost/TB ลงโดย warranty ไม่พุ่ง | เพิ่มความเชื่อมั่น structural cost moat |
| CY2028 pricing finalized พร้อม terms ที่คุ้มค่าและลูกค้ารับจริง | ลดความไม่แน่นอน cash-flow duration |
| FCF หลัง capex/working capital/SBC economics แข็งแรงต่อเนื่องหลายปี | รองรับ fair value สูงขึ้น ไม่ใช่เฉพาะ adjusted EPS |
| WIP/สินค้าสำเร็จรูปสะสม, pushouts, price-cost spread แคบ, capex เกินแผนซ้ำ | ลด forecast และ fair value |
| WDC/Toshiba เพิ่ม EB supply เร็วกว่าดีมานด์ หรือ SSD TCO ลดช่องว่างอย่างมีนัยสำคัญ | ลด long-run margin/moat assumptions |

## Sources

ตรวจสอบ 2026-11-11 เว้นแต่ระบุเป็นข้อมูลใน research history:

1. **Seagate FY2026 Form 10-K**, ยื่น 4 ส.ค. 2026: Business, risk factors, MD&A, audited statements, customer concentration และ capital allocation — https://www.sec.gov/Archives/edgar/data/1137789/000113778926000159/stx-20260703.htm
2. **Seagate Q1 FY2027 Form 10-Q**, ยื่น 29 ต.ค. 2026, period ended 2 ต.ค.: statements, Notes 2/3/7/11/12, MD&A shipment table และ risk factors — https://www.sec.gov/Archives/edgar/data/1137789/000113778926000309/stx-20261002.htm
3. **Q1 FY2027 earnings call transcript**, call 27 ต.ค. 2026, เผยแพร่ผ่าน Motley Fool 28 ต.ค.: ใช้คำพูดผู้บริหารใน full transcript ไม่ใช่ AI summary; roadmap/contracts เป็น forward-looking — https://www.fool.com/earnings/call-transcripts/2026/10/28/seagate-stx-q1-2027-earnings-call-transcript
4. **Seagate Mozaic 4+ announcement**, 3 มี.ค. 2026; product/efficiency claims มาจากบริษัท ไม่ใช่ independent field study — https://investors.seagate.com/news/news-details/2026/Seagate-Delivers-Industrys-Highest-Capacity-Hard-Drives-with-Next-Generation-Mozaic-4/default.aspx
5. **TECHi STX quote**, snapshot ราคาปิด 10 พ.ย. 2026 16:00 EST $501.62; ตรวจสอบซ้ำกับผลค้นหา Barchart ในรอบนี้ เป็น third-party price ไม่ใช่ exchange-certified/live feed — https://www.techi.com/quote/STX/ ; https://www.barchart.com/stocks/quotes/STX/expected-move
6. **WDC Q1 FY2027 earnings call**, 22 ต.ค. 2026; ใช้เปรียบเทียบ margins และ roadmap ไม่ใช่ full peer valuation — https://news.alphastreet.com/western-digital-corporation-wdc-q1-2027-earnings-call-transcript/
7. **Seagate Q1 FY2027 earnings release**, 27 ต.ค. 2026; results, non-GAAP reconciliation, dividend และ guidance — https://investors.seagate.com/news/news-details/2026/Seagate-Technology-Reports-Fiscal-First-Quarter-2027-Financial-Results/default.aspx
8. **BIS enforcement announcement / order**, 19 เม.ย. 2023; ส่วนยอดค้างและความคืบหน้าปัจจุบันใช้ 10-Q [2] — https://www.bis.gov/press-release/bis-imposes-300-million-penalty-against-seagate-technology-llc-related-shipments-huawei

### ขอบเขตและข้อจำกัด

- ไม่ได้เข้าถึงสัญญาลูกค้าฉบับเต็ม, plant-level yield, proprietary market-share dataset หรือรายงาน Morningstar แบบเสียเงิน จึงไม่อ้างว่ารู้ take-or-pay protection หรือ market share ที่แม่นยำ
- DCF ใช้ balance sheet 2 ต.ค. ไม่ใช่ reconstructed balance sheet 11 พ.ย.; ผลดำเนินงานหลังวันงบ เงินปันผล buybacks และเงินสดที่เกิดเพิ่มยังไม่ทราบครบ ควรอ่าน fair value เป็นค่าประมาณ ไม่ใช่ตัวเลขแม่นยำถึงดอลลาร์
- เป็น fundamental research ไม่ใช่ personalized portfolio/tax advice ไม่มีการประเมินความเหมาะสมส่วนบุคคลหรือค่าเงินบาท/USD
- Historical passes: [3 พ.ย.](research-2026-11-03.md), [6 พ.ย.](research-2026-11-06.md); valuation และ categorical claims ในไฟล์เก่าที่ขัดกับรอบนี้ให้ถือว่าถูก supersede
