# 新型冠状病毒肺炎疫情数据

所有文件均为 UTF-8 编码，用 Excel 打开前请注意编码问题。

使用数据前请务必阅读本 README 文档的相关说明以及各数据文件中的备注。

全部数据来自于国家和全国各省（自治区、直辖市）卫健委以及世界卫生组织（WHO），可能有疏漏。

## 目前包含的数据汇总

- **全国（不含港澳台）**：
  
  新增确诊病例、新增重症病例、新增死亡病例、新增治愈出院、新增疑似病例、累计确诊病例、现有确诊病例、现有重症病例、累计死亡病例、累计治愈出院、现有疑似病例、追踪到密切接触者、已解除医学观察、当日解除医学观察、尚在接受医学观察、累计报告境外输入确诊病例、境外输入现有确诊病例、境外输入现有重症病例、境外输入累计治愈出院、境外输入累计死亡病例、境外输入现有疑似病例、新增无症状感染者、当日转为确诊病例无症状感染者、当日解除隔离无症状感染者、尚在医学观察无症状感染者

  - **湖北省**：
    
    新增确诊病例、新增死亡病例、新增治愈出院、累计确诊病例、累计死亡病例、累计治愈出院、现有在院治疗、在院重症病例、在院危重症病例、现有疑似病例、当日新增疑似病例、当日排除疑似病例、集中隔离疑似病例病例、追踪到密切接触者、已解除医学观察、尚在接受医学观察、新增无症状感染者、当日转为确诊病例无症状感染者、当日解除隔离无症状感染者、尚在医学观察无症状感染者

    
    - **湖北省武汉市**：
      
      新增确诊病例、新增死亡病例、新增治愈出院、累计确诊病例、累计死亡病例、累计治愈出院
    
    - **湖北省其他市（州、林区）**：
      
      累计确诊病例、累计死亡病例、累计治愈出院
  
  - **辽宁省**：
    
    新增确诊病例、新增死亡病例、新增治愈出院、累计确诊病例、累计死亡病例、累计治愈出院、现有在院治疗、在院重症病例、在院危重症病例、追踪到密切接触者、已解除医学观察、尚在接受医学观察、累计报告境外输入确诊病例
    
    - **辽宁省各市**：
      
      累计确诊病例
  
  - **浙江省**：
    
    新增确诊病例、新增治愈出院、累计确诊病例、累计死亡病例、累计治愈出院、追踪到密切接触者、当日解除医学观察、尚在接受医学观察
    
    - **浙江省各市**：
      
      累计确诊病例、累计死亡病例、累计治愈出院
  
  - **内蒙古自治区**：
    
    累计确诊病例、累计死亡病例、累计治愈出院、累计报告境外输入确诊病例、境外输入现有疑似病例
  
  - **北京市、吉林省、黑龙江省**：
    
    累计确诊病例、累计死亡病例、累计治愈出院、累计报告境外输入确诊病例
  
  - **新疆维吾尔自治区（含兵团）**：
    
    累计确诊病例、累计死亡病例、累计治愈出院、尚在接受医学观察
  
  - **西藏自治区、青海省**：
    
    累计确诊病例、累计死亡病例、累计治愈出院

- **中国境外各国家/领地/地区**：
  
  Total confirmed cases, Total deaths, Transmission classification, Days since last reported case, Total cases with travel history to China, Total cases with possible or confirmed transmission outside of China, Likely place of exposure: China, Likely place of exposure: Outside reporting country and outside China, Likely place of exposure: In reporting country, Total cases with site of transmission under investigation

## 国家卫健委通报的数据说明

文件 [`data-nhc.csv`](data-nhc.csv) 中的数据来自[国家卫生健康委员会官方网站](http://www.nhc.gov.cn/)，包括自 2020 年 1 月 20 日起的每日全国新型冠状病毒肺炎疫情最新情况，还包括部分湖北省和武汉市的数据。对其中部分数据说明如下：

- 日期：格式为 `yyyy/M/d`；
- 现有确诊病例：2 月 5 日首次披露时称为“隔离治疗病例”，此后改称“现有确诊病例”；
- 现有疑似病例：1 月 20 日至 1 月 24 日的通报中披露的是“累计报告疑似病例”，1 月 29 日至 2 月 2 日的通报中称作“共有疑似病例”；
- 新增重症病例：该项数据为负数表示重症病例数减少；
- 各地区对某项数据有核减或核增的，会在备注一栏予以说明；
- 国家卫健委的通报中除数据外其他值得关注的事项，也会在备注一栏予以说明。

此外，随着新冠肺炎疫情的发展，国家卫健委每日通报的数据项目会不时发生变化和调整。在文件中，当日未通报的数据项一律留空处理，即使其中部分数据项或可由其他数据项计算而得到。

如果您试图通过计算来补全部分数据，请格外注意计算方法的正确性。例如：与新增重症病例不同，新增疑似病例并不等于当日疑似病例减去前一日疑似病例数。

## 湖北省卫健委通报的数据说明

文件 [`data-hubei.csv`](data-hubei.csv) 中的数据来自[湖北省卫生健康委员会官方网站](http://wjw.hubei.gov.cn/)，包括每日湖北省和武汉市新增确诊、死亡、治愈病例，累计确诊、死亡、治愈病例，尚在院治疗、重症、危重症病例，当日新增、现有、排除、集中隔离疑似病例，以及累计追踪到、已解除医学观察和尚在接受医学观察的密切接触者等数据，还包括分市（州、林区）统计的累计确诊、治愈、死亡病例等数据。

其中，湖北省卫健委自 2 月 20 日才开始每日通报各市（州、林区）累计治愈出院病例数，文件中 2 月 19 日至 2 月 14 日的这一数据是从后一日的累计治愈出院病例数减去该日新增治愈出院病例数所得；2 月 13 日及之前的这一数据是从前一日的累计治愈出院病例数加上当日新增治愈出院病例数所得，这些计算所得的数据均与当日全省累计治愈出院病例数比对一致。其中由于 2 月 4 日湖北省治愈出院病例核减 1 例，导致 2 月 4 日至 2 月 12 日各市（州、林区）累计治愈出院病例数之和比当日全省累计治愈出院病例数大 1。此外，2 月 13 日武汉、黄冈等六市对 12 日 24 时确诊病例（含临床诊断病例）数进行了调整核销，其中核减了 269 例治愈出院病例，当日各市（州、林区）累计治愈出院病例数仅供参考。

## 辽宁省卫健委通报的数据说明

文件 [`data-liaoning.csv`](data-liaoning.csv) 中的数据来自[辽宁省卫生健康委员会官方网站](http://wsjk.ln.gov.cn/)。

辽宁省卫健委的通报没有固定的时间间隔，因此文件中用前两列表明该次通报所对应的起止时间，格式为 `yyyy/MM/dd hh:mm`。

## 全国其余各省（区、市）卫健委通报的数据说明

// TODO：目前完成北京市、吉林省、黑龙江省、西藏自治区、青海省、新疆维吾尔自治区（含兵团）、内蒙古自治区、浙江省。

对于其余各省（区、市），只收集了累计确诊病例、累计治愈出院、累计死亡病例这三项数据，数据来源是各省（区、市）卫健委官网。

其中，对于按自然日通报疫情数据的省（区、市），第一列为 `日期`，格式为 `yyyy/M/d`，表示截至该日 24 时（即次日 0 时）的疫情数据；对于其他省（区、市），第一列为 `截至`，格式为 `yyyy/MM/dd hh:mm`，表示截至该时刻的疫情数据。

## 港澳台地区的数据说明

// TODO

## 其他国家和地区的数据说明

文件 [`data-who.csv`](data-who.csv) 中的数据来自世界卫生组织（WHO）每日发布的 [Situation Report](situation_reports)，使用数据前请务必仔细阅读各 Situation Report 来查看各项数据的解释和说明。

## 其他数据源推荐

### 阿里巴巴

接口URL：`https://cdn.mdeer.com/data/yqstaticdata.js`

数据格式：JSON

Demo
```html
<script>
window.callbackstaticdata = function(res){
    console.log(res);
    // 数据输出
    console.log(JSON.stringify(res));
}

// t 为时间戳，防止缓存
$.getScript("https://cdn.mdeer.com/data/yqstaticdata.js?callback=callbackstaticdata&t="+(+new Date));
</script>
```

### 新浪

`https://gwpre.sina.cn/interface/fymap2020_data.json`

### 网易

`https://c.m.163.com/ug/api/wuhan/app/data/list-total`

`https://c.m.163.com/ug/api/wuhan/app/data/list-by-area-code?areaCode=`

### 约翰斯·霍普金斯大学

`https://github.com/CSSEGISandData/COVID-19`